# Comparing `tmp/terrascope-api-1.0.40.2.tar.gz` & `tmp/terrascope-api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrascope-api-1.0.40.2.tar", last modified: Mon May 13 17:29:13 2024, max compression
+gzip compressed data, was "terrascope-api-1.0.5.tar", last modified: Mon Dec 19 20:09:27 2022, max compression
```

## Comparing `terrascope-api-1.0.40.2.tar` & `terrascope-api-1.0.5.tar`

### file list

```diff
@@ -1,90 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:29:13.130298 terrascope-api-1.0.40.2/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-05-12 21:47:19.000000 terrascope-api-1.0.40.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      212 2024-05-13 17:29:13.128984 terrascope-api-1.0.40.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-12 21:47:19.000000 terrascope-api-1.0.40.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 17:29:13.131881 terrascope-api-1.0.40.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1198 2023-05-12 21:47:19.000000 terrascope-api-1.0.40.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:29:12.568415 terrascope-api-1.0.40.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:29:12.570160 terrascope-api-1.0.40.2/src/py/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:29:12.605756 terrascope-api-1.0.40.2/src/py/terrascope_api/
--rw-r--r--   0 root         (0) root         (0)      384 2023-05-12 21:47:19.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2084 2023-05-12 21:47:19.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/async_client.py
--rw-r--r--   0 root         (0) root         (0)     3622 2023-08-17 19:49:30.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/async_interceptors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:29:12.936093 terrascope-api-1.0.40.2/src/py/terrascope_api/models/
--rw-------   0 root         (0) root         (0)     1481 2024-05-13 17:29:06.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/__init__.py
--rw-------   0 root         (0) root         (0)     5823 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/algorithm_computation_pb2.py
--rw-------   0 root         (0) root         (0)     7940 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/algorithm_config_pb2.py
--rw-------   0 root         (0) root         (0)     1995 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/algorithm_manifest_pb2.py
--rw-------   0 root         (0) root         (0)     4241 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/algorithm_pb2.py
--rw-------   0 root         (0) root         (0)     9291 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/algorithm_version_pb2.py
--rw-------   0 root         (0) root         (0)     6393 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/analysis_computation_pb2.py
--rw-------   0 root         (0) root         (0)     8832 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/analysis_config_pb2.py
--rw-------   0 root         (0) root         (0)     4154 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/analysis_pb2.py
--rw-------   0 root         (0) root         (0)     5975 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/analysis_version_pb2.py
--rw-------   0 root         (0) root         (0)     6030 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/aoi_catalog_pb2.py
--rw-------   0 root         (0) root         (0)     5922 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/aoi_collection_pb2.py
--rw-------   0 root         (0) root         (0)     2890 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/aoi_export_pb2.py
--rw-------   0 root         (0) root         (0)     6316 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/aoi_pb2.py
--rw-------   0 root         (0) root         (0)     2742 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/aoi_transaction_pb2.py
--rw-------   0 root         (0) root         (0)     5713 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/aoi_version_pb2.py
--rw-------   0 root         (0) root         (0)     1132 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/common_models_pb2.py
--rw-------   0 root         (0) root         (0)     8435 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/credit_pb2.py
--rw-------   0 root         (0) root         (0)     7107 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/data_search_pb2.py
--rw-------   0 root         (0) root         (0)     2748 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/data_source_pb2.py
--rw-------   0 root         (0) root         (0)     3318 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/data_type_pb2.py
--rw-------   0 root         (0) root         (0)     1717 2024-05-13 17:29:04.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/forgot_password_pb2.py
--rw-------   0 root         (0) root         (0)     3949 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/imagery_pb2.py
--rw-------   0 root         (0) root         (0)     5596 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/notification_pb2.py
--rw-------   0 root         (0) root         (0)     3693 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/permission_pb2.py
--rw-------   0 root         (0) root         (0)    17759 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/project_pb2.py
--rw-------   0 root         (0) root         (0)     9885 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/result_pb2.py
--rw-------   0 root         (0) root         (0)     1712 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/system_pb2.py
--rw-------   0 root         (0) root         (0)     3261 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/tile_pb2.py
--rw-------   0 root         (0) root         (0)     4970 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/toi_pb2.py
--rw-------   0 root         (0) root         (0)     1691 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/token_pb2.py
--rw-------   0 root         (0) root         (0)     6497 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/user_collection_pb2.py
--rw-------   0 root         (0) root         (0)     5461 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/user_pb2.py
--rw-------   0 root         (0) root         (0)     7306 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/models/visualization_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:29:13.124237 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/
--rw-------   0 root         (0) root         (0)     1646 2024-05-13 17:29:06.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/__init__.py
--rw-------   0 root         (0) root         (0)    10536 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/algorithm_computation_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    16037 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/algorithm_config_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     3869 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/algorithm_manifest_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     9291 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/algorithm_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    15021 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/algorithm_version_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    10270 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/analysis_computation_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    11717 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/analysis_config_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     7358 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/analysis_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     8517 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/analysis_version_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    11307 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/aoi_catalog_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    13216 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/aoi_collection_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     5504 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/aoi_export_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     9205 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/aoi_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     5800 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/aoi_transaction_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     7599 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/aoi_version_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     1130 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/common_models_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    16564 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/credit_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    12951 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/data_search_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     5380 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/data_source_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     6949 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/data_type_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     3880 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/forgot_password_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     3649 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/imagery_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    12686 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/notification_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     5782 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/permission_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    29742 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/project_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    11112 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/result_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     3585 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/system_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     3510 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/tile_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     8759 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/toi_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     3720 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/token_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    14660 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/user_collection_pb2_grpc.py
--rw-------   0 root         (0) root         (0)    16154 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/user_pb2_grpc.py
--rw-------   0 root         (0) root         (0)     9882 2024-05-13 17:29:05.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/visualization_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-12 21:47:19.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/sync_client.py
--rw-r--r--   0 root         (0) root         (0)     5136 2024-05-13 17:23:50.000000 terrascope-api-1.0.40.2/src/py/terrascope_api/terrascope_base_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:29:12.626506 terrascope-api-1.0.40.2/src/py/terrascope_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      212 2024-05-13 17:29:12.000000 terrascope-api-1.0.40.2/src/py/terrascope_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3825 2024-05-13 17:29:12.000000 terrascope-api-1.0.40.2/src/py/terrascope_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 17:29:12.000000 terrascope-api-1.0.40.2/src/py/terrascope_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-13 17:29:12.000000 terrascope-api-1.0.40.2/src/py/terrascope_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-13 17:29:12.000000 terrascope-api-1.0.40.2/src/py/terrascope_api.egg-info/top_level.txt
+drwxr-xr-x   0 sjawahar   (501) staff       (20)        0 2022-12-19 20:09:27.822223 terrascope-api-1.0.5/
+-rw-r--r--   0 sjawahar   (501) staff       (20)     1061 2022-12-12 15:59:49.000000 terrascope-api-1.0.5/LICENSE
+-rw-r--r--   0 sjawahar   (501) staff       (20)      164 2022-12-19 20:09:27.820129 terrascope-api-1.0.5/PKG-INFO
+-rw-r--r--   0 sjawahar   (501) staff       (20)      579 2022-09-14 22:43:22.000000 terrascope-api-1.0.5/README.md
+-rw-r--r--   0 sjawahar   (501) staff       (20)       38 2022-12-19 20:09:27.822517 terrascope-api-1.0.5/setup.cfg
+-rw-r--r--   0 sjawahar   (501) staff       (20)     1150 2022-12-19 20:07:44.000000 terrascope-api-1.0.5/setup.py
+drwxr-xr-x   0 sjawahar   (501) staff       (20)        0 2022-12-19 20:09:27.759745 terrascope-api-1.0.5/src/
+drwxr-xr-x   0 sjawahar   (501) staff       (20)        0 2022-12-19 20:09:27.760124 terrascope-api-1.0.5/src/py/
+drwxr-xr-x   0 sjawahar   (501) staff       (20)        0 2022-12-19 20:09:27.765404 terrascope-api-1.0.5/src/py/terrascope_api/
+-rw-r--r--   0 sjawahar   (501) staff       (20)      384 2022-12-12 15:59:49.000000 terrascope-api-1.0.5/src/py/terrascope_api/__init__.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     6051 2022-12-19 20:00:29.000000 terrascope-api-1.0.5/src/py/terrascope_api/async_client.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     3615 2022-12-12 15:59:49.000000 terrascope-api-1.0.5/src/py/terrascope_api/async_interceptors.py
+drwxr-xr-x   0 sjawahar   (501) staff       (20)        0 2022-12-19 20:09:27.792665 terrascope-api-1.0.5/src/py/terrascope_api/models/
+-rw-r--r--   0 sjawahar   (501) staff       (20)     1174 2022-12-19 20:02:45.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/__init__.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     5481 2022-12-19 20:02:37.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/algorithm_computation_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     7454 2022-12-19 20:02:37.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/algorithm_config_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     1869 2022-12-19 20:02:38.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/algorithm_manifest_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     3947 2022-12-19 20:02:38.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/algorithm_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     8661 2022-12-19 20:02:38.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/algorithm_version_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     5698 2022-12-19 20:02:38.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/analysis_computation_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     7294 2022-12-19 20:02:38.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/analysis_config_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     3860 2022-12-19 20:02:38.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/analysis_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     5681 2022-12-19 20:02:38.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/analysis_version_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     5461 2022-12-19 20:02:38.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/aoi_collection_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     5938 2022-12-19 20:02:38.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/aoi_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     2568 2022-12-19 20:02:38.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/aoi_transaction_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     4446 2022-12-19 20:02:38.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/aoi_version_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     1054 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/common_models_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     7251 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/credit_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     2507 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/data_source_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     2800 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/data_type_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     3423 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/permission_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     6104 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/result_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     1555 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/system_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     2586 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/tile_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     4604 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/toi_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     1565 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/token_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     3285 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/user_collection_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     3029 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/user_pb2.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     5071 2022-12-19 20:02:39.000000 terrascope-api-1.0.5/src/py/terrascope_api/models/visualization_pb2.py
+drwxr-xr-x   0 sjawahar   (501) staff       (20)        0 2022-12-19 20:09:27.817769 terrascope-api-1.0.5/src/py/terrascope_api/stubs/
+-rw-r--r--   0 sjawahar   (501) staff       (20)     1304 2022-12-19 20:02:45.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/__init__.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     8881 2022-12-19 20:02:40.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/algorithm_computation_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)    13880 2022-12-19 20:02:40.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/algorithm_config_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     2724 2022-12-19 20:02:40.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/algorithm_manifest_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     7648 2022-12-19 20:02:40.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/algorithm_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)    13032 2022-12-19 20:02:41.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/algorithm_version_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     8616 2022-12-19 20:02:41.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/analysis_computation_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     6229 2022-12-19 20:02:41.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/analysis_config_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     5885 2022-12-19 20:02:41.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/analysis_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     7036 2022-12-19 20:02:41.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/analysis_version_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)    11230 2022-12-19 20:02:42.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/aoi_collection_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     7568 2022-12-19 20:02:42.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/aoi_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     4489 2022-12-19 20:02:42.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/aoi_transaction_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     6123 2022-12-19 20:02:42.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/aoi_version_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)      159 2022-12-19 20:02:42.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/common_models_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)    14248 2022-12-19 20:02:43.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/credit_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     4073 2022-12-19 20:02:43.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/data_source_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     5475 2022-12-19 20:02:43.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/data_type_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     4476 2022-12-19 20:02:43.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/permission_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     4258 2022-12-19 20:02:43.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/result_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     2452 2022-12-19 20:02:43.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/system_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     2379 2022-12-19 20:02:44.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/tile_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     7122 2022-12-19 20:02:44.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/toi_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     2588 2022-12-19 20:02:44.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/token_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     6023 2022-12-19 20:02:44.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/user_collection_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     7298 2022-12-19 20:02:44.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/user_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     4439 2022-12-19 20:02:44.000000 terrascope-api-1.0.5/src/py/terrascope_api/stubs/visualization_pb2_grpc.py
+-rw-r--r--   0 sjawahar   (501) staff       (20)     5507 2022-12-19 20:00:29.000000 terrascope-api-1.0.5/src/py/terrascope_api/sync_client.py
+drwxr-xr-x   0 sjawahar   (501) staff       (20)        0 2022-12-19 20:09:27.768244 terrascope-api-1.0.5/src/py/terrascope_api.egg-info/
+-rw-r--r--   0 sjawahar   (501) staff       (20)      164 2022-12-19 20:09:27.000000 terrascope-api-1.0.5/src/py/terrascope_api.egg-info/PKG-INFO
+-rw-r--r--   0 sjawahar   (501) staff       (20)     3088 2022-12-19 20:09:27.000000 terrascope-api-1.0.5/src/py/terrascope_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sjawahar   (501) staff       (20)        1 2022-12-19 20:09:27.000000 terrascope-api-1.0.5/src/py/terrascope_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sjawahar   (501) staff       (20)       30 2022-12-19 20:09:27.000000 terrascope-api-1.0.5/src/py/terrascope_api.egg-info/requires.txt
+-rw-r--r--   0 sjawahar   (501) staff       (20)       15 2022-12-19 20:09:27.000000 terrascope-api-1.0.5/src/py/terrascope_api.egg-info/top_level.txt
```

### Comparing `terrascope-api-1.0.40.2/LICENSE` & `terrascope-api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `terrascope-api-1.0.40.2/README.md` & `terrascope-api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `terrascope-api-1.0.40.2/setup.py` & `terrascope-api-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 inject_custom_repository('orbital')
 
 EXCLUDE_FILES = []
 
 setuptools.setup(
     name='terrascope-api',
-    version=get_version('ops/conda-recipe/conda_build_config.yaml'),
+    version='1.0.5',
     description='Terrascope API Client',
     url='https://github.com/orbitalinsight/oi_papi',
     package_dir={'': 'src/py'},
     packages=setuptools.find_packages('src/py', exclude=[
         'mocked_services',
         'oi_papi',
         'oi_papi.*'
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/async_interceptors.py` & `terrascope-api-1.0.5/src/py/terrascope_api/async_interceptors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import importlib
 from typing import Callable, Union
 
 import grpc
 from grpc.aio import \
-    UnaryUnaryClientInterceptor, \
-    UnaryStreamClientInterceptor, \
-    StreamUnaryClientInterceptor, \
-    StreamStreamClientInterceptor, \
+    UnaryUnaryClientInterceptor,\
+    UnaryStreamClientInterceptor,\
+    StreamUnaryClientInterceptor,\
+    StreamStreamClientInterceptor,\
     ClientCallDetails
 from grpc.aio._call import \
-    UnaryUnaryCall, \
-    UnaryStreamCall, \
-    StreamUnaryCall, \
+    UnaryUnaryCall,\
+    UnaryStreamCall,\
+    StreamUnaryCall,\
     StreamStreamCall
 
 from grpc.aio._typing import RequestType, ResponseIterableType, ResponseType, \
     RequestIterableType
 
 if importlib.util.find_spec('oi_tracing'):
     from oi_tracing import inject_current_span
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/__init__.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,30 +3,23 @@
 from . import algorithm_manifest_pb2 as algorithm_manifest
 from . import algorithm_pb2 as algorithm
 from . import algorithm_version_pb2 as algorithm_version
 from . import analysis_computation_pb2 as analysis_computation
 from . import analysis_config_pb2 as analysis_config
 from . import analysis_pb2 as analysis
 from . import analysis_version_pb2 as analysis_version
-from . import aoi_catalog_pb2 as aoi_catalog
 from . import aoi_collection_pb2 as aoi_collection
-from . import aoi_export_pb2 as aoi_export
 from . import aoi_pb2 as aoi
 from . import aoi_transaction_pb2 as aoi_transaction
 from . import aoi_version_pb2 as aoi_version
 from . import common_models_pb2 as common_models
 from . import credit_pb2 as credit
-from . import data_search_pb2 as data_search
 from . import data_source_pb2 as data_source
 from . import data_type_pb2 as data_type
-from . import forgot_password_pb2 as forgot_password
-from . import imagery_pb2 as imagery
-from . import notification_pb2 as notification
 from . import permission_pb2 as permission
-from . import project_pb2 as project
 from . import result_pb2 as result
 from . import system_pb2 as system
 from . import tile_pb2 as tile
 from . import toi_pb2 as toi
 from . import token_pb2 as token
 from . import user_collection_pb2 as user_collection
 from . import user_pb2 as user
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/algorithm_computation_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/algorithm_computation_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: algorithm_computation.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
 
 from terrascope_api.models.common_models_pb2 import *
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x61lgorithm_computation.proto\x12\x07oi.papi\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\"\xf5\x03\n\x14\x41lgorithmComputation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x19\n\x11\x61oi_collection_id\x18\x02 \x01(\t\x12\x16\n\x0e\x61lgo_config_id\x18\x03 \x01(\t\x12\x0e\n\x06toi_id\x18\x04 \x01(\t\x12\x11\n\tinput_ids\x18\x05 \x03(\t\x12\x30\n\x0csubmitted_on\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x05state\x18\x07 \x01(\x0e\x32#.oi.papi.AlgorithmComputation.State\x12\x38\n\x08progress\x18\x08 \x01(\x0b\x32&.oi.papi.AlgorithmComputation.Progress\x12\x32\n\x0elast_execution\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1aO\n\x08Progress\x12\x0f\n\x07running\x18\x01 \x01(\x01\x12\x11\n\tsucceeded\x18\x02 \x01(\x01\x12\x0e\n\x06\x66\x61iled\x18\x03 \x01(\x01\x12\x0f\n\x07no_data\x18\x04 \x01(\x01\"V\n\x05State\x12\x11\n\rUNKNOWN_STATE\x10\x00\x12\x0f\n\x0bNOT_STARTED\x10\x01\x12\x0f\n\x0bIN_PROGRESS\x10\x02\x12\n\n\x06PAUSED\x10\x03\x12\x0c\n\x08\x43OMPLETE\x10\x04\"k\n!AlgorithmComputationCreateRequest\x12\x1b\n\x13\x61lgorithm_config_id\x18\x01 \x01(\t\x12\x19\n\x11\x61oi_collection_id\x18\x02 \x01(\t\x12\x0e\n\x06toi_id\x18\x03 \x01(\t\"w\n\"AlgorithmComputationCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12<\n\x15\x61lgorithm_computation\x18\x02 \x01(\x0b\x32\x1d.oi.papi.AlgorithmComputation\"-\n\x1e\x41lgorithmComputationRunRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"6\n\x1f\x41lgorithmComputationRunResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"V\n\x1e\x41lgorithmComputationGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x9e\x01\n\x1f\x41lgorithmComputationGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12=\n\x16\x61lgorithm_computations\x18\x02 \x03(\x0b\x32\x1d.oi.papi.AlgorithmComputation\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\xb2\x02\n\x1f\x41lgorithmComputationListRequest\x12\x32\n\x05state\x18\x01 \x01(\x0e\x32#.oi.papi.AlgorithmComputation.State\x12\x34\n\x10min_submitted_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10max_submitted_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13\x61lgorithm_config_id\x18\x04 \x01(\t\x12\x0e\n\x06toi_id\x18\x05 \x01(\t\x12\x19\n\x11\x61oi_collection_id\x18\x06 \x01(\t\x12\'\n\npagination\x18\x07 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x9f\x01\n AlgorithmComputationListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12=\n\x16\x61lgorithm_computations\x18\x02 \x03(\x0b\x32\x1d.oi.papi.AlgorithmComputation\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination2\x8d\x03\n\x17\x41lgorithmComputationApi\x12\x61\n\x06\x63reate\x12*.oi.papi.AlgorithmComputationCreateRequest\x1a+.oi.papi.AlgorithmComputationCreateResponse\x12X\n\x03run\x12\'.oi.papi.AlgorithmComputationRunRequest\x1a(.oi.papi.AlgorithmComputationRunResponse\x12X\n\x03get\x12\'.oi.papi.AlgorithmComputationGetRequest\x1a(.oi.papi.AlgorithmComputationGetResponse\x12[\n\x04list\x12(.oi.papi.AlgorithmComputationListRequest\x1a).oi.papi.AlgorithmComputationListResponseP\x01\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'algorithm_computation_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_ALGORITHMCOMPUTATION']._serialized_start=95
-  _globals['_ALGORITHMCOMPUTATION']._serialized_end=596
-  _globals['_ALGORITHMCOMPUTATION_PROGRESS']._serialized_start=429
-  _globals['_ALGORITHMCOMPUTATION_PROGRESS']._serialized_end=508
-  _globals['_ALGORITHMCOMPUTATION_STATE']._serialized_start=510
-  _globals['_ALGORITHMCOMPUTATION_STATE']._serialized_end=596
-  _globals['_ALGORITHMCOMPUTATIONCREATEREQUEST']._serialized_start=598
-  _globals['_ALGORITHMCOMPUTATIONCREATEREQUEST']._serialized_end=705
-  _globals['_ALGORITHMCOMPUTATIONCREATERESPONSE']._serialized_start=707
-  _globals['_ALGORITHMCOMPUTATIONCREATERESPONSE']._serialized_end=826
-  _globals['_ALGORITHMCOMPUTATIONRUNREQUEST']._serialized_start=828
-  _globals['_ALGORITHMCOMPUTATIONRUNREQUEST']._serialized_end=873
-  _globals['_ALGORITHMCOMPUTATIONRUNRESPONSE']._serialized_start=875
-  _globals['_ALGORITHMCOMPUTATIONRUNRESPONSE']._serialized_end=929
-  _globals['_ALGORITHMCOMPUTATIONGETREQUEST']._serialized_start=931
-  _globals['_ALGORITHMCOMPUTATIONGETREQUEST']._serialized_end=1017
-  _globals['_ALGORITHMCOMPUTATIONGETRESPONSE']._serialized_start=1020
-  _globals['_ALGORITHMCOMPUTATIONGETRESPONSE']._serialized_end=1178
-  _globals['_ALGORITHMCOMPUTATIONLISTREQUEST']._serialized_start=1181
-  _globals['_ALGORITHMCOMPUTATIONLISTREQUEST']._serialized_end=1487
-  _globals['_ALGORITHMCOMPUTATIONLISTRESPONSE']._serialized_start=1490
-  _globals['_ALGORITHMCOMPUTATIONLISTRESPONSE']._serialized_end=1649
-  _globals['_ALGORITHMCOMPUTATIONAPI']._serialized_start=1652
-  _globals['_ALGORITHMCOMPUTATIONAPI']._serialized_end=2049
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'algorithm_computation_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _ALGORITHMCOMPUTATION._serialized_start=95
+  _ALGORITHMCOMPUTATION._serialized_end=596
+  _ALGORITHMCOMPUTATION_PROGRESS._serialized_start=429
+  _ALGORITHMCOMPUTATION_PROGRESS._serialized_end=508
+  _ALGORITHMCOMPUTATION_STATE._serialized_start=510
+  _ALGORITHMCOMPUTATION_STATE._serialized_end=596
+  _ALGORITHMCOMPUTATIONCREATEREQUEST._serialized_start=598
+  _ALGORITHMCOMPUTATIONCREATEREQUEST._serialized_end=705
+  _ALGORITHMCOMPUTATIONCREATERESPONSE._serialized_start=707
+  _ALGORITHMCOMPUTATIONCREATERESPONSE._serialized_end=826
+  _ALGORITHMCOMPUTATIONRUNREQUEST._serialized_start=828
+  _ALGORITHMCOMPUTATIONRUNREQUEST._serialized_end=873
+  _ALGORITHMCOMPUTATIONRUNRESPONSE._serialized_start=875
+  _ALGORITHMCOMPUTATIONRUNRESPONSE._serialized_end=929
+  _ALGORITHMCOMPUTATIONGETREQUEST._serialized_start=931
+  _ALGORITHMCOMPUTATIONGETREQUEST._serialized_end=1017
+  _ALGORITHMCOMPUTATIONGETRESPONSE._serialized_start=1020
+  _ALGORITHMCOMPUTATIONGETRESPONSE._serialized_end=1178
+  _ALGORITHMCOMPUTATIONLISTREQUEST._serialized_start=1181
+  _ALGORITHMCOMPUTATIONLISTREQUEST._serialized_end=1487
+  _ALGORITHMCOMPUTATIONLISTRESPONSE._serialized_start=1490
+  _ALGORITHMCOMPUTATIONLISTRESPONSE._serialized_end=1649
+  _ALGORITHMCOMPUTATIONAPI._serialized_start=1652
+  _ALGORITHMCOMPUTATIONAPI._serialized_end=2049
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/algorithm_config_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/algorithm_config_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: algorithm_config.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
@@ -34,47 +33,47 @@
 except AttributeError:
   common__models__pb2 = algorithm__version__pb2.common_models_pb2
 
 from terrascope_api.models.common_models_pb2 import *
 from terrascope_api.models.algorithm_pb2 import *
 from terrascope_api.models.algorithm_version_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x61lgorithm_config.proto\x12\x07oi.papi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x13\x63ommon_models.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0f\x61lgorithm.proto\x1a\x17\x61lgorithm_version.proto\"\xbf\x02\n\x0f\x41lgorithmConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12\x34\n\x11\x61lgorithm_version\x18\x02 \x01(\x0b\x32\x19.oi.papi.AlgorithmVersion\x12\'\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12%\n\talgorithm\x18\x04 \x01(\x0b\x32\x12.oi.papi.Algorithm\x12.\n\ncreated_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0eis_deactivated\x18\x06 \x01(\x08\x12\x15\n\ris_deprecated\x18\x07 \x01(\x08\x12\x0c\n\x04name\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\t \x01(\t\x12\x18\n\x10resources_locked\x18\n \x01(\x08\"\x88\x01\n\x1c\x41lgorithmConfigCreateRequest\x12\x1c\n\x14\x61lgorithm_version_id\x18\x01 \x01(\t\x12\'\n\x06params\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"h\n\x1d\x41lgorithmConfigCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x32\n\x10\x61lgorithm_config\x18\x02 \x01(\x0b\x32\x18.oi.papi.AlgorithmConfig\"]\n\x1c\x41lgorithmConfigUpdateRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x31\n\x10\x61lgorithm_config\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"4\n\x1d\x41lgorithmConfigUpdateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"\x85\x01\n\x19\x41lgorithmConfigGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\x14\n\x0c\x61lgorithm_id\x18\x02 \x01(\t\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\x1c\n\x14\x61lgorithm_version_id\x18\x04 \x01(\t\"\x8f\x01\n\x1a\x41lgorithmConfigGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x33\n\x11\x61lgorithm_configs\x18\x02 \x03(\x0b\x32\x18.oi.papi.AlgorithmConfig\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x93\x02\n\x1a\x41lgorithmConfigListRequest\x12\x14\n\x0c\x61lgorithm_id\x18\x01 \x01(\t\x12\x1c\n\x14\x61lgorithm_version_id\x18\x02 \x01(\t\x12\x13\n\x0bsearch_text\x18\x03 \x01(\t\x12\x32\n\x0emin_created_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13include_deactivated\x18\x06 \x01(\x08\x12\'\n\npagination\x18\x07 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x90\x01\n\x1b\x41lgorithmConfigListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x33\n\x11\x61lgorithm_configs\x18\x02 \x03(\x0b\x32\x18.oi.papi.AlgorithmConfig\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"+\n\x1c\x41lgorithmConfigDeleteRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"4\n\x1d\x41lgorithmConfigDeleteResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\".\n\x1f\x41lgorithmConfigDeprecateRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"7\n AlgorithmConfigDeprecateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"/\n AlgorithmConfigDeactivateRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"8\n!AlgorithmConfigDeactivateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r2\x89\x05\n\x12\x41lgorithmConfigApi\x12W\n\x06\x63reate\x12%.oi.papi.AlgorithmConfigCreateRequest\x1a&.oi.papi.AlgorithmConfigCreateResponse\x12N\n\x03get\x12\".oi.papi.AlgorithmConfigGetRequest\x1a#.oi.papi.AlgorithmConfigGetResponse\x12Q\n\x04list\x12#.oi.papi.AlgorithmConfigListRequest\x1a$.oi.papi.AlgorithmConfigListResponse\x12W\n\x06update\x12%.oi.papi.AlgorithmConfigUpdateRequest\x1a&.oi.papi.AlgorithmConfigUpdateResponse\x12`\n\tdeprecate\x12(.oi.papi.AlgorithmConfigDeprecateRequest\x1a).oi.papi.AlgorithmConfigDeprecateResponse\x12\x63\n\ndeactivate\x12).oi.papi.AlgorithmConfigDeactivateRequest\x1a*.oi.papi.AlgorithmConfigDeactivateResponse\x12W\n\x06\x64\x65lete\x12%.oi.papi.AlgorithmConfigDeleteRequest\x1a&.oi.papi.AlgorithmConfigDeleteResponseP\x01P\x03P\x04\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x61lgorithm_config.proto\x12\x07oi.papi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x13\x63ommon_models.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0f\x61lgorithm.proto\x1a\x17\x61lgorithm_version.proto\"\xa5\x02\n\x0f\x41lgorithmConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12\x34\n\x11\x61lgorithm_version\x18\x02 \x01(\x0b\x32\x19.oi.papi.AlgorithmVersion\x12\'\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12%\n\talgorithm\x18\x04 \x01(\x0b\x32\x12.oi.papi.Algorithm\x12.\n\ncreated_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0eis_deactivated\x18\x06 \x01(\x08\x12\x15\n\ris_deprecated\x18\x07 \x01(\x08\x12\x0c\n\x04name\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\t \x01(\t\"\x88\x01\n\x1c\x41lgorithmConfigCreateRequest\x12\x1c\n\x14\x61lgorithm_version_id\x18\x01 \x01(\t\x12\'\n\x06params\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"h\n\x1d\x41lgorithmConfigCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x32\n\x10\x61lgorithm_config\x18\x02 \x01(\x0b\x32\x18.oi.papi.AlgorithmConfig\"]\n\x1c\x41lgorithmConfigUpdateRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x31\n\x10\x61lgorithm_config\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"4\n\x1d\x41lgorithmConfigUpdateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"\x85\x01\n\x19\x41lgorithmConfigGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\x14\n\x0c\x61lgorithm_id\x18\x02 \x01(\t\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\x1c\n\x14\x61lgorithm_version_id\x18\x04 \x01(\t\"\x8f\x01\n\x1a\x41lgorithmConfigGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x33\n\x11\x61lgorithm_configs\x18\x02 \x03(\x0b\x32\x18.oi.papi.AlgorithmConfig\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x93\x02\n\x1a\x41lgorithmConfigListRequest\x12\x14\n\x0c\x61lgorithm_id\x18\x01 \x01(\t\x12\x1c\n\x14\x61lgorithm_version_id\x18\x02 \x01(\t\x12\x13\n\x0bsearch_text\x18\x03 \x01(\t\x12\x32\n\x0emin_created_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13include_deactivated\x18\x06 \x01(\x08\x12\'\n\npagination\x18\x07 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x90\x01\n\x1b\x41lgorithmConfigListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x33\n\x11\x61lgorithm_configs\x18\x02 \x03(\x0b\x32\x18.oi.papi.AlgorithmConfig\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"+\n\x1c\x41lgorithmConfigDeleteRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"4\n\x1d\x41lgorithmConfigDeleteResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\".\n\x1f\x41lgorithmConfigDeprecateRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"7\n AlgorithmConfigDeprecateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"/\n AlgorithmConfigDeactivateRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"8\n!AlgorithmConfigDeactivateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r2\x89\x05\n\x12\x41lgorithmConfigApi\x12W\n\x06\x63reate\x12%.oi.papi.AlgorithmConfigCreateRequest\x1a&.oi.papi.AlgorithmConfigCreateResponse\x12N\n\x03get\x12\".oi.papi.AlgorithmConfigGetRequest\x1a#.oi.papi.AlgorithmConfigGetResponse\x12Q\n\x04list\x12#.oi.papi.AlgorithmConfigListRequest\x1a$.oi.papi.AlgorithmConfigListResponse\x12W\n\x06update\x12%.oi.papi.AlgorithmConfigUpdateRequest\x1a&.oi.papi.AlgorithmConfigUpdateResponse\x12`\n\tdeprecate\x12(.oi.papi.AlgorithmConfigDeprecateRequest\x1a).oi.papi.AlgorithmConfigDeprecateResponse\x12\x63\n\ndeactivate\x12).oi.papi.AlgorithmConfigDeactivateRequest\x1a*.oi.papi.AlgorithmConfigDeactivateResponse\x12W\n\x06\x64\x65lete\x12%.oi.papi.AlgorithmConfigDeleteRequest\x1a&.oi.papi.AlgorithmConfigDeleteResponseP\x01P\x03P\x04\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'algorithm_config_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_ALGORITHMCONFIG']._serialized_start=162
-  _globals['_ALGORITHMCONFIG']._serialized_end=481
-  _globals['_ALGORITHMCONFIGCREATEREQUEST']._serialized_start=484
-  _globals['_ALGORITHMCONFIGCREATEREQUEST']._serialized_end=620
-  _globals['_ALGORITHMCONFIGCREATERESPONSE']._serialized_start=622
-  _globals['_ALGORITHMCONFIGCREATERESPONSE']._serialized_end=726
-  _globals['_ALGORITHMCONFIGUPDATEREQUEST']._serialized_start=728
-  _globals['_ALGORITHMCONFIGUPDATEREQUEST']._serialized_end=821
-  _globals['_ALGORITHMCONFIGUPDATERESPONSE']._serialized_start=823
-  _globals['_ALGORITHMCONFIGUPDATERESPONSE']._serialized_end=875
-  _globals['_ALGORITHMCONFIGGETREQUEST']._serialized_start=878
-  _globals['_ALGORITHMCONFIGGETREQUEST']._serialized_end=1011
-  _globals['_ALGORITHMCONFIGGETRESPONSE']._serialized_start=1014
-  _globals['_ALGORITHMCONFIGGETRESPONSE']._serialized_end=1157
-  _globals['_ALGORITHMCONFIGLISTREQUEST']._serialized_start=1160
-  _globals['_ALGORITHMCONFIGLISTREQUEST']._serialized_end=1435
-  _globals['_ALGORITHMCONFIGLISTRESPONSE']._serialized_start=1438
-  _globals['_ALGORITHMCONFIGLISTRESPONSE']._serialized_end=1582
-  _globals['_ALGORITHMCONFIGDELETEREQUEST']._serialized_start=1584
-  _globals['_ALGORITHMCONFIGDELETEREQUEST']._serialized_end=1627
-  _globals['_ALGORITHMCONFIGDELETERESPONSE']._serialized_start=1629
-  _globals['_ALGORITHMCONFIGDELETERESPONSE']._serialized_end=1681
-  _globals['_ALGORITHMCONFIGDEPRECATEREQUEST']._serialized_start=1683
-  _globals['_ALGORITHMCONFIGDEPRECATEREQUEST']._serialized_end=1729
-  _globals['_ALGORITHMCONFIGDEPRECATERESPONSE']._serialized_start=1731
-  _globals['_ALGORITHMCONFIGDEPRECATERESPONSE']._serialized_end=1786
-  _globals['_ALGORITHMCONFIGDEACTIVATEREQUEST']._serialized_start=1788
-  _globals['_ALGORITHMCONFIGDEACTIVATEREQUEST']._serialized_end=1835
-  _globals['_ALGORITHMCONFIGDEACTIVATERESPONSE']._serialized_start=1837
-  _globals['_ALGORITHMCONFIGDEACTIVATERESPONSE']._serialized_end=1893
-  _globals['_ALGORITHMCONFIGAPI']._serialized_start=1896
-  _globals['_ALGORITHMCONFIGAPI']._serialized_end=2545
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'algorithm_config_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _ALGORITHMCONFIG._serialized_start=162
+  _ALGORITHMCONFIG._serialized_end=455
+  _ALGORITHMCONFIGCREATEREQUEST._serialized_start=458
+  _ALGORITHMCONFIGCREATEREQUEST._serialized_end=594
+  _ALGORITHMCONFIGCREATERESPONSE._serialized_start=596
+  _ALGORITHMCONFIGCREATERESPONSE._serialized_end=700
+  _ALGORITHMCONFIGUPDATEREQUEST._serialized_start=702
+  _ALGORITHMCONFIGUPDATEREQUEST._serialized_end=795
+  _ALGORITHMCONFIGUPDATERESPONSE._serialized_start=797
+  _ALGORITHMCONFIGUPDATERESPONSE._serialized_end=849
+  _ALGORITHMCONFIGGETREQUEST._serialized_start=852
+  _ALGORITHMCONFIGGETREQUEST._serialized_end=985
+  _ALGORITHMCONFIGGETRESPONSE._serialized_start=988
+  _ALGORITHMCONFIGGETRESPONSE._serialized_end=1131
+  _ALGORITHMCONFIGLISTREQUEST._serialized_start=1134
+  _ALGORITHMCONFIGLISTREQUEST._serialized_end=1409
+  _ALGORITHMCONFIGLISTRESPONSE._serialized_start=1412
+  _ALGORITHMCONFIGLISTRESPONSE._serialized_end=1556
+  _ALGORITHMCONFIGDELETEREQUEST._serialized_start=1558
+  _ALGORITHMCONFIGDELETEREQUEST._serialized_end=1601
+  _ALGORITHMCONFIGDELETERESPONSE._serialized_start=1603
+  _ALGORITHMCONFIGDELETERESPONSE._serialized_end=1655
+  _ALGORITHMCONFIGDEPRECATEREQUEST._serialized_start=1657
+  _ALGORITHMCONFIGDEPRECATEREQUEST._serialized_end=1703
+  _ALGORITHMCONFIGDEPRECATERESPONSE._serialized_start=1705
+  _ALGORITHMCONFIGDEPRECATERESPONSE._serialized_end=1760
+  _ALGORITHMCONFIGDEACTIVATEREQUEST._serialized_start=1762
+  _ALGORITHMCONFIGDEACTIVATEREQUEST._serialized_end=1809
+  _ALGORITHMCONFIGDEACTIVATERESPONSE._serialized_start=1811
+  _ALGORITHMCONFIGDEACTIVATERESPONSE._serialized_end=1867
+  _ALGORITHMCONFIGAPI._serialized_start=1870
+  _ALGORITHMCONFIGAPI._serialized_end=2519
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/algorithm_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/algorithm_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: algorithm.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
 
 from terrascope_api.models.common_models_pb2 import *
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0f\x61lgorithm.proto\x12\x07oi.papi\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\"{\n\tAlgorithm\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x03 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x04 \x01(\t\x12.\n\ncreated_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"L\n\x16\x41lgorithmCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x03 \x01(\t\"U\n\x17\x41lgorithmCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12%\n\talgorithm\x18\x02 \x01(\x0b\x32\x12.oi.papi.Algorithm\"K\n\x13\x41lgorithmGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\"|\n\x14\x41lgorithmGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12&\n\nalgorithms\x18\x02 \x03(\x0b\x32\x12.oi.papi.Algorithm\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\xbc\x01\n\x14\x41lgorithmListRequest\x12\x13\n\x0bsearch_text\x18\x01 \x01(\t\x12\x32\n\x0emin_created_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\npagination\x18\x04 \x01(\x0b\x32\x13.oi.papi.Pagination\"}\n\x15\x41lgorithmListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12&\n\nalgorithms\x18\x02 \x03(\x0b\x32\x12.oi.papi.Algorithm\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"@\n\x16\x41lgorithmUpdateRequest\x12&\n\nalgorithms\x18\x01 \x03(\x0b\x32\x12.oi.papi.Algorithm\".\n\x17\x41lgorithmUpdateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r2\xb3\x02\n\x0c\x41lgorithmApi\x12K\n\x06\x63reate\x12\x1f.oi.papi.AlgorithmCreateRequest\x1a .oi.papi.AlgorithmCreateResponse\x12K\n\x06update\x12\x1f.oi.papi.AlgorithmUpdateRequest\x1a .oi.papi.AlgorithmUpdateResponse\x12\x42\n\x03get\x12\x1c.oi.papi.AlgorithmGetRequest\x1a\x1d.oi.papi.AlgorithmGetResponse\x12\x45\n\x04list\x12\x1d.oi.papi.AlgorithmListRequest\x1a\x1e.oi.papi.AlgorithmListResponseP\x01\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'algorithm_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_ALGORITHM']._serialized_start=82
-  _globals['_ALGORITHM']._serialized_end=205
-  _globals['_ALGORITHMCREATEREQUEST']._serialized_start=207
-  _globals['_ALGORITHMCREATEREQUEST']._serialized_end=283
-  _globals['_ALGORITHMCREATERESPONSE']._serialized_start=285
-  _globals['_ALGORITHMCREATERESPONSE']._serialized_end=370
-  _globals['_ALGORITHMGETREQUEST']._serialized_start=372
-  _globals['_ALGORITHMGETREQUEST']._serialized_end=447
-  _globals['_ALGORITHMGETRESPONSE']._serialized_start=449
-  _globals['_ALGORITHMGETRESPONSE']._serialized_end=573
-  _globals['_ALGORITHMLISTREQUEST']._serialized_start=576
-  _globals['_ALGORITHMLISTREQUEST']._serialized_end=764
-  _globals['_ALGORITHMLISTRESPONSE']._serialized_start=766
-  _globals['_ALGORITHMLISTRESPONSE']._serialized_end=891
-  _globals['_ALGORITHMUPDATEREQUEST']._serialized_start=893
-  _globals['_ALGORITHMUPDATEREQUEST']._serialized_end=957
-  _globals['_ALGORITHMUPDATERESPONSE']._serialized_start=959
-  _globals['_ALGORITHMUPDATERESPONSE']._serialized_end=1005
-  _globals['_ALGORITHMAPI']._serialized_start=1008
-  _globals['_ALGORITHMAPI']._serialized_end=1315
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'algorithm_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _ALGORITHM._serialized_start=82
+  _ALGORITHM._serialized_end=205
+  _ALGORITHMCREATEREQUEST._serialized_start=207
+  _ALGORITHMCREATEREQUEST._serialized_end=283
+  _ALGORITHMCREATERESPONSE._serialized_start=285
+  _ALGORITHMCREATERESPONSE._serialized_end=370
+  _ALGORITHMGETREQUEST._serialized_start=372
+  _ALGORITHMGETREQUEST._serialized_end=447
+  _ALGORITHMGETRESPONSE._serialized_start=449
+  _ALGORITHMGETRESPONSE._serialized_end=573
+  _ALGORITHMLISTREQUEST._serialized_start=576
+  _ALGORITHMLISTREQUEST._serialized_end=764
+  _ALGORITHMLISTRESPONSE._serialized_start=766
+  _ALGORITHMLISTRESPONSE._serialized_end=891
+  _ALGORITHMUPDATEREQUEST._serialized_start=893
+  _ALGORITHMUPDATEREQUEST._serialized_end=957
+  _ALGORITHMUPDATERESPONSE._serialized_start=959
+  _ALGORITHMUPDATERESPONSE._serialized_end=1005
+  _ALGORITHMAPI._serialized_start=1008
+  _ALGORITHMAPI._serialized_end=1315
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/algorithm_version_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/algorithm_version_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: algorithm_version.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
@@ -20,59 +19,59 @@
   common__models__pb2 = algorithm__pb2.common__models__pb2
 except AttributeError:
   common__models__pb2 = algorithm__pb2.common_models_pb2
 
 from terrascope_api.models.common_models_pb2 import *
 from terrascope_api.models.algorithm_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17\x61lgorithm_version.proto\x12\x07oi.papi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\x1a\x0f\x61lgorithm.proto\"\x8e\x08\n\x08Manifest\x12,\n\x08metadata\x18\x01 \x01(\x0b\x32\x1a.oi.papi.Manifest.Metadata\x12\x31\n\x06inputs\x18\x02 \x03(\x0b\x32!.oi.papi.Manifest.AlgorithmInputs\x12\x33\n\x07outputs\x18\x03 \x03(\x0b\x32\".oi.papi.Manifest.AlgorithmOutputs\x12\x43\n\x14\x63ontainer_parameters\x18\x04 \x01(\x0b\x32%.oi.papi.Manifest.ContainerParameters\x12.\n\tinterface\x18\x05 \x01(\x0b\x32\x1b.oi.papi.Manifest.Interface\x12;\n\x10resource_request\x18\x06 \x01(\x0b\x32!.oi.papi.Manifest.ResourceRequest\x12/\n\nparameters\x18\x07 \x03(\x0b\x32\x1b.oi.papi.Manifest.Parameter\x12\x18\n\x10manifest_version\x18\x08 \x01(\t\x1a\x44\n\x08Metadata\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x0c\n\x04tags\x18\x02 \x03(\tJ\x04\x08\x01\x10\x02\x1a\x34\n\tInterface\x12\x16\n\x0einterface_type\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\x1aO\n\x0f\x41lgorithmInputs\x12\x16\n\x0e\x64\x61ta_type_name\x18\x01 \x01(\t\x12\x11\n\tmin_count\x18\x02 \x01(\r\x12\x11\n\tmax_count\x18\x03 \x01(\r\x1aS\n\x10\x41lgorithmOutputs\x12!\n\x19observation_value_columns\x18\x02 \x03(\t\x12\x16\n\x0e\x64\x61ta_type_name\x18\x03 \x01(\tJ\x04\x08\x01\x10\x02\x1ar\n\x13\x43ontainerParameters\x12\r\n\x05image\x18\x01 \x01(\t\x12;\n\x10resource_request\x18\x02 \x01(\x0b\x32!.oi.papi.Manifest.ResourceRequest\x12\x0f\n\x07\x63ommand\x18\x03 \x03(\t\x1aH\n\x0fResourceRequest\x12\x0b\n\x03gpu\x18\x01 \x01(\r\x12\x11\n\tmemory_gb\x18\x02 \x01(\r\x12\x15\n\rcpu_millicore\x18\x03 \x01(\r\x1a\x8e\x01\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\r\n\x05units\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0b\n\x03min\x18\x05 \x01(\r\x12\x0b\n\x03max\x18\x06 \x01(\r\x12\x16\n\x0e\x61llowed_values\x18\x07 \x03(\t\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x08 \x01(\r\"\xe0\x01\n\x10\x41lgorithmVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12%\n\talgorithm\x18\x02 \x01(\x0b\x32\x12.oi.papi.Algorithm\x12\x0f\n\x07version\x18\x03 \x01(\t\x12)\n\x08manifest\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12.\n\ncreated_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0eis_deactivated\x18\x06 \x01(\x08\x12\x15\n\ris_deprecated\x18\x07 \x01(\x08\"\xae\x01\n\x1d\x41lgorithmVersionCreateRequest\x12\x14\n\x0c\x61lgorithm_id\x18\x01 \x01(\t\x12\x32\n\x0fmanifest_struct\x18\x02 \x01(\x0b\x32\x17.google.protobuf.StructH\x00\x12-\n\x10manifest_message\x18\x03 \x01(\x0b\x32\x11.oi.papi.ManifestH\x00\x42\x14\n\x12\x61lgorithm_manifest\"k\n\x1e\x41lgorithmVersionCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x34\n\x11\x61lgorithm_version\x18\x02 \x01(\x0b\x32\x19.oi.papi.AlgorithmVersion\"R\n\x1a\x41lgorithmVersionGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x92\x01\n\x1b\x41lgorithmVersionGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x35\n\x12\x61lgorithm_versions\x18\x02 \x03(\x0b\x32\x19.oi.papi.AlgorithmVersion\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x84\x02\n\x1b\x41lgorithmVersionListRequest\x12\x14\n\x0c\x61lgorithm_id\x18\x01 \x01(\t\x12\x13\n\x0bsearch_text\x18\x02 \x01(\t\x12\x0b\n\x03tag\x18\x03 \x01(\t\x12\x32\n\x0emin_created_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14include_all_versions\x18\x06 \x01(\x08\x12\'\n\npagination\x18\x07 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x93\x01\n\x1c\x41lgorithmVersionListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x35\n\x12\x61lgorithm_versions\x18\x02 \x03(\x0b\x32\x19.oi.papi.AlgorithmVersion\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"/\n AlgorithmVersionDeprecateRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"8\n!AlgorithmVersionDeprecateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"0\n!AlgorithmVersionDeactivateRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"9\n\"AlgorithmVersionDeactivateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\".\n\x1f\x41lgorithmVersionActivateRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"7\n AlgorithmVersionActivateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r2\xc3\x04\n\x13\x41lgorithmVersionApi\x12Y\n\x06\x63reate\x12&.oi.papi.AlgorithmVersionCreateRequest\x1a\'.oi.papi.AlgorithmVersionCreateResponse\x12P\n\x03get\x12#.oi.papi.AlgorithmVersionGetRequest\x1a$.oi.papi.AlgorithmVersionGetResponse\x12S\n\x04list\x12$.oi.papi.AlgorithmVersionListRequest\x1a%.oi.papi.AlgorithmVersionListResponse\x12\x62\n\tdeprecate\x12).oi.papi.AlgorithmVersionDeprecateRequest\x1a*.oi.papi.AlgorithmVersionDeprecateResponse\x12\x65\n\ndeactivate\x12*.oi.papi.AlgorithmVersionDeactivateRequest\x1a+.oi.papi.AlgorithmVersionDeactivateResponse\x12_\n\x08\x61\x63tivate\x12(.oi.papi.AlgorithmVersionActivateRequest\x1a).oi.papi.AlgorithmVersionActivateResponseP\x02P\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17\x61lgorithm_version.proto\x12\x07oi.papi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\x1a\x0f\x61lgorithm.proto\"\x85\x08\n\x08Manifest\x12,\n\x08metadata\x18\x01 \x01(\x0b\x32\x1a.oi.papi.Manifest.Metadata\x12\x31\n\x06inputs\x18\x02 \x03(\x0b\x32!.oi.papi.Manifest.AlgorithmInputs\x12\x33\n\x07outputs\x18\x03 \x03(\x0b\x32\".oi.papi.Manifest.AlgorithmOutputs\x12\x43\n\x14\x63ontainer_parameters\x18\x04 \x01(\x0b\x32%.oi.papi.Manifest.ContainerParameters\x12.\n\tinterface\x18\x05 \x01(\x0b\x32\x1b.oi.papi.Manifest.Interface\x12;\n\x10resource_request\x18\x06 \x01(\x0b\x32!.oi.papi.Manifest.ResourceRequest\x12/\n\nparameters\x18\x07 \x03(\x0b\x32\x1b.oi.papi.Manifest.Parameter\x1aX\n\x08Metadata\x12\x18\n\x10manifest_version\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x0c\n\x04tags\x18\x02 \x03(\t\x1a\x34\n\tInterface\x12\x16\n\x0einterface_type\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\x1aO\n\x0f\x41lgorithmInputs\x12\x16\n\x0e\x64\x61ta_type_name\x18\x01 \x01(\t\x12\x11\n\tmin_count\x18\x02 \x01(\r\x12\x11\n\tmax_count\x18\x03 \x01(\r\x1aP\n\x10\x41lgorithmOutputs\x12\x19\n\x11output_data_types\x18\x01 \x03(\t\x12!\n\x19observation_value_columns\x18\x02 \x03(\t\x1ar\n\x13\x43ontainerParameters\x12\r\n\x05image\x18\x01 \x01(\t\x12;\n\x10resource_request\x18\x02 \x01(\x0b\x32!.oi.papi.Manifest.ResourceRequest\x12\x0f\n\x07\x63ommand\x18\x03 \x03(\t\x1aH\n\x0fResourceRequest\x12\x0b\n\x03gpu\x18\x01 \x01(\r\x12\x11\n\tmemory_gb\x18\x02 \x01(\r\x12\x15\n\rcpu_millicore\x18\x03 \x01(\r\x1a\x8e\x01\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\r\x12\r\n\x05units\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0b\n\x03min\x18\x05 \x01(\r\x12\x0b\n\x03max\x18\x06 \x01(\r\x12\x16\n\x0e\x61llowed_values\x18\x07 \x03(\t\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x08 \x01(\r\"\xe0\x01\n\x10\x41lgorithmVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12%\n\talgorithm\x18\x02 \x01(\x0b\x32\x12.oi.papi.Algorithm\x12\x0f\n\x07version\x18\x03 \x01(\t\x12)\n\x08manifest\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12.\n\ncreated_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0eis_deactivated\x18\x06 \x01(\x08\x12\x15\n\ris_deprecated\x18\x07 \x01(\x08\"\xae\x01\n\x1d\x41lgorithmVersionCreateRequest\x12\x14\n\x0c\x61lgorithm_id\x18\x01 \x01(\t\x12\x32\n\x0fmanifest_struct\x18\x02 \x01(\x0b\x32\x17.google.protobuf.StructH\x00\x12-\n\x10manifest_message\x18\x03 \x01(\x0b\x32\x11.oi.papi.ManifestH\x00\x42\x14\n\x12\x61lgorithm_manifest\"k\n\x1e\x41lgorithmVersionCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x34\n\x11\x61lgorithm_version\x18\x02 \x01(\x0b\x32\x19.oi.papi.AlgorithmVersion\"R\n\x1a\x41lgorithmVersionGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x92\x01\n\x1b\x41lgorithmVersionGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x35\n\x12\x61lgorithm_versions\x18\x02 \x03(\x0b\x32\x19.oi.papi.AlgorithmVersion\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x84\x02\n\x1b\x41lgorithmVersionListRequest\x12\x14\n\x0c\x61lgorithm_id\x18\x01 \x01(\t\x12\x13\n\x0bsearch_text\x18\x02 \x01(\t\x12\x0b\n\x03tag\x18\x03 \x01(\t\x12\x32\n\x0emin_created_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14include_all_versions\x18\x06 \x01(\x08\x12\'\n\npagination\x18\x07 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x93\x01\n\x1c\x41lgorithmVersionListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x35\n\x12\x61lgorithm_versions\x18\x02 \x03(\x0b\x32\x19.oi.papi.AlgorithmVersion\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"/\n AlgorithmVersionDeprecateRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"8\n!AlgorithmVersionDeprecateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"0\n!AlgorithmVersionDeactivateRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"9\n\"AlgorithmVersionDeactivateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\".\n\x1f\x41lgorithmVersionActivateRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"7\n AlgorithmVersionActivateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r2\xc3\x04\n\x13\x41lgorithmVersionApi\x12Y\n\x06\x63reate\x12&.oi.papi.AlgorithmVersionCreateRequest\x1a\'.oi.papi.AlgorithmVersionCreateResponse\x12P\n\x03get\x12#.oi.papi.AlgorithmVersionGetRequest\x1a$.oi.papi.AlgorithmVersionGetResponse\x12S\n\x04list\x12$.oi.papi.AlgorithmVersionListRequest\x1a%.oi.papi.AlgorithmVersionListResponse\x12\x62\n\tdeprecate\x12).oi.papi.AlgorithmVersionDeprecateRequest\x1a*.oi.papi.AlgorithmVersionDeprecateResponse\x12\x65\n\ndeactivate\x12*.oi.papi.AlgorithmVersionDeactivateRequest\x1a+.oi.papi.AlgorithmVersionDeactivateResponse\x12_\n\x08\x61\x63tivate\x12(.oi.papi.AlgorithmVersionActivateRequest\x1a).oi.papi.AlgorithmVersionActivateResponseP\x02P\x03\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'algorithm_version_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_MANIFEST']._serialized_start=138
-  _globals['_MANIFEST']._serialized_end=1176
-  _globals['_MANIFEST_METADATA']._serialized_start=553
-  _globals['_MANIFEST_METADATA']._serialized_end=621
-  _globals['_MANIFEST_INTERFACE']._serialized_start=623
-  _globals['_MANIFEST_INTERFACE']._serialized_end=675
-  _globals['_MANIFEST_ALGORITHMINPUTS']._serialized_start=677
-  _globals['_MANIFEST_ALGORITHMINPUTS']._serialized_end=756
-  _globals['_MANIFEST_ALGORITHMOUTPUTS']._serialized_start=758
-  _globals['_MANIFEST_ALGORITHMOUTPUTS']._serialized_end=841
-  _globals['_MANIFEST_CONTAINERPARAMETERS']._serialized_start=843
-  _globals['_MANIFEST_CONTAINERPARAMETERS']._serialized_end=957
-  _globals['_MANIFEST_RESOURCEREQUEST']._serialized_start=959
-  _globals['_MANIFEST_RESOURCEREQUEST']._serialized_end=1031
-  _globals['_MANIFEST_PARAMETER']._serialized_start=1034
-  _globals['_MANIFEST_PARAMETER']._serialized_end=1176
-  _globals['_ALGORITHMVERSION']._serialized_start=1179
-  _globals['_ALGORITHMVERSION']._serialized_end=1403
-  _globals['_ALGORITHMVERSIONCREATEREQUEST']._serialized_start=1406
-  _globals['_ALGORITHMVERSIONCREATEREQUEST']._serialized_end=1580
-  _globals['_ALGORITHMVERSIONCREATERESPONSE']._serialized_start=1582
-  _globals['_ALGORITHMVERSIONCREATERESPONSE']._serialized_end=1689
-  _globals['_ALGORITHMVERSIONGETREQUEST']._serialized_start=1691
-  _globals['_ALGORITHMVERSIONGETREQUEST']._serialized_end=1773
-  _globals['_ALGORITHMVERSIONGETRESPONSE']._serialized_start=1776
-  _globals['_ALGORITHMVERSIONGETRESPONSE']._serialized_end=1922
-  _globals['_ALGORITHMVERSIONLISTREQUEST']._serialized_start=1925
-  _globals['_ALGORITHMVERSIONLISTREQUEST']._serialized_end=2185
-  _globals['_ALGORITHMVERSIONLISTRESPONSE']._serialized_start=2188
-  _globals['_ALGORITHMVERSIONLISTRESPONSE']._serialized_end=2335
-  _globals['_ALGORITHMVERSIONDEPRECATEREQUEST']._serialized_start=2337
-  _globals['_ALGORITHMVERSIONDEPRECATEREQUEST']._serialized_end=2384
-  _globals['_ALGORITHMVERSIONDEPRECATERESPONSE']._serialized_start=2386
-  _globals['_ALGORITHMVERSIONDEPRECATERESPONSE']._serialized_end=2442
-  _globals['_ALGORITHMVERSIONDEACTIVATEREQUEST']._serialized_start=2444
-  _globals['_ALGORITHMVERSIONDEACTIVATEREQUEST']._serialized_end=2492
-  _globals['_ALGORITHMVERSIONDEACTIVATERESPONSE']._serialized_start=2494
-  _globals['_ALGORITHMVERSIONDEACTIVATERESPONSE']._serialized_end=2551
-  _globals['_ALGORITHMVERSIONACTIVATEREQUEST']._serialized_start=2553
-  _globals['_ALGORITHMVERSIONACTIVATEREQUEST']._serialized_end=2599
-  _globals['_ALGORITHMVERSIONACTIVATERESPONSE']._serialized_start=2601
-  _globals['_ALGORITHMVERSIONACTIVATERESPONSE']._serialized_end=2656
-  _globals['_ALGORITHMVERSIONAPI']._serialized_start=2659
-  _globals['_ALGORITHMVERSIONAPI']._serialized_end=3238
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'algorithm_version_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _MANIFEST._serialized_start=138
+  _MANIFEST._serialized_end=1167
+  _MANIFEST_METADATA._serialized_start=527
+  _MANIFEST_METADATA._serialized_end=615
+  _MANIFEST_INTERFACE._serialized_start=617
+  _MANIFEST_INTERFACE._serialized_end=669
+  _MANIFEST_ALGORITHMINPUTS._serialized_start=671
+  _MANIFEST_ALGORITHMINPUTS._serialized_end=750
+  _MANIFEST_ALGORITHMOUTPUTS._serialized_start=752
+  _MANIFEST_ALGORITHMOUTPUTS._serialized_end=832
+  _MANIFEST_CONTAINERPARAMETERS._serialized_start=834
+  _MANIFEST_CONTAINERPARAMETERS._serialized_end=948
+  _MANIFEST_RESOURCEREQUEST._serialized_start=950
+  _MANIFEST_RESOURCEREQUEST._serialized_end=1022
+  _MANIFEST_PARAMETER._serialized_start=1025
+  _MANIFEST_PARAMETER._serialized_end=1167
+  _ALGORITHMVERSION._serialized_start=1170
+  _ALGORITHMVERSION._serialized_end=1394
+  _ALGORITHMVERSIONCREATEREQUEST._serialized_start=1397
+  _ALGORITHMVERSIONCREATEREQUEST._serialized_end=1571
+  _ALGORITHMVERSIONCREATERESPONSE._serialized_start=1573
+  _ALGORITHMVERSIONCREATERESPONSE._serialized_end=1680
+  _ALGORITHMVERSIONGETREQUEST._serialized_start=1682
+  _ALGORITHMVERSIONGETREQUEST._serialized_end=1764
+  _ALGORITHMVERSIONGETRESPONSE._serialized_start=1767
+  _ALGORITHMVERSIONGETRESPONSE._serialized_end=1913
+  _ALGORITHMVERSIONLISTREQUEST._serialized_start=1916
+  _ALGORITHMVERSIONLISTREQUEST._serialized_end=2176
+  _ALGORITHMVERSIONLISTRESPONSE._serialized_start=2179
+  _ALGORITHMVERSIONLISTRESPONSE._serialized_end=2326
+  _ALGORITHMVERSIONDEPRECATEREQUEST._serialized_start=2328
+  _ALGORITHMVERSIONDEPRECATEREQUEST._serialized_end=2375
+  _ALGORITHMVERSIONDEPRECATERESPONSE._serialized_start=2377
+  _ALGORITHMVERSIONDEPRECATERESPONSE._serialized_end=2433
+  _ALGORITHMVERSIONDEACTIVATEREQUEST._serialized_start=2435
+  _ALGORITHMVERSIONDEACTIVATEREQUEST._serialized_end=2483
+  _ALGORITHMVERSIONDEACTIVATERESPONSE._serialized_start=2485
+  _ALGORITHMVERSIONDEACTIVATERESPONSE._serialized_end=2542
+  _ALGORITHMVERSIONACTIVATEREQUEST._serialized_start=2544
+  _ALGORITHMVERSIONACTIVATEREQUEST._serialized_end=2590
+  _ALGORITHMVERSIONACTIVATERESPONSE._serialized_start=2592
+  _ALGORITHMVERSIONACTIVATERESPONSE._serialized_end=2647
+  _ALGORITHMVERSIONAPI._serialized_start=2650
+  _ALGORITHMVERSIONAPI._serialized_end=3229
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/analysis_computation_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/analysis_computation_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: analysis_computation.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
@@ -19,41 +18,39 @@
   common__models__pb2 = analysis__pb2.common__models__pb2
 except AttributeError:
   common__models__pb2 = analysis__pb2.common_models_pb2
 
 from terrascope_api.models.common_models_pb2 import *
 from terrascope_api.models.analysis_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x61nalysis_computation.proto\x12\x07oi.papi\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\x1a\x0e\x61nalysis.proto\"i\n AnalysisComputationCreateRequest\x12\x1a\n\x12\x61nalysis_config_id\x18\x01 \x01(\t\x12\x0e\n\x06toi_id\x18\x02 \x01(\t\x12\x19\n\x11\x61oi_collection_id\x18\x03 \x01(\t\"t\n!AnalysisComputationCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12:\n\x14\x61nalysis_computation\x18\x02 \x01(\x0b\x32\x1c.oi.papi.AnalysisComputation\",\n\x1d\x41nalysisComputationRunRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"5\n\x1e\x41nalysisComputationRunResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"U\n\x1d\x41nalysisComputationGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\"f\n\x17\x41nalysisComputationNode\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0e\x63omputation_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hildren\x18\x03 \x03(\t\x12\x13\n\x0bhas_results\x18\x04 \x01(\x08\"\xf0\x03\n\x13\x41nalysisComputation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61nalysis_id\x18\x02 \x01(\t\x12\x0e\n\x06toi_id\x18\x03 \x01(\t\x12\x19\n\x11\x61oi_collection_id\x18\x04 \x01(\t\x12\x1a\n\x12\x61nalysis_config_id\x18\x05 \x01(\t\x12\x30\n\x0csubmitted_on\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\x05state\x18\x07 \x01(\x0e\x32\".oi.papi.AnalysisComputation.State\x12;\n\x11\x63omputation_nodes\x18\x08 \x03(\x0b\x32 .oi.papi.AnalysisComputationNode\x12\x37\n\x08progress\x18\t \x01(\x0b\x32%.oi.papi.AnalysisComputation.Progress\x1a>\n\x08Progress\x12\x0f\n\x07running\x18\x01 \x01(\x01\x12\x11\n\tsucceeded\x18\x02 \x01(\x01\x12\x0e\n\x06\x66\x61iled\x18\x03 \x01(\x01\"V\n\x05State\x12\x11\n\rUNKNOWN_STATE\x10\x00\x12\x0f\n\x0bNOT_STARTED\x10\x01\x12\x0f\n\x0bIN_PROGRESS\x10\x02\x12\n\n\x06PAUSED\x10\x03\x12\x0c\n\x08\x43OMPLETE\x10\x04\"\x9b\x01\n\x1e\x41nalysisComputationGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12;\n\x15\x61nalysis_computations\x18\x02 \x03(\x0b\x32\x1c.oi.papi.AnalysisComputation\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\xb0\x02\n\x1e\x41nalysisComputationListRequest\x12\r\n\x05state\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x34\n\x10min_submitted_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10max_submitted_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12\x61nalysis_config_id\x18\x05 \x01(\t\x12\x0e\n\x06toi_id\x18\x06 \x01(\t\x12\x19\n\x11\x61oi_collection_id\x18\x07 \x01(\t\x12\x13\n\x0b\x61nalysis_id\x18\x08 \x01(\t\x12\'\n\npagination\x18\t \x01(\x0b\x32\x13.oi.papi.Pagination\"\x9c\x01\n\x1f\x41nalysisComputationListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12;\n\x15\x61nalysis_computations\x18\x02 \x03(\x0b\x32\x1c.oi.papi.AnalysisComputation\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination2\x84\x03\n\x16\x41nalysisComputationApi\x12_\n\x06\x63reate\x12).oi.papi.AnalysisComputationCreateRequest\x1a*.oi.papi.AnalysisComputationCreateResponse\x12V\n\x03run\x12&.oi.papi.AnalysisComputationRunRequest\x1a\'.oi.papi.AnalysisComputationRunResponse\x12V\n\x03get\x12&.oi.papi.AnalysisComputationGetRequest\x1a\'.oi.papi.AnalysisComputationGetResponse\x12Y\n\x04list\x12\'.oi.papi.AnalysisComputationListRequest\x1a(.oi.papi.AnalysisComputationListResponseP\x01P\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x61nalysis_computation.proto\x12\x07oi.papi\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\x1a\x0e\x61nalysis.proto\"i\n AnalysisComputationCreateRequest\x12\x1a\n\x12\x61nalysis_config_id\x18\x01 \x01(\t\x12\x0e\n\x06toi_id\x18\x02 \x01(\t\x12\x19\n\x11\x61oi_collection_id\x18\x03 \x01(\t\"t\n!AnalysisComputationCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12:\n\x14\x61nalysis_computation\x18\x02 \x01(\x0b\x32\x1c.oi.papi.AnalysisComputation\",\n\x1d\x41nalysisComputationRunRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"5\n\x1e\x41nalysisComputationRunResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"U\n\x1d\x41nalysisComputationGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\"f\n\x17\x41nalysisComputationNode\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0e\x63omputation_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hildren\x18\x03 \x03(\t\x12\x13\n\x0bhas_results\x18\x04 \x01(\x08\"\xf7\x02\n\x13\x41nalysisComputation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61nalysis_id\x18\x02 \x01(\t\x12\x0e\n\x06toi_id\x18\x03 \x01(\t\x12\x19\n\x11\x61oi_collection_id\x18\x04 \x01(\t\x12\x1a\n\x12\x61nalysis_config_id\x18\x05 \x01(\t\x12\x30\n\x0csubmitted_on\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\x05state\x18\x07 \x01(\x0e\x32\".oi.papi.AnalysisComputation.State\x12;\n\x11\x63omputation_nodes\x18\x08 \x03(\x0b\x32 .oi.papi.AnalysisComputationNode\"V\n\x05State\x12\x11\n\rUNKNOWN_STATE\x10\x00\x12\x0f\n\x0bNOT_STARTED\x10\x01\x12\x0f\n\x0bIN_PROGRESS\x10\x02\x12\n\n\x06PAUSED\x10\x03\x12\x0c\n\x08\x43OMPLETE\x10\x04\"\x9b\x01\n\x1e\x41nalysisComputationGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12;\n\x15\x61nalysis_computations\x18\x02 \x03(\x0b\x32\x1c.oi.papi.AnalysisComputation\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\xb0\x02\n\x1e\x41nalysisComputationListRequest\x12\r\n\x05state\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x34\n\x10min_submitted_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10max_submitted_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12\x61nalysis_config_id\x18\x05 \x01(\t\x12\x0e\n\x06toi_id\x18\x06 \x01(\t\x12\x19\n\x11\x61oi_collection_id\x18\x07 \x01(\t\x12\x13\n\x0b\x61nalysis_id\x18\x08 \x01(\t\x12\'\n\npagination\x18\t \x01(\x0b\x32\x13.oi.papi.Pagination\"\x9c\x01\n\x1f\x41nalysisComputationListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12;\n\x15\x61nalysis_computations\x18\x02 \x03(\x0b\x32\x1c.oi.papi.AnalysisComputation\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination2\x84\x03\n\x16\x41nalysisComputationApi\x12_\n\x06\x63reate\x12).oi.papi.AnalysisComputationCreateRequest\x1a*.oi.papi.AnalysisComputationCreateResponse\x12V\n\x03run\x12&.oi.papi.AnalysisComputationRunRequest\x1a\'.oi.papi.AnalysisComputationRunResponse\x12V\n\x03get\x12&.oi.papi.AnalysisComputationGetRequest\x1a\'.oi.papi.AnalysisComputationGetResponse\x12Y\n\x04list\x12\'.oi.papi.AnalysisComputationListRequest\x1a(.oi.papi.AnalysisComputationListResponseP\x01P\x02\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'analysis_computation_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_ANALYSISCOMPUTATIONCREATEREQUEST']._serialized_start=109
-  _globals['_ANALYSISCOMPUTATIONCREATEREQUEST']._serialized_end=214
-  _globals['_ANALYSISCOMPUTATIONCREATERESPONSE']._serialized_start=216
-  _globals['_ANALYSISCOMPUTATIONCREATERESPONSE']._serialized_end=332
-  _globals['_ANALYSISCOMPUTATIONRUNREQUEST']._serialized_start=334
-  _globals['_ANALYSISCOMPUTATIONRUNREQUEST']._serialized_end=378
-  _globals['_ANALYSISCOMPUTATIONRUNRESPONSE']._serialized_start=380
-  _globals['_ANALYSISCOMPUTATIONRUNRESPONSE']._serialized_end=433
-  _globals['_ANALYSISCOMPUTATIONGETREQUEST']._serialized_start=435
-  _globals['_ANALYSISCOMPUTATIONGETREQUEST']._serialized_end=520
-  _globals['_ANALYSISCOMPUTATIONNODE']._serialized_start=522
-  _globals['_ANALYSISCOMPUTATIONNODE']._serialized_end=624
-  _globals['_ANALYSISCOMPUTATION']._serialized_start=627
-  _globals['_ANALYSISCOMPUTATION']._serialized_end=1123
-  _globals['_ANALYSISCOMPUTATION_PROGRESS']._serialized_start=973
-  _globals['_ANALYSISCOMPUTATION_PROGRESS']._serialized_end=1035
-  _globals['_ANALYSISCOMPUTATION_STATE']._serialized_start=1037
-  _globals['_ANALYSISCOMPUTATION_STATE']._serialized_end=1123
-  _globals['_ANALYSISCOMPUTATIONGETRESPONSE']._serialized_start=1126
-  _globals['_ANALYSISCOMPUTATIONGETRESPONSE']._serialized_end=1281
-  _globals['_ANALYSISCOMPUTATIONLISTREQUEST']._serialized_start=1284
-  _globals['_ANALYSISCOMPUTATIONLISTREQUEST']._serialized_end=1588
-  _globals['_ANALYSISCOMPUTATIONLISTRESPONSE']._serialized_start=1591
-  _globals['_ANALYSISCOMPUTATIONLISTRESPONSE']._serialized_end=1747
-  _globals['_ANALYSISCOMPUTATIONAPI']._serialized_start=1750
-  _globals['_ANALYSISCOMPUTATIONAPI']._serialized_end=2138
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'analysis_computation_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _ANALYSISCOMPUTATIONCREATEREQUEST._serialized_start=109
+  _ANALYSISCOMPUTATIONCREATEREQUEST._serialized_end=214
+  _ANALYSISCOMPUTATIONCREATERESPONSE._serialized_start=216
+  _ANALYSISCOMPUTATIONCREATERESPONSE._serialized_end=332
+  _ANALYSISCOMPUTATIONRUNREQUEST._serialized_start=334
+  _ANALYSISCOMPUTATIONRUNREQUEST._serialized_end=378
+  _ANALYSISCOMPUTATIONRUNRESPONSE._serialized_start=380
+  _ANALYSISCOMPUTATIONRUNRESPONSE._serialized_end=433
+  _ANALYSISCOMPUTATIONGETREQUEST._serialized_start=435
+  _ANALYSISCOMPUTATIONGETREQUEST._serialized_end=520
+  _ANALYSISCOMPUTATIONNODE._serialized_start=522
+  _ANALYSISCOMPUTATIONNODE._serialized_end=624
+  _ANALYSISCOMPUTATION._serialized_start=627
+  _ANALYSISCOMPUTATION._serialized_end=1002
+  _ANALYSISCOMPUTATION_STATE._serialized_start=916
+  _ANALYSISCOMPUTATION_STATE._serialized_end=1002
+  _ANALYSISCOMPUTATIONGETRESPONSE._serialized_start=1005
+  _ANALYSISCOMPUTATIONGETRESPONSE._serialized_end=1160
+  _ANALYSISCOMPUTATIONLISTREQUEST._serialized_start=1163
+  _ANALYSISCOMPUTATIONLISTREQUEST._serialized_end=1467
+  _ANALYSISCOMPUTATIONLISTRESPONSE._serialized_start=1470
+  _ANALYSISCOMPUTATIONLISTRESPONSE._serialized_end=1626
+  _ANALYSISCOMPUTATIONAPI._serialized_start=1629
+  _ANALYSISCOMPUTATIONAPI._serialized_end=2017
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/analysis_config_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/analysis_config_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: analysis_config.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
@@ -79,39 +78,31 @@
   common__models__pb2 = algorithm__config__pb2.common_models_pb2
 
 from terrascope_api.models.common_models_pb2 import *
 from terrascope_api.models.analysis_pb2 import *
 from terrascope_api.models.analysis_version_pb2 import *
 from terrascope_api.models.algorithm_config_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61nalysis_config.proto\x12\x07oi.papi\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\x1a\x0e\x61nalysis.proto\x1a\x16\x61nalysis_version.proto\x1a\x16\x61lgorithm_config.proto\"\x8c\x03\n\x0e\x41nalysisConfig\x12#\n\x08\x61nalysis\x18\x01 \x01(\x0b\x32\x11.oi.papi.Analysis\x12\x32\n\x10\x61nalysis_version\x18\x02 \x01(\x0b\x32\x18.oi.papi.AnalysisVersion\x12\n\n\x02id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12.\n\ncreated_on\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x44\n\x16\x61lgorithm_config_nodes\x18\x07 \x03(\x0b\x32$.oi.papi.AnalysisAlgorithmConfigNode\x12\x33\n\x11\x61lgorithm_configs\x18\x08 \x03(\x0b\x32\x18.oi.papi.AlgorithmConfig\x12\x15\n\ris_deprecated\x18\t \x01(\x08\x12\x16\n\x0eis_deactivated\x18\n \x01(\x08\x12\x18\n\x10resources_locked\x18\x0b \x01(\x08\"\xa3\x01\n\x1b\x41nalysisConfigCreateRequest\x12\x1b\n\x13\x61nalysis_version_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x44\n\x16\x61lgorithm_config_nodes\x18\x04 \x03(\x0b\x32$.oi.papi.AnalysisAlgorithmConfigNode\"e\n\x1c\x41nalysisConfigCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x30\n\x0f\x61nalysis_config\x18\x02 \x01(\x0b\x32\x17.oi.papi.AnalysisConfig\"\x92\x01\n\x1b\x41nalysisConfigUpdateRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x44\n\x16\x61lgorithm_config_nodes\x18\x04 \x03(\x0b\x32$.oi.papi.AnalysisAlgorithmConfigNode\"3\n\x1c\x41nalysisConfigUpdateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"s\n\x18\x41nalysisConfigGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12!\n\x19include_algorithm_details\x18\x02 \x01(\x08\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x8c\x01\n\x19\x41nalysisConfigGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x31\n\x10\x61nalysis_configs\x18\x02 \x03(\x0b\x32\x17.oi.papi.AnalysisConfig\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\xa4\x02\n\x19\x41nalysisConfigListRequest\x12\x13\n\x0b\x61nalysis_id\x18\x01 \x01(\t\x12\x1b\n\x13\x61nalysis_version_id\x18\x02 \x01(\t\x12\x13\n\x0bsearch_text\x18\x03 \x01(\t\x12\x32\n\x0emin_created_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13include_deactivated\x18\x06 \x01(\x08\x12\x12\n\nsubject_id\x18\x07 \x01(\t\x12\'\n\npagination\x18\x08 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x8d\x01\n\x1a\x41nalysisConfigListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x31\n\x10\x61nalysis_configs\x18\x02 \x03(\x0b\x32\x17.oi.papi.AnalysisConfig\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\".\n\x1f\x41nalysisConfigDeactivateRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"7\n AnalysisConfigDeactivateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r2\xc3\x03\n\x11\x41nalysisConfigApi\x12U\n\x06\x63reate\x12$.oi.papi.AnalysisConfigCreateRequest\x1a%.oi.papi.AnalysisConfigCreateResponse\x12U\n\x06update\x12$.oi.papi.AnalysisConfigUpdateRequest\x1a%.oi.papi.AnalysisConfigUpdateResponse\x12L\n\x03get\x12!.oi.papi.AnalysisConfigGetRequest\x1a\".oi.papi.AnalysisConfigGetResponse\x12O\n\x04list\x12\".oi.papi.AnalysisConfigListRequest\x1a#.oi.papi.AnalysisConfigListResponse\x12\x61\n\ndeactivate\x12(.oi.papi.AnalysisConfigDeactivateRequest\x1a).oi.papi.AnalysisConfigDeactivateResponseP\x01P\x02P\x03P\x04\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61nalysis_config.proto\x12\x07oi.papi\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\x1a\x0e\x61nalysis.proto\x1a\x16\x61nalysis_version.proto\x1a\x16\x61lgorithm_config.proto\"\xa3\x01\n\x1b\x41nalysisConfigCreateRequest\x12\x1b\n\x13\x61nalysis_version_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x44\n\x16\x61lgorithm_config_nodes\x18\x04 \x03(\x0b\x32$.oi.papi.AnalysisAlgorithmConfigNode\"\xf2\x02\n\x0e\x41nalysisConfig\x12#\n\x08\x61nalysis\x18\x01 \x01(\x0b\x32\x11.oi.papi.Analysis\x12\x32\n\x10\x61nalysis_version\x18\x02 \x01(\x0b\x32\x18.oi.papi.AnalysisVersion\x12\n\n\x02id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12.\n\ncreated_on\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x44\n\x16\x61lgorithm_config_nodes\x18\x07 \x03(\x0b\x32$.oi.papi.AnalysisAlgorithmConfigNode\x12\x33\n\x11\x61lgorithm_configs\x18\x08 \x03(\x0b\x32\x18.oi.papi.AlgorithmConfig\x12\x15\n\ris_deprecated\x18\t \x01(\x08\x12\x16\n\x0eis_deactivated\x18\n \x01(\x08\"e\n\x1c\x41nalysisConfigCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x30\n\x0f\x61nalysis_config\x18\x02 \x01(\x0b\x32\x17.oi.papi.AnalysisConfig\"s\n\x18\x41nalysisConfigGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12!\n\x19include_algorithm_details\x18\x02 \x01(\x08\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x8c\x01\n\x19\x41nalysisConfigGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x31\n\x10\x61nalysis_configs\x18\x02 \x03(\x0b\x32\x17.oi.papi.AnalysisConfig\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\xa4\x02\n\x19\x41nalysisConfigListRequest\x12\x13\n\x0b\x61nalysis_id\x18\x01 \x01(\t\x12\x1b\n\x13\x61nalysis_version_id\x18\x02 \x01(\t\x12\x13\n\x0bsearch_text\x18\x03 \x01(\t\x12\x32\n\x0emin_created_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13include_deactivated\x18\x06 \x01(\x08\x12\x12\n\nsubject_id\x18\x07 \x01(\t\x12\'\n\npagination\x18\x08 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x8d\x01\n\x1a\x41nalysisConfigListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x31\n\x10\x61nalysis_configs\x18\x02 \x03(\x0b\x32\x17.oi.papi.AnalysisConfig\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination2\x89\x02\n\x11\x41nalysisConfigApi\x12U\n\x06\x63reate\x12$.oi.papi.AnalysisConfigCreateRequest\x1a%.oi.papi.AnalysisConfigCreateResponse\x12L\n\x03get\x12!.oi.papi.AnalysisConfigGetRequest\x1a\".oi.papi.AnalysisConfigGetResponse\x12O\n\x04list\x12\".oi.papi.AnalysisConfigListRequest\x1a#.oi.papi.AnalysisConfigListResponseP\x01P\x02P\x03P\x04\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'analysis_config_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_ANALYSISCONFIG']._serialized_start=153
-  _globals['_ANALYSISCONFIG']._serialized_end=549
-  _globals['_ANALYSISCONFIGCREATEREQUEST']._serialized_start=552
-  _globals['_ANALYSISCONFIGCREATEREQUEST']._serialized_end=715
-  _globals['_ANALYSISCONFIGCREATERESPONSE']._serialized_start=717
-  _globals['_ANALYSISCONFIGCREATERESPONSE']._serialized_end=818
-  _globals['_ANALYSISCONFIGUPDATEREQUEST']._serialized_start=821
-  _globals['_ANALYSISCONFIGUPDATEREQUEST']._serialized_end=967
-  _globals['_ANALYSISCONFIGUPDATERESPONSE']._serialized_start=969
-  _globals['_ANALYSISCONFIGUPDATERESPONSE']._serialized_end=1020
-  _globals['_ANALYSISCONFIGGETREQUEST']._serialized_start=1022
-  _globals['_ANALYSISCONFIGGETREQUEST']._serialized_end=1137
-  _globals['_ANALYSISCONFIGGETRESPONSE']._serialized_start=1140
-  _globals['_ANALYSISCONFIGGETRESPONSE']._serialized_end=1280
-  _globals['_ANALYSISCONFIGLISTREQUEST']._serialized_start=1283
-  _globals['_ANALYSISCONFIGLISTREQUEST']._serialized_end=1575
-  _globals['_ANALYSISCONFIGLISTRESPONSE']._serialized_start=1578
-  _globals['_ANALYSISCONFIGLISTRESPONSE']._serialized_end=1719
-  _globals['_ANALYSISCONFIGDEACTIVATEREQUEST']._serialized_start=1721
-  _globals['_ANALYSISCONFIGDEACTIVATEREQUEST']._serialized_end=1767
-  _globals['_ANALYSISCONFIGDEACTIVATERESPONSE']._serialized_start=1769
-  _globals['_ANALYSISCONFIGDEACTIVATERESPONSE']._serialized_end=1824
-  _globals['_ANALYSISCONFIGAPI']._serialized_start=1827
-  _globals['_ANALYSISCONFIGAPI']._serialized_end=2278
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'analysis_config_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _ANALYSISCONFIGCREATEREQUEST._serialized_start=153
+  _ANALYSISCONFIGCREATEREQUEST._serialized_end=316
+  _ANALYSISCONFIG._serialized_start=319
+  _ANALYSISCONFIG._serialized_end=689
+  _ANALYSISCONFIGCREATERESPONSE._serialized_start=691
+  _ANALYSISCONFIGCREATERESPONSE._serialized_end=792
+  _ANALYSISCONFIGGETREQUEST._serialized_start=794
+  _ANALYSISCONFIGGETREQUEST._serialized_end=909
+  _ANALYSISCONFIGGETRESPONSE._serialized_start=912
+  _ANALYSISCONFIGGETRESPONSE._serialized_end=1052
+  _ANALYSISCONFIGLISTREQUEST._serialized_start=1055
+  _ANALYSISCONFIGLISTREQUEST._serialized_end=1347
+  _ANALYSISCONFIGLISTRESPONSE._serialized_start=1350
+  _ANALYSISCONFIGLISTRESPONSE._serialized_end=1491
+  _ANALYSISCONFIGAPI._serialized_start=1494
+  _ANALYSISCONFIGAPI._serialized_end=1759
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/analysis_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/analysis_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: analysis.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
 
 from terrascope_api.models.common_models_pb2 import *
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x61nalysis.proto\x12\x07oi.papi\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\"U\n\x15\x41nalysisAlgorithmNode\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1c\n\x14\x61lgorithm_version_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hildren\x18\x03 \x03(\t\"5\n\x15\x41nalysisCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x02 \x01(\t\"R\n\x16\x41nalysisCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12#\n\x08\x61nalysis\x18\x02 \x01(\x0b\x32\x11.oi.papi.Analysis\"H\n\x1b\x41nalysisAlgorithmConfigNode\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x13\x61lgorithm_config_id\x18\x02 \x01(\t\"J\n\x12\x41nalysisGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\"d\n\x08\x41nalysis\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x02 \x01(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04name\x18\x04 \x01(\t\"x\n\x13\x41nalysisGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12#\n\x08\x61nalyses\x18\x02 \x03(\x0b\x32\x11.oi.papi.Analysis\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\xbb\x01\n\x13\x41nalysisListRequest\x12\x13\n\x0bsearch_text\x18\x01 \x01(\t\x12\x32\n\x0emin_created_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\npagination\x18\x04 \x01(\x0b\x32\x13.oi.papi.Pagination\"y\n\x14\x41nalysisListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12#\n\x08\x61nalyses\x18\x02 \x03(\x0b\x32\x11.oi.papi.Analysis\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination2\xdf\x01\n\x0b\x41nalysisApi\x12I\n\x06\x63reate\x12\x1e.oi.papi.AnalysisCreateRequest\x1a\x1f.oi.papi.AnalysisCreateResponse\x12@\n\x03get\x12\x1b.oi.papi.AnalysisGetRequest\x1a\x1c.oi.papi.AnalysisGetResponse\x12\x43\n\x04list\x12\x1c.oi.papi.AnalysisListRequest\x1a\x1d.oi.papi.AnalysisListResponseP\x01\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'analysis_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_ANALYSISALGORITHMNODE']._serialized_start=81
-  _globals['_ANALYSISALGORITHMNODE']._serialized_end=166
-  _globals['_ANALYSISCREATEREQUEST']._serialized_start=168
-  _globals['_ANALYSISCREATEREQUEST']._serialized_end=221
-  _globals['_ANALYSISCREATERESPONSE']._serialized_start=223
-  _globals['_ANALYSISCREATERESPONSE']._serialized_end=305
-  _globals['_ANALYSISALGORITHMCONFIGNODE']._serialized_start=307
-  _globals['_ANALYSISALGORITHMCONFIGNODE']._serialized_end=379
-  _globals['_ANALYSISGETREQUEST']._serialized_start=381
-  _globals['_ANALYSISGETREQUEST']._serialized_end=455
-  _globals['_ANALYSIS']._serialized_start=457
-  _globals['_ANALYSIS']._serialized_end=557
-  _globals['_ANALYSISGETRESPONSE']._serialized_start=559
-  _globals['_ANALYSISGETRESPONSE']._serialized_end=679
-  _globals['_ANALYSISLISTREQUEST']._serialized_start=682
-  _globals['_ANALYSISLISTREQUEST']._serialized_end=869
-  _globals['_ANALYSISLISTRESPONSE']._serialized_start=871
-  _globals['_ANALYSISLISTRESPONSE']._serialized_end=992
-  _globals['_ANALYSISAPI']._serialized_start=995
-  _globals['_ANALYSISAPI']._serialized_end=1218
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'analysis_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _ANALYSISALGORITHMNODE._serialized_start=81
+  _ANALYSISALGORITHMNODE._serialized_end=166
+  _ANALYSISCREATEREQUEST._serialized_start=168
+  _ANALYSISCREATEREQUEST._serialized_end=221
+  _ANALYSISCREATERESPONSE._serialized_start=223
+  _ANALYSISCREATERESPONSE._serialized_end=305
+  _ANALYSISALGORITHMCONFIGNODE._serialized_start=307
+  _ANALYSISALGORITHMCONFIGNODE._serialized_end=379
+  _ANALYSISGETREQUEST._serialized_start=381
+  _ANALYSISGETREQUEST._serialized_end=455
+  _ANALYSIS._serialized_start=457
+  _ANALYSIS._serialized_end=557
+  _ANALYSISGETRESPONSE._serialized_start=559
+  _ANALYSISGETRESPONSE._serialized_end=679
+  _ANALYSISLISTREQUEST._serialized_start=682
+  _ANALYSISLISTREQUEST._serialized_end=869
+  _ANALYSISLISTRESPONSE._serialized_start=871
+  _ANALYSISLISTRESPONSE._serialized_end=992
+  _ANALYSISAPI._serialized_start=995
+  _ANALYSISAPI._serialized_end=1218
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/analysis_version_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/analysis_version_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: analysis_version.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
@@ -35,33 +34,33 @@
 
 from terrascope_api.models.common_models_pb2 import *
 from terrascope_api.models.analysis_pb2 import *
 from terrascope_api.models.algorithm_version_pb2 import *
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x61nalysis_version.proto\x12\x07oi.papi\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\x1a\x0e\x61nalysis.proto\x1a\x17\x61lgorithm_version.proto\"\xdb\x01\n\x10\x41nalysisManifest\x12\x18\n\x10manifest_version\x18\x01 \x01(\t\x12\x34\n\x08metadata\x18\x02 \x01(\x0b\x32\".oi.papi.AnalysisManifest.Metadata\x12\x37\n\x0f\x61lgorithm_nodes\x18\x03 \x03(\x0b\x32\x1e.oi.papi.AnalysisAlgorithmNode\x1a>\n\x08Metadata\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x0c\n\x04tags\x18\x03 \x03(\t\"\xdf\x01\n\x0f\x41nalysisVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12#\n\x08\x61nalysis\x18\x02 \x01(\x0b\x32\x11.oi.papi.Analysis\x12\x34\n\x11\x61nalysis_manifest\x18\x03 \x01(\x0b\x32\x19.oi.papi.AnalysisManifest\x12.\n\ncreated_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x12\x61lgorithm_versions\x18\x05 \x03(\x0b\x32\x19.oi.papi.AlgorithmVersion\"i\n\x1c\x41nalysisVersionCreateRequest\x12\x13\n\x0b\x61nalysis_id\x18\x01 \x01(\t\x12\x34\n\x11\x61nalysis_manifest\x18\x02 \x01(\x0b\x32\x19.oi.papi.AnalysisManifest\"h\n\x1d\x41nalysisVersionCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x32\n\x10\x61nalysis_version\x18\x02 \x01(\x0b\x32\x18.oi.papi.AnalysisVersion\"\x8e\x01\n\x19\x41nalysisVersionGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\x18\n\x10include_manifest\x18\x02 \x01(\x08\x12!\n\x19include_algorithm_details\x18\x03 \x01(\x08\x12\'\n\npagination\x18\x04 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x8f\x01\n\x1a\x41nalysisVersionGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x33\n\x11\x61nalysis_versions\x18\x02 \x03(\x0b\x32\x18.oi.papi.AnalysisVersion\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x9c\x02\n\x1a\x41nalysisVersionListRequest\x12\x13\n\x0b\x61nalysis_id\x18\x01 \x01(\t\x12\x0b\n\x03tag\x18\x02 \x01(\t\x12\x13\n\x0bsearch_text\x18\x03 \x01(\t\x12\x32\n\x0emin_created_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10include_manifest\x18\x06 \x01(\x08\x12\x1c\n\x14include_all_versions\x18\x07 \x01(\x08\x12\'\n\npagination\x18\x08 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x90\x01\n\x1b\x41nalysisVersionListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x33\n\x11\x61nalysis_versions\x18\x02 \x03(\x0b\x32\x18.oi.papi.AnalysisVersion\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination2\x90\x02\n\x12\x41nalysisVersionApi\x12W\n\x06\x63reate\x12%.oi.papi.AnalysisVersionCreateRequest\x1a&.oi.papi.AnalysisVersionCreateResponse\x12N\n\x03get\x12\".oi.papi.AnalysisVersionGetRequest\x1a#.oi.papi.AnalysisVersionGetResponse\x12Q\n\x04list\x12#.oi.papi.AnalysisVersionListRequest\x1a$.oi.papi.AnalysisVersionListResponseP\x01P\x02P\x03\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'analysis_version_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_ANALYSISMANIFEST']._serialized_start=131
-  _globals['_ANALYSISMANIFEST']._serialized_end=350
-  _globals['_ANALYSISMANIFEST_METADATA']._serialized_start=288
-  _globals['_ANALYSISMANIFEST_METADATA']._serialized_end=350
-  _globals['_ANALYSISVERSION']._serialized_start=353
-  _globals['_ANALYSISVERSION']._serialized_end=576
-  _globals['_ANALYSISVERSIONCREATEREQUEST']._serialized_start=578
-  _globals['_ANALYSISVERSIONCREATEREQUEST']._serialized_end=683
-  _globals['_ANALYSISVERSIONCREATERESPONSE']._serialized_start=685
-  _globals['_ANALYSISVERSIONCREATERESPONSE']._serialized_end=789
-  _globals['_ANALYSISVERSIONGETREQUEST']._serialized_start=792
-  _globals['_ANALYSISVERSIONGETREQUEST']._serialized_end=934
-  _globals['_ANALYSISVERSIONGETRESPONSE']._serialized_start=937
-  _globals['_ANALYSISVERSIONGETRESPONSE']._serialized_end=1080
-  _globals['_ANALYSISVERSIONLISTREQUEST']._serialized_start=1083
-  _globals['_ANALYSISVERSIONLISTREQUEST']._serialized_end=1367
-  _globals['_ANALYSISVERSIONLISTRESPONSE']._serialized_start=1370
-  _globals['_ANALYSISVERSIONLISTRESPONSE']._serialized_end=1514
-  _globals['_ANALYSISVERSIONAPI']._serialized_start=1517
-  _globals['_ANALYSISVERSIONAPI']._serialized_end=1789
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'analysis_version_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _ANALYSISMANIFEST._serialized_start=131
+  _ANALYSISMANIFEST._serialized_end=350
+  _ANALYSISMANIFEST_METADATA._serialized_start=288
+  _ANALYSISMANIFEST_METADATA._serialized_end=350
+  _ANALYSISVERSION._serialized_start=353
+  _ANALYSISVERSION._serialized_end=576
+  _ANALYSISVERSIONCREATEREQUEST._serialized_start=578
+  _ANALYSISVERSIONCREATEREQUEST._serialized_end=683
+  _ANALYSISVERSIONCREATERESPONSE._serialized_start=685
+  _ANALYSISVERSIONCREATERESPONSE._serialized_end=789
+  _ANALYSISVERSIONGETREQUEST._serialized_start=792
+  _ANALYSISVERSIONGETREQUEST._serialized_end=934
+  _ANALYSISVERSIONGETRESPONSE._serialized_start=937
+  _ANALYSISVERSIONGETRESPONSE._serialized_end=1080
+  _ANALYSISVERSIONLISTREQUEST._serialized_start=1083
+  _ANALYSISVERSIONLISTREQUEST._serialized_end=1367
+  _ANALYSISVERSIONLISTRESPONSE._serialized_start=1370
+  _ANALYSISVERSIONLISTRESPONSE._serialized_end=1514
+  _ANALYSISVERSIONAPI._serialized_start=1517
+  _ANALYSISVERSIONAPI._serialized_end=1789
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/aoi_catalog_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/result_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: aoi_catalog.proto
-# Protobuf Python Version: 5.26.1
+# source: result.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
-from terrascope_api.models import aoi_collection_pb2 as aoi__collection__pb2
+from terrascope_api.models import toi_pb2 as toi__pb2
 try:
-  common__models__pb2 = aoi__collection__pb2.common__models__pb2
+  common__models__pb2 = toi__pb2.common__models__pb2
 except AttributeError:
-  common__models__pb2 = aoi__collection__pb2.common_models_pb2
+  common__models__pb2 = toi__pb2.common_models_pb2
 
 from terrascope_api.models.common_models_pb2 import *
-from terrascope_api.models.aoi_collection_pb2 import *
+from terrascope_api.models.toi_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x61oi_catalog.proto\x12\x07oi.papi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x13\x63ommon_models.proto\x1a\x14\x61oi_collection.proto\"\x85\x02\n\x08\x41OIStats\x12+\n\ncategories\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12*\n\tcountries\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12(\n\x07sources\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06states\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12%\n\x04tags\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12&\n\x05types\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xe6\x01\n\x12\x41OIStatsGetRequest\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x13\n\x0bsearch_text\x18\x05 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\x12\x10\n\x08min_area\x18\x08 \x01(\x01\x12\x10\n\x08max_area\x18\t \x01(\x01\x12\x0f\n\x07sources\x18\n \x03(\t\x12*\n\x0clibrary_type\x18\x0b \x01(\x0e\x32\x14.oi.papi.LibraryType\"P\n\x13\x41OIStatsGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12$\n\taoi_stats\x18\x02 \x01(\x0b\x32\x11.oi.papi.AOIStats\"6\n\nAOICluster\x12\x0b\n\x03lat\x18\x01 \x01(\x01\x12\x0c\n\x04long\x18\x02 \x01(\x01\x12\r\n\x05\x63ount\x18\x03 \x01(\r\"\xe8\x01\n\x14\x41OIClusterGetRequest\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x13\n\x0bsearch_text\x18\x05 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\x12\x10\n\x08min_area\x18\x08 \x01(\x01\x12\x10\n\x08max_area\x18\t \x01(\x01\x12\x0f\n\x07sources\x18\n \x03(\t\x12*\n\x0clibrary_type\x18\x0b \x01(\x0e\x32\x14.oi.papi.LibraryType\"W\n\x15\x41OIClusterGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12)\n\x0c\x61oi_clusters\x18\x02 \x03(\x0b\x32\x13.oi.papi.AOICluster\"\'\n\x14\x41OICatalogAddRequest\x12\x0f\n\x07\x61oi_ids\x18\x01 \x03(\t\",\n\x15\x41OICatalogAddResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"*\n\x17\x41OICatalogDeleteRequest\x12\x0f\n\x07\x61oi_ids\x18\x01 \x03(\t\"/\n\x18\x41OICatalogDeleteResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"$\n\"AOICatalogGetPrivateCatalogRequest\"V\n#AOICatalogGetPrivateCatalogResponse\x12/\n\x0fuser_collection\x18\x01 \x01(\x0b\x32\x16.oi.papi.AOICollection*&\n\x0bLibraryType\x12\x0b\n\x07PRIVATE\x10\x00\x12\n\n\x06PUBLIC\x10\x01\x32\xe0\x03\n\rAOICatalogApi\x12J\n\rget_aoi_stats\x12\x1b.oi.papi.AOIStatsGetRequest\x1a\x1c.oi.papi.AOIStatsGetResponse\x12Q\n\x10get_aoi_clusters\x12\x1d.oi.papi.AOIClusterGetRequest\x1a\x1e.oi.papi.AOIClusterGetResponse\x12S\n\x12\x61\x64\x64_aoi_to_catalog\x12\x1d.oi.papi.AOICatalogAddRequest\x1a\x1e.oi.papi.AOICatalogAddResponse\x12^\n\x17\x64\x65lete_aoi_from_catalog\x12 .oi.papi.AOICatalogDeleteRequest\x1a!.oi.papi.AOICatalogDeleteResponse\x12{\n\x1eget_private_catalog_collection\x12+.oi.papi.AOICatalogGetPrivateCatalogRequest\x1a,.oi.papi.AOICatalogGetPrivateCatalogResponseP\x01P\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cresult.proto\x12\x07oi.papi\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\x1a\ttoi.proto\"\xae\x05\n\x06Result\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12source_aoi_version\x18\x03 \x01(\r\x12\x18\n\x10\x64\x65st_aoi_version\x18\x04 \x01(\r\x12\x19\n\x11\x61lgo_config_class\x18\x05 \x01(\t\x12\x1c\n\x14\x61lgo_config_subclass\x18\x06 \x01(\t\x12\x31\n\x0cobservations\x18\x07 \x03(\x0b\x32\x1b.oi.papi.Result.Observation\x12\x11\n\tdata_type\x18\x08 \x01(\t\x1a\xb2\x03\n\x0bObservation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x14\n\x0c\x64\x61ta_view_id\x18\x02 \x01(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08start_ts\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x05value\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x32\n\x06status\x18\x06 \x01(\x0e\x32\".oi.papi.Result.Observation.Status\x12=\n\x0cmeasurements\x18\x07 \x03(\x0b\x32\'.oi.papi.Result.Observation.Measurement\x1aO\n\x0bMeasurement\x12\n\n\x02id\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0c\n\x04geom\x18\x03 \x01(\t\"7\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0c\n\x08\x43OMPLETE\x10\x01\x12\x0b\n\x07PARTIAL\x10\x02\"\xb9\x03\n\x10ResultGetRequest\x12 \n\x18\x61lgorithm_computation_id\x18\x01 \x01(\t\x12\x1a\n\x12source_aoi_version\x18\x02 \x01(\r\x12\x18\n\x10\x64\x65st_aoi_version\x18\x03 \x01(\r\x12\x19\n\x11\x61lgo_config_class\x18\x04 \x01(\t\x12\x1c\n\x14\x61lgo_config_subclass\x18\x05 \x01(\t\x12.\n\ncreated_on\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14observation_start_ts\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08geom_wkt\x18\x08 \x01(\t\x12>\n\x12observation_status\x18\t \x01(\x0e\x32\".oi.papi.Result.Observation.Status\x12\x1c\n\x14include_measurements\x18\n \x01(\x08\x12\x11\n\tdata_type\x18\x0b \x01(\t\x12\'\n\npagination\x18\x0c \x01(\x0b\x32\x13.oi.papi.Pagination\"s\n\x11ResultGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12 \n\x07results\x18\x03 \x03(\x0b\x32\x0f.oi.papi.Result\"\xeb\x02\n\x13ResultExportRequest\x12 \n\x18\x61lgorithm_computation_id\x18\x01 \x01(\t\x12<\n\x0b\x65xport_type\x18\x02 \x01(\x0e\x32\'.oi.papi.ResultExportRequest.ExportType\x12\x38\n\tfile_type\x18\x03 \x01(\x0e\x32%.oi.papi.ResultExportRequest.FileType\x12\x1a\n\x12source_aoi_version\x18\x04 \x01(\r\"U\n\nExportType\x12\x17\n\x13UNKNOWN_EXPORT_TYPE\x10\x00\x12\x0c\n\x08STANDARD\x10\x01\x12\x0c\n\x08\x44\x45TAILED\x10\x02\x12\x12\n\x0eSINGLE_OBJECTS\x10\x03\"G\n\x08\x46ileType\x12\x15\n\x11UNKNOWN_FILE_TYPE\x10\x00\x12\x07\n\x03\x43SV\x10\x01\x12\x0b\n\x07GEOJSON\x10\x02\x12\x0e\n\nGEOPACKAGE\x10\x03\"c\n\x14ResultExportResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x14\n\x0c\x64ownload_url\x18\x02 \x01(\t\x12 \n\x18\x61lgorithm_computation_id\x18\x03 \x01(\t2\xc3\x01\n\tResultApi\x12T\n\x03get\x12\x19.oi.papi.ResultGetRequest\x1a\x1a.oi.papi.ResultGetResponse\"\x16\x82\xd3\xe4\x93\x02\x10\"\x0b/result/get:\x01*\x12`\n\x06\x65xport\x12\x1c.oi.papi.ResultExportRequest\x1a\x1d.oi.papi.ResultExportResponse\"\x19\x82\xd3\xe4\x93\x02\x13\"\x0e/result/export:\x01*P\x03P\x04\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aoi_catalog_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_LIBRARYTYPE']._serialized_start=1368
-  _globals['_LIBRARYTYPE']._serialized_end=1406
-  _globals['_AOISTATS']._serialized_start=104
-  _globals['_AOISTATS']._serialized_end=365
-  _globals['_AOISTATSGETREQUEST']._serialized_start=368
-  _globals['_AOISTATSGETREQUEST']._serialized_end=598
-  _globals['_AOISTATSGETRESPONSE']._serialized_start=600
-  _globals['_AOISTATSGETRESPONSE']._serialized_end=680
-  _globals['_AOICLUSTER']._serialized_start=682
-  _globals['_AOICLUSTER']._serialized_end=736
-  _globals['_AOICLUSTERGETREQUEST']._serialized_start=739
-  _globals['_AOICLUSTERGETREQUEST']._serialized_end=971
-  _globals['_AOICLUSTERGETRESPONSE']._serialized_start=973
-  _globals['_AOICLUSTERGETRESPONSE']._serialized_end=1060
-  _globals['_AOICATALOGADDREQUEST']._serialized_start=1062
-  _globals['_AOICATALOGADDREQUEST']._serialized_end=1101
-  _globals['_AOICATALOGADDRESPONSE']._serialized_start=1103
-  _globals['_AOICATALOGADDRESPONSE']._serialized_end=1147
-  _globals['_AOICATALOGDELETEREQUEST']._serialized_start=1149
-  _globals['_AOICATALOGDELETEREQUEST']._serialized_end=1191
-  _globals['_AOICATALOGDELETERESPONSE']._serialized_start=1193
-  _globals['_AOICATALOGDELETERESPONSE']._serialized_end=1240
-  _globals['_AOICATALOGGETPRIVATECATALOGREQUEST']._serialized_start=1242
-  _globals['_AOICATALOGGETPRIVATECATALOGREQUEST']._serialized_end=1278
-  _globals['_AOICATALOGGETPRIVATECATALOGRESPONSE']._serialized_start=1280
-  _globals['_AOICATALOGGETPRIVATECATALOGRESPONSE']._serialized_end=1366
-  _globals['_AOICATALOGAPI']._serialized_start=1409
-  _globals['_AOICATALOGAPI']._serialized_end=1889
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'result_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _RESULTAPI.methods_by_name['get']._options = None
+  _RESULTAPI.methods_by_name['get']._serialized_options = b'\202\323\344\223\002\020\"\013/result/get:\001*'
+  _RESULTAPI.methods_by_name['export']._options = None
+  _RESULTAPI.methods_by_name['export']._serialized_options = b'\202\323\344\223\002\023\"\016/result/export:\001*'
+  _RESULT._serialized_start=151
+  _RESULT._serialized_end=837
+  _RESULT_OBSERVATION._serialized_start=403
+  _RESULT_OBSERVATION._serialized_end=837
+  _RESULT_OBSERVATION_MEASUREMENT._serialized_start=701
+  _RESULT_OBSERVATION_MEASUREMENT._serialized_end=780
+  _RESULT_OBSERVATION_STATUS._serialized_start=782
+  _RESULT_OBSERVATION_STATUS._serialized_end=837
+  _RESULTGETREQUEST._serialized_start=840
+  _RESULTGETREQUEST._serialized_end=1281
+  _RESULTGETRESPONSE._serialized_start=1283
+  _RESULTGETRESPONSE._serialized_end=1398
+  _RESULTEXPORTREQUEST._serialized_start=1401
+  _RESULTEXPORTREQUEST._serialized_end=1764
+  _RESULTEXPORTREQUEST_EXPORTTYPE._serialized_start=1606
+  _RESULTEXPORTREQUEST_EXPORTTYPE._serialized_end=1691
+  _RESULTEXPORTREQUEST_FILETYPE._serialized_start=1693
+  _RESULTEXPORTREQUEST_FILETYPE._serialized_end=1764
+  _RESULTEXPORTRESPONSE._serialized_start=1766
+  _RESULTEXPORTRESPONSE._serialized_end=1865
+  _RESULTAPI._serialized_start=1868
+  _RESULTAPI._serialized_end=2063
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/aoi_collection_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/aoi_collection_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aoi_collection.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from terrascope_api.models import common_models_pb2 as common__models__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 from terrascope_api.models.common_models_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61oi_collection.proto\x12\x07oi.papi\x1a\x13\x63ommon_models.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"|\n\rAOICollection\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x10\n\x08num_aois\x18\x05 \x01(\r\"\x90\x01\n\x07\x41OIInfo\x12\x0e\n\x06\x61oi_id\x18\x01 \x01(\t\x12\x16\n\x0e\x61oi_version_id\x18\x02 \x01(\t\x12\x10\n\x08\x61oi_name\x18\x03 \x01(\t\x12\x0b\n\x03lat\x18\x04 \x01(\x02\x12\x0c\n\x04long\x18\x05 \x01(\x02\x12\x10\n\x08\x61rea_km2\x18\x06 \x01(\x01\x12\x0c\n\x04geom\x18\x07 \x01(\t\x12\x10\n\x08timezone\x18\x08 \x01(\t\"*\n\x1a\x41OICollectionCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"b\n\x1b\x41OICollectionCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12.\n\x0e\x61oi_collection\x18\x02 \x01(\x0b\x32\x16.oi.papi.AOICollection\"_\n\x17\x41OICollectionGetRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07verbose\x18\x02 \x01(\x08\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"|\n\x18\x41OICollectionGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\"\n\x08\x61oi_info\x18\x03 \x03(\x0b\x32\x10.oi.papi.AOIInfo\">\n\x17\x41OICollectionAddRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0f\x61oi_version_ids\x18\x02 \x03(\r\"/\n\x18\x41OICollectionAddResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"A\n\x1a\x41OICollectionRemoveRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0f\x61oi_version_ids\x18\x02 \x03(\r\"2\n\x1b\x41OICollectionRemoveResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"5\n\x19\x41OICollectionCloneRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"L\n\x1a\x41OICollectionCloneResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x19\n\x11\x61oi_collection_id\x18\x02 \x01(\t\"\xc0\x01\n\x18\x41OICollectionListRequest\x12\'\n\npagination\x18\x01 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\x32\n\x0emin_created_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bsearch_text\x18\x04 \x01(\t\"\x8a\x01\n\x19\x41OICollectionListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12/\n\x0f\x61oi_collections\x18\x03 \x03(\x0b\x32\x16.oi.papi.AOICollection2\xf5\x03\n\x10\x41OICollectionApi\x12S\n\x06\x63reate\x12#.oi.papi.AOICollectionCreateRequest\x1a$.oi.papi.AOICollectionCreateResponse\x12J\n\x03get\x12 .oi.papi.AOICollectionGetRequest\x1a!.oi.papi.AOICollectionGetResponse\x12P\n\x05\x63lone\x12\".oi.papi.AOICollectionCloneRequest\x1a#.oi.papi.AOICollectionCloneResponse\x12J\n\x03\x61\x64\x64\x12 .oi.papi.AOICollectionAddRequest\x1a!.oi.papi.AOICollectionAddResponse\x12S\n\x06remove\x12#.oi.papi.AOICollectionRemoveRequest\x1a$.oi.papi.AOICollectionRemoveResponse\x12M\n\x04list\x12!.oi.papi.AOICollectionListRequest\x1a\".oi.papi.AOICollectionListResponseP\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61oi_collection.proto\x12\x07oi.papi\x1a\x13\x63ommon_models.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"|\n\rAOICollection\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x10\n\x08num_aois\x18\x05 \x01(\r\"~\n\x07\x41OIInfo\x12\x0e\n\x06\x61oi_id\x18\x01 \x01(\t\x12\x16\n\x0e\x61oi_version_id\x18\x02 \x01(\t\x12\x10\n\x08\x61oi_name\x18\x03 \x01(\t\x12\x0b\n\x03lat\x18\x04 \x01(\x02\x12\x0c\n\x04long\x18\x05 \x01(\x02\x12\x10\n\x08\x61rea_km2\x18\x06 \x01(\x01\x12\x0c\n\x04geom\x18\x07 \x01(\t\"*\n\x1a\x41OICollectionCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"b\n\x1b\x41OICollectionCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12.\n\x0e\x61oi_collection\x18\x02 \x01(\x0b\x32\x16.oi.papi.AOICollection\"_\n\x17\x41OICollectionGetRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07verbose\x18\x02 \x01(\x08\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"|\n\x18\x41OICollectionGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\"\n\x08\x61oi_info\x18\x03 \x03(\x0b\x32\x10.oi.papi.AOIInfo\">\n\x17\x41OICollectionAddRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0f\x61oi_version_ids\x18\x02 \x03(\r\"/\n\x18\x41OICollectionAddResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"A\n\x1a\x41OICollectionRemoveRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0f\x61oi_version_ids\x18\x02 \x03(\r\"2\n\x1b\x41OICollectionRemoveResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"5\n\x19\x41OICollectionCloneRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"L\n\x1a\x41OICollectionCloneResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x19\n\x11\x61oi_collection_id\x18\x02 \x01(\t\"\xc0\x01\n\x18\x41OICollectionListRequest\x12\'\n\npagination\x18\x01 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\x32\n\x0emin_created_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bsearch_text\x18\x04 \x01(\t\"\x8a\x01\n\x19\x41OICollectionListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12/\n\x0f\x61oi_collections\x18\x03 \x03(\x0b\x32\x16.oi.papi.AOICollection2\xf5\x03\n\x10\x41OICollectionApi\x12S\n\x06\x63reate\x12#.oi.papi.AOICollectionCreateRequest\x1a$.oi.papi.AOICollectionCreateResponse\x12J\n\x03get\x12 .oi.papi.AOICollectionGetRequest\x1a!.oi.papi.AOICollectionGetResponse\x12P\n\x05\x63lone\x12\".oi.papi.AOICollectionCloneRequest\x1a#.oi.papi.AOICollectionCloneResponse\x12J\n\x03\x61\x64\x64\x12 .oi.papi.AOICollectionAddRequest\x1a!.oi.papi.AOICollectionAddResponse\x12S\n\x06remove\x12#.oi.papi.AOICollectionRemoveRequest\x1a$.oi.papi.AOICollectionRemoveResponse\x12M\n\x04list\x12!.oi.papi.AOICollectionListRequest\x1a\".oi.papi.AOICollectionListResponseP\x00\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aoi_collection_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_AOICOLLECTION']._serialized_start=87
-  _globals['_AOICOLLECTION']._serialized_end=211
-  _globals['_AOIINFO']._serialized_start=214
-  _globals['_AOIINFO']._serialized_end=358
-  _globals['_AOICOLLECTIONCREATEREQUEST']._serialized_start=360
-  _globals['_AOICOLLECTIONCREATEREQUEST']._serialized_end=402
-  _globals['_AOICOLLECTIONCREATERESPONSE']._serialized_start=404
-  _globals['_AOICOLLECTIONCREATERESPONSE']._serialized_end=502
-  _globals['_AOICOLLECTIONGETREQUEST']._serialized_start=504
-  _globals['_AOICOLLECTIONGETREQUEST']._serialized_end=599
-  _globals['_AOICOLLECTIONGETRESPONSE']._serialized_start=601
-  _globals['_AOICOLLECTIONGETRESPONSE']._serialized_end=725
-  _globals['_AOICOLLECTIONADDREQUEST']._serialized_start=727
-  _globals['_AOICOLLECTIONADDREQUEST']._serialized_end=789
-  _globals['_AOICOLLECTIONADDRESPONSE']._serialized_start=791
-  _globals['_AOICOLLECTIONADDRESPONSE']._serialized_end=838
-  _globals['_AOICOLLECTIONREMOVEREQUEST']._serialized_start=840
-  _globals['_AOICOLLECTIONREMOVEREQUEST']._serialized_end=905
-  _globals['_AOICOLLECTIONREMOVERESPONSE']._serialized_start=907
-  _globals['_AOICOLLECTIONREMOVERESPONSE']._serialized_end=957
-  _globals['_AOICOLLECTIONCLONEREQUEST']._serialized_start=959
-  _globals['_AOICOLLECTIONCLONEREQUEST']._serialized_end=1012
-  _globals['_AOICOLLECTIONCLONERESPONSE']._serialized_start=1014
-  _globals['_AOICOLLECTIONCLONERESPONSE']._serialized_end=1090
-  _globals['_AOICOLLECTIONLISTREQUEST']._serialized_start=1093
-  _globals['_AOICOLLECTIONLISTREQUEST']._serialized_end=1285
-  _globals['_AOICOLLECTIONLISTRESPONSE']._serialized_start=1288
-  _globals['_AOICOLLECTIONLISTRESPONSE']._serialized_end=1426
-  _globals['_AOICOLLECTIONAPI']._serialized_start=1429
-  _globals['_AOICOLLECTIONAPI']._serialized_end=1930
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aoi_collection_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _AOICOLLECTION._serialized_start=87
+  _AOICOLLECTION._serialized_end=211
+  _AOIINFO._serialized_start=213
+  _AOIINFO._serialized_end=339
+  _AOICOLLECTIONCREATEREQUEST._serialized_start=341
+  _AOICOLLECTIONCREATEREQUEST._serialized_end=383
+  _AOICOLLECTIONCREATERESPONSE._serialized_start=385
+  _AOICOLLECTIONCREATERESPONSE._serialized_end=483
+  _AOICOLLECTIONGETREQUEST._serialized_start=485
+  _AOICOLLECTIONGETREQUEST._serialized_end=580
+  _AOICOLLECTIONGETRESPONSE._serialized_start=582
+  _AOICOLLECTIONGETRESPONSE._serialized_end=706
+  _AOICOLLECTIONADDREQUEST._serialized_start=708
+  _AOICOLLECTIONADDREQUEST._serialized_end=770
+  _AOICOLLECTIONADDRESPONSE._serialized_start=772
+  _AOICOLLECTIONADDRESPONSE._serialized_end=819
+  _AOICOLLECTIONREMOVEREQUEST._serialized_start=821
+  _AOICOLLECTIONREMOVEREQUEST._serialized_end=886
+  _AOICOLLECTIONREMOVERESPONSE._serialized_start=888
+  _AOICOLLECTIONREMOVERESPONSE._serialized_end=938
+  _AOICOLLECTIONCLONEREQUEST._serialized_start=940
+  _AOICOLLECTIONCLONEREQUEST._serialized_end=993
+  _AOICOLLECTIONCLONERESPONSE._serialized_start=995
+  _AOICOLLECTIONCLONERESPONSE._serialized_end=1071
+  _AOICOLLECTIONLISTREQUEST._serialized_start=1074
+  _AOICOLLECTIONLISTREQUEST._serialized_end=1266
+  _AOICOLLECTIONLISTRESPONSE._serialized_start=1269
+  _AOICOLLECTIONLISTRESPONSE._serialized_end=1407
+  _AOICOLLECTIONAPI._serialized_start=1410
+  _AOICOLLECTIONAPI._serialized_end=1911
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/aoi_export_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/user_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: aoi_export.proto
-# Protobuf Python Version: 5.26.1
+# source: user.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from terrascope_api.models import common_models_pb2 as common__models__pb2
 
+from terrascope_api.models.common_models_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x61oi_export.proto\x12\x07oi.papi\"\x9a\x01\n\x10\x41OIExportRequest\x12\x0f\n\x07\x61oi_ids\x18\x01 \x03(\t\x12-\n\tfile_type\x18\x02 \x01(\x0e\x32\x1a.oi.papi.AOIExportFileType\x12\x33\n\x0c\x61rchive_type\x18\x03 \x01(\x0e\x32\x1d.oi.papi.AOIExportArchiveType\x12\x11\n\tfile_name\x18\x04 \x01(\t\"\xae\x01\n\x1a\x41OICollectionExportRequest\x12\x19\n\x11\x61oi_collection_id\x18\x01 \x01(\t\x12-\n\tfile_type\x18\x02 \x01(\x0e\x32\x1a.oi.papi.AOIExportFileType\x12\x33\n\x0c\x61rchive_type\x18\x03 \x01(\x0e\x32\x1d.oi.papi.AOIExportArchiveType\x12\x11\n\tfile_name\x18\x04 \x01(\t\"%\n\x11\x41OIExportResponse\x12\x10\n\x08location\x18\x01 \x01(\t\"/\n\x1b\x41OICollectionExportResponse\x12\x10\n\x08location\x18\x01 \x01(\t*a\n\x11\x41OIExportFileType\x12\x1b\n\x17UNKNOWN_EXPORT_FILETYPE\x10\x00\x12\x0b\n\x07GEOJSON\x10\x01\x12\x12\n\x0e\x45SRI_SHAPEFILE\x10\x02\x12\x0e\n\nGEOPACKAGE\x10\x03*>\n\x14\x41OIExportArchiveType\x12\x18\n\x14UNKNOWN_ARCHIVE_TYPE\x10\x00\x12\x0c\n\x08ZIP_FILE\x10\x01\x32\xb4\x01\n\x0c\x41OIExportApi\x12\x44\n\x0b\x65xport_aois\x12\x19.oi.papi.AOIExportRequest\x1a\x1a.oi.papi.AOIExportResponse\x12^\n\x11\x65xport_collection\x12#.oi.papi.AOICollectionExportRequest\x1a$.oi.papi.AOICollectionExportResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nuser.proto\x12\x07oi.papi\x1a\x13\x63ommon_models.proto\"/\n\x0cLoginRequest\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"7\n\rLoginResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x11\n\tjwt_token\x18\x02 \x01(\t\"/\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\"L\n\x11UserCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\x12\x1a\n\x12user_collection_id\x18\x03 \x01(\t\"F\n\x12UserCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x1b\n\x04user\x18\x02 \x01(\x0b\x32\r.oi.papi.User\"\x1d\n\x0eUserGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"D\n\x0fUserGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x1c\n\x05users\x18\x02 \x03(\x0b\x32\r.oi.papi.User\" \n\x0fUserListRequest\x12\r\n\x05\x65mail\x18\x01 \x01(\t\"E\n\x10UserListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x1c\n\x05users\x18\x02 \x03(\x0b\x32\r.oi.papi.User2\xfb\x01\n\x07UserApi\x12\x36\n\x05login\x12\x15.oi.papi.LoginRequest\x1a\x16.oi.papi.LoginResponse\x12\x41\n\x06\x63reate\x12\x1a.oi.papi.UserCreateRequest\x1a\x1b.oi.papi.UserCreateResponse\x12\x38\n\x03get\x12\x17.oi.papi.UserGetRequest\x1a\x18.oi.papi.UserGetResponse\x12;\n\x04list\x12\x18.oi.papi.UserListRequest\x1a\x19.oi.papi.UserListResponseP\x00\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aoi_export_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_AOIEXPORTFILETYPE']._serialized_start=451
-  _globals['_AOIEXPORTFILETYPE']._serialized_end=548
-  _globals['_AOIEXPORTARCHIVETYPE']._serialized_start=550
-  _globals['_AOIEXPORTARCHIVETYPE']._serialized_end=612
-  _globals['_AOIEXPORTREQUEST']._serialized_start=30
-  _globals['_AOIEXPORTREQUEST']._serialized_end=184
-  _globals['_AOICOLLECTIONEXPORTREQUEST']._serialized_start=187
-  _globals['_AOICOLLECTIONEXPORTREQUEST']._serialized_end=361
-  _globals['_AOIEXPORTRESPONSE']._serialized_start=363
-  _globals['_AOIEXPORTRESPONSE']._serialized_end=400
-  _globals['_AOICOLLECTIONEXPORTRESPONSE']._serialized_start=402
-  _globals['_AOICOLLECTIONEXPORTRESPONSE']._serialized_end=449
-  _globals['_AOIEXPORTAPI']._serialized_start=615
-  _globals['_AOIEXPORTAPI']._serialized_end=795
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'user_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _LOGINREQUEST._serialized_start=44
+  _LOGINREQUEST._serialized_end=91
+  _LOGINRESPONSE._serialized_start=93
+  _LOGINRESPONSE._serialized_end=148
+  _USER._serialized_start=150
+  _USER._serialized_end=197
+  _USERCREATEREQUEST._serialized_start=199
+  _USERCREATEREQUEST._serialized_end=275
+  _USERCREATERESPONSE._serialized_start=277
+  _USERCREATERESPONSE._serialized_end=347
+  _USERGETREQUEST._serialized_start=349
+  _USERGETREQUEST._serialized_end=378
+  _USERGETRESPONSE._serialized_start=380
+  _USERGETRESPONSE._serialized_end=448
+  _USERLISTREQUEST._serialized_start=450
+  _USERLISTREQUEST._serialized_end=482
+  _USERLISTRESPONSE._serialized_start=484
+  _USERLISTRESPONSE._serialized_end=553
+  _USERAPI._serialized_start=556
+  _USERAPI._serialized_end=807
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/aoi_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/aoi_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aoi.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
 
 from terrascope_api.models.common_models_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\taoi.proto\x12\x07oi.papi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\"\x8c\x01\n\x0e\x41OITransaction\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"7\n\rAOIIdentifier\x12\x0e\n\x06\x61oi_id\x18\x01 \x01(\t\x12\x16\n\x0e\x61oi_version_id\x18\x02 \x01(\r\"\xa5\x02\n\tAOIObject\x12.\n\x0e\x61oi_identifier\x18\x01 \x01(\x0b\x32\x16.oi.papi.AOIIdentifier\x12\x10\n\x08geom_wkt\x18\x02 \x01(\t\x12\x0b\n\x03lat\x18\x03 \x01(\x02\x12\x0c\n\x04long\x18\x04 \x01(\x02\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x10\n\x08\x61rea_km2\x18\x06 \x01(\x01\x12\x10\n\x08\x63\x61tegory\x18\x07 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x0e\n\x06source\x18\t \x01(\t\x12\x0f\n\x07\x63ountry\x18\n \x01(\t\x12\r\n\x05state\x18\x0b \x01(\t\x12\x0c\n\x04tags\x18\x0c \x03(\t\x12+\n\nattributes\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x10\n\x08timezone\x18\x0e \x01(\t\"\xdf\x02\n\nAOIVersion\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0e\n\x06\x61oi_id\x18\x02 \x01(\t\x12\x36\n\x12\x63reation_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x63reator\x18\x04 \x01(\t\x12\x10\n\x08\x61oi_name\x18\x05 \x01(\t\x12\x10\n\x08geom_wkt\x18\x06 \x01(\t\x12\x0b\n\x03lat\x18\x07 \x01(\x02\x12\x0c\n\x04long\x18\x08 \x01(\x02\x12\x10\n\x08\x61rea_km2\x18\t \x01(\x01\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x0e\n\x06source\x18\x0c \x01(\t\x12\x0f\n\x07\x63ountry\x18\r \x01(\t\x12\r\n\x05state\x18\x0e \x01(\t\x12\x0c\n\x04tags\x18\x0f \x03(\t\x12+\n\nattributes\x18\x10 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x10\n\x08timezone\x18\x11 \x01(\t\"\x95\x01\n\x08\x41OIInput\x12\x0e\n\x06\x61oi_id\x18\x01 \x01(\t\x12\x10\n\x08geom_wkt\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0c\n\x04tags\x18\x06 \x03(\t\x12+\n\nattributes\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"T\n\x10\x41OICreateRequest\x12%\n\naoi_inputs\x18\x01 \x03(\x0b\x32\x11.oi.papi.AOIInput\x12\x19\n\x11\x61oi_collection_id\x18\x02 \x01(\t\"\x94\x01\n\x11\x41OICreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12/\n\x0f\x61oi_identifiers\x18\x03 \x03(\x0b\x32\x16.oi.papi.AOIIdentifier\x12\x10\n\x08\x61rea_km2\x18\x04 \x03(\x01\"<\n\x10\x41OIUploadRequest\x12\x19\n\x11\x61oi_collection_id\x18\x01 \x01(\t\x12\r\n\x05\x63hunk\x18\x02 \x01(\x0c\"Z\n\x11\x41OIUploadResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x30\n\x0f\x61oi_transaction\x18\x02 \x01(\x0b\x32\x17.oi.papi.AOITransaction\"V\n\rAOIGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\x0f\n\x07verbose\x18\x02 \x01(\x08\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"y\n\x0e\x41OIGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12)\n\x0c\x61oi_versions\x18\x03 \x03(\x0b\x32\x13.oi.papi.AOIVersion\"U\n\x10\x41OIUpdateRequest\x12\x0e\n\x06\x61oi_id\x18\x01 \x01(\t\x12\x31\n\x16\x61oi_modification_input\x18\x02 \x01(\x0b\x32\x11.oi.papi.AOIInput\"(\n\x11\x41OIUpdateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r2\x85\x02\n\x06\x41OIApi\x12?\n\x06\x63reate\x12\x19.oi.papi.AOICreateRequest\x1a\x1a.oi.papi.AOICreateResponse\x12\x36\n\x03get\x12\x16.oi.papi.AOIGetRequest\x1a\x17.oi.papi.AOIGetResponse\x12\x41\n\x06upload\x12\x19.oi.papi.AOIUploadRequest\x1a\x1a.oi.papi.AOIUploadResponse(\x01\x12?\n\x06update\x12\x19.oi.papi.AOIUpdateRequest\x1a\x1a.oi.papi.AOIUpdateResponseP\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\taoi.proto\x12\x07oi.papi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\"\x8c\x01\n\x0e\x41OITransaction\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"7\n\rAOIIdentifier\x12\x0e\n\x06\x61oi_id\x18\x01 \x01(\t\x12\x16\n\x0e\x61oi_version_id\x18\x02 \x01(\r\"\xab\x02\n\tAOIObject\x12.\n\x0e\x61oi_identifier\x18\x01 \x01(\x0b\x32\x16.oi.papi.AOIIdentifier\x12\x10\n\x08geom_wkt\x18\x02 \x01(\t\x12\x0b\n\x03lat\x18\x03 \x01(\x02\x12\x0c\n\x04long\x18\x04 \x01(\x02\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x10\n\x08\x61rea_km2\x18\x06 \x01(\x01\x12\x10\n\x08\x63\x61tegory\x18\x07 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x0e\n\x06source\x18\t \x01(\t\x12\x0f\n\x07\x63ountry\x18\n \x01(\t\x12\r\n\x05state\x18\x0b \x01(\t\x12\x0c\n\x04tags\x18\x0c \x03(\t\x12+\n\nattributes\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x16\n\x0elocal_timezone\x18\x0e \x01(\t\"\xe5\x02\n\nAOIVersion\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0e\n\x06\x61oi_id\x18\x02 \x01(\t\x12\x36\n\x12\x63reation_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x63reator\x18\x04 \x01(\t\x12\x10\n\x08\x61oi_name\x18\x05 \x01(\t\x12\x10\n\x08geom_wkt\x18\x06 \x01(\t\x12\x0b\n\x03lat\x18\x07 \x01(\x02\x12\x0c\n\x04long\x18\x08 \x01(\x02\x12\x10\n\x08\x61rea_km2\x18\t \x01(\x01\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x0e\n\x06source\x18\x0c \x01(\t\x12\x0f\n\x07\x63ountry\x18\r \x01(\t\x12\r\n\x05state\x18\x0e \x01(\t\x12\x0c\n\x04tags\x18\x0f \x03(\t\x12+\n\nattributes\x18\x10 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x16\n\x0elocal_timezone\x18\x11 \x01(\t\"\x95\x01\n\x08\x41OIInput\x12\x0e\n\x06\x61oi_id\x18\x01 \x01(\t\x12\x10\n\x08geom_wkt\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0c\n\x04tags\x18\x06 \x03(\t\x12+\n\nattributes\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"T\n\x10\x41OICreateRequest\x12%\n\naoi_inputs\x18\x01 \x03(\x0b\x32\x11.oi.papi.AOIInput\x12\x19\n\x11\x61oi_collection_id\x18\x02 \x01(\t\"\x94\x01\n\x11\x41OICreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12/\n\x0f\x61oi_identifiers\x18\x03 \x03(\x0b\x32\x16.oi.papi.AOIIdentifier\x12\x10\n\x08\x61rea_km2\x18\x04 \x03(\x01\"<\n\x10\x41OIUploadRequest\x12\x19\n\x11\x61oi_collection_id\x18\x01 \x01(\t\x12\r\n\x05\x63hunk\x18\x02 \x01(\x0c\"Z\n\x11\x41OIUploadResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x30\n\x0f\x61oi_transaction\x18\x02 \x01(\x0b\x32\x17.oi.papi.AOITransaction\"V\n\rAOIGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\x0f\n\x07verbose\x18\x02 \x01(\x08\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"y\n\x0e\x41OIGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12)\n\x0c\x61oi_versions\x18\x03 \x03(\x0b\x32\x13.oi.papi.AOIVersion\"U\n\x10\x41OIUpdateRequest\x12\x0e\n\x06\x61oi_id\x18\x01 \x01(\t\x12\x31\n\x16\x61oi_modification_input\x18\x02 \x01(\x0b\x32\x11.oi.papi.AOIInput\"(\n\x11\x41OIUpdateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r2\x85\x02\n\x06\x41OIApi\x12?\n\x06\x63reate\x12\x19.oi.papi.AOICreateRequest\x1a\x1a.oi.papi.AOICreateResponse\x12\x36\n\x03get\x12\x16.oi.papi.AOIGetRequest\x1a\x17.oi.papi.AOIGetResponse\x12\x41\n\x06upload\x12\x19.oi.papi.AOIUploadRequest\x1a\x1a.oi.papi.AOIUploadResponse(\x01\x12?\n\x06update\x12\x19.oi.papi.AOIUpdateRequest\x1a\x1a.oi.papi.AOIUpdateResponseP\x02\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aoi_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_AOITRANSACTION']._serialized_start=107
-  _globals['_AOITRANSACTION']._serialized_end=247
-  _globals['_AOIIDENTIFIER']._serialized_start=249
-  _globals['_AOIIDENTIFIER']._serialized_end=304
-  _globals['_AOIOBJECT']._serialized_start=307
-  _globals['_AOIOBJECT']._serialized_end=600
-  _globals['_AOIVERSION']._serialized_start=603
-  _globals['_AOIVERSION']._serialized_end=954
-  _globals['_AOIINPUT']._serialized_start=957
-  _globals['_AOIINPUT']._serialized_end=1106
-  _globals['_AOICREATEREQUEST']._serialized_start=1108
-  _globals['_AOICREATEREQUEST']._serialized_end=1192
-  _globals['_AOICREATERESPONSE']._serialized_start=1195
-  _globals['_AOICREATERESPONSE']._serialized_end=1343
-  _globals['_AOIUPLOADREQUEST']._serialized_start=1345
-  _globals['_AOIUPLOADREQUEST']._serialized_end=1405
-  _globals['_AOIUPLOADRESPONSE']._serialized_start=1407
-  _globals['_AOIUPLOADRESPONSE']._serialized_end=1497
-  _globals['_AOIGETREQUEST']._serialized_start=1499
-  _globals['_AOIGETREQUEST']._serialized_end=1585
-  _globals['_AOIGETRESPONSE']._serialized_start=1587
-  _globals['_AOIGETRESPONSE']._serialized_end=1708
-  _globals['_AOIUPDATEREQUEST']._serialized_start=1710
-  _globals['_AOIUPDATEREQUEST']._serialized_end=1795
-  _globals['_AOIUPDATERESPONSE']._serialized_start=1797
-  _globals['_AOIUPDATERESPONSE']._serialized_end=1837
-  _globals['_AOIAPI']._serialized_start=1840
-  _globals['_AOIAPI']._serialized_end=2101
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aoi_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _AOITRANSACTION._serialized_start=107
+  _AOITRANSACTION._serialized_end=247
+  _AOIIDENTIFIER._serialized_start=249
+  _AOIIDENTIFIER._serialized_end=304
+  _AOIOBJECT._serialized_start=307
+  _AOIOBJECT._serialized_end=606
+  _AOIVERSION._serialized_start=609
+  _AOIVERSION._serialized_end=966
+  _AOIINPUT._serialized_start=969
+  _AOIINPUT._serialized_end=1118
+  _AOICREATEREQUEST._serialized_start=1120
+  _AOICREATEREQUEST._serialized_end=1204
+  _AOICREATERESPONSE._serialized_start=1207
+  _AOICREATERESPONSE._serialized_end=1355
+  _AOIUPLOADREQUEST._serialized_start=1357
+  _AOIUPLOADREQUEST._serialized_end=1417
+  _AOIUPLOADRESPONSE._serialized_start=1419
+  _AOIUPLOADRESPONSE._serialized_end=1509
+  _AOIGETREQUEST._serialized_start=1511
+  _AOIGETREQUEST._serialized_end=1597
+  _AOIGETRESPONSE._serialized_start=1599
+  _AOIGETRESPONSE._serialized_end=1720
+  _AOIUPDATEREQUEST._serialized_start=1722
+  _AOIUPDATEREQUEST._serialized_end=1807
+  _AOIUPDATERESPONSE._serialized_start=1809
+  _AOIUPDATERESPONSE._serialized_end=1849
+  _AOIAPI._serialized_start=1852
+  _AOIAPI._serialized_end=2113
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/aoi_version_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/aoi_version_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aoi_version.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from terrascope_api.models import common_models_pb2 as common__models__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
@@ -19,35 +18,31 @@
   common__models__pb2 = aoi__pb2.common__models__pb2
 except AttributeError:
   common__models__pb2 = aoi__pb2.common_models_pb2
 
 from terrascope_api.models.common_models_pb2 import *
 from terrascope_api.models.aoi_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x61oi_version.proto\x12\x07oi.papi\x1a\x13\x63ommon_models.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\taoi.proto\"s\n\x14\x41OIVersionGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\r\x12%\n\naoi_fields\x18\x02 \x03(\x0e\x32\x11.oi.papi.AOIField\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x80\x01\n\x15\x41OIVersionGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12)\n\x0c\x61oi_versions\x18\x03 \x03(\x0b\x32\x13.oi.papi.AOIVersion\"\\\n\x17\x41OIVersionCreateRequest\x12\x0e\n\x06\x61oi_id\x18\x01 \x01(\t\x12\x31\n\x16\x61oi_modification_input\x18\x02 \x01(\x0b\x32\x11.oi.papi.AOIInput\"\x82\x01\n\x18\x41OIVersionCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12(\n\x0b\x61oi_version\x18\x03 \x01(\x0b\x32\x13.oi.papi.AOIVersion\"\xc1\x05\n\x15\x41OIVersionListRequest\x12\x10\n\x08geom_wkt\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x0c\n\x04tags\x18\x03 \x03(\t\x12\x13\n\x0bsearch_text\x18\x04 \x01(\t\x12\x32\n\x0emin_created_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12%\n\naoi_fields\x18\x07 \x03(\x0e\x32\x11.oi.papi.AOIField\x12\'\n\npagination\x18\x08 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\x0f\n\x07verbose\x18\t \x01(\x08\x12\x0c\n\x04\x62\x62ox\x18\n \x03(\x01\x12$\n\tsort_keys\x18\x0b \x01(\x0e\x32\x11.oi.papi.AOIField\x12<\n\nsort_order\x18\x0c \x01(\x0e\x32(.oi.papi.AOIVersionListRequest.SortOrder\x12\x10\n\x08\x61oi_type\x18\r \x01(\t\x12\x0f\n\x07\x63ountry\x18\x0e \x01(\t\x12\r\n\x05state\x18\x0f \x01(\t\x12\x10\n\x08min_area\x18\x10 \x01(\x01\x12\x10\n\x08max_area\x18\x11 \x01(\x01\x12\x14\n\x0c\x64\x61ta_sources\x18\x12 \x03(\t\x12@\n\x0clibrary_type\x18\x13 \x01(\x0e\x32*.oi.papi.AOIVersionListRequest.LibraryType\"@\n\x0bLibraryType\x12\x18\n\x14UNKNOWN_LIBRARY_TYPE\x10\x00\x12\x0b\n\x07PRIVATE\x10\x01\x12\n\n\x06PUBLIC\x10\x02\"6\n\tSortOrder\x12\x16\n\x12UNKNOWN_SORT_ORDER\x10\x00\x12\x07\n\x03\x41SC\x10\x01\x12\x08\n\x04\x44\x45SC\x10\x02\"\x81\x01\n\x16\x41OIVersionListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12)\n\x0c\x61oi_versions\x18\x03 \x03(\x0b\x32\x13.oi.papi.AOIVersion*\xea\x01\n\x08\x41OIField\x12\x15\n\x11UNKNOWN_AOI_FIELD\x10\x00\x12\n\n\x06\x41OI_ID\x10\x01\x12\x0c\n\x08GEOM_WKT\x10\x02\x12\x07\n\x03LAT\x10\x03\x12\x08\n\x04LONG\x10\x04\x12\x08\n\x04NAME\x10\x05\x12\x0c\n\x08\x41REA_KM2\x10\x06\x12\x0c\n\x08\x43\x41TEGORY\x10\x07\x12\x08\n\x04TYPE\x10\x08\x12\n\n\x06SOURCE\x10\t\x12\x0b\n\x07\x43OUNTRY\x10\n\x12\t\n\x05STATE\x10\x0b\x12\x08\n\x04TAGS\x10\x0c\x12\x0e\n\nATTRIBUTES\x10\r\x12\x0c\n\x08TIMEZONE\x10\x0e\x12\x0e\n\nCREATED_ON\x10\x0f\x12\x0e\n\nCREATED_BY\x10\x10\x32\xed\x01\n\rAOIVersionApi\x12M\n\x06\x63reate\x12 .oi.papi.AOIVersionCreateRequest\x1a!.oi.papi.AOIVersionCreateResponse\x12\x44\n\x03get\x12\x1d.oi.papi.AOIVersionGetRequest\x1a\x1e.oi.papi.AOIVersionGetResponse\x12G\n\x04list\x12\x1e.oi.papi.AOIVersionListRequest\x1a\x1f.oi.papi.AOIVersionListResponseP\x00P\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x61oi_version.proto\x12\x07oi.papi\x1a\x13\x63ommon_models.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\taoi.proto\"s\n\x14\x41OIVersionGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\r\x12%\n\naoi_fields\x18\x02 \x03(\x0e\x32\x11.oi.papi.AOIField\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"\x80\x01\n\x15\x41OIVersionGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12)\n\x0c\x61oi_versions\x18\x03 \x03(\x0b\x32\x13.oi.papi.AOIVersion\"\\\n\x17\x41OIVersionCreateRequest\x12\x0e\n\x06\x61oi_id\x18\x01 \x01(\t\x12\x31\n\x16\x61oi_modification_input\x18\x02 \x01(\x0b\x32\x11.oi.papi.AOIInput\"\x82\x01\n\x18\x41OIVersionCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12(\n\x0b\x61oi_version\x18\x03 \x01(\x0b\x32\x13.oi.papi.AOIVersion\"\xa7\x02\n\x15\x41OIVersionListRequest\x12\x10\n\x08geom_wkt\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x0c\n\x04tags\x18\x03 \x03(\t\x12\x13\n\x0bsearch_text\x18\x04 \x01(\t\x12\x32\n\x0emin_created_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0emax_created_on\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12%\n\naoi_fields\x18\x07 \x03(\x0e\x32\x11.oi.papi.AOIField\x12\'\n\npagination\x18\x08 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\x0f\n\x07verbose\x18\t \x01(\x08\"\x81\x01\n\x16\x41OIVersionListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12)\n\x0c\x61oi_versions\x18\x03 \x03(\x0b\x32\x13.oi.papi.AOIVersion*\xf0\x01\n\x08\x41OIField\x12\x15\n\x11UNKNOWN_AOI_FIELD\x10\x00\x12\n\n\x06\x41OI_ID\x10\x01\x12\x0c\n\x08GEOM_WKT\x10\x02\x12\x07\n\x03LAT\x10\x03\x12\x08\n\x04LONG\x10\x04\x12\x08\n\x04NAME\x10\x05\x12\x0c\n\x08\x41REA_KM2\x10\x06\x12\x0c\n\x08\x43\x41TEGORY\x10\x07\x12\x08\n\x04TYPE\x10\x08\x12\n\n\x06SOURCE\x10\t\x12\x0b\n\x07\x43OUNTRY\x10\n\x12\t\n\x05STATE\x10\x0b\x12\x08\n\x04TAGS\x10\x0c\x12\x0e\n\nATTRIBUTES\x10\r\x12\x12\n\x0eLOCAL_TIMEZONE\x10\x0e\x12\x0e\n\nCREATED_ON\x10\x0f\x12\x0e\n\nCREATED_BY\x10\x10\x32\xed\x01\n\rAOIVersionApi\x12M\n\x06\x63reate\x12 .oi.papi.AOIVersionCreateRequest\x1a!.oi.papi.AOIVersionCreateResponse\x12\x44\n\x03get\x12\x1d.oi.papi.AOIVersionGetRequest\x1a\x1e.oi.papi.AOIVersionGetResponse\x12G\n\x04list\x12\x1e.oi.papi.AOIVersionListRequest\x1a\x1f.oi.papi.AOIVersionListResponseP\x00P\x02\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aoi_version_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_AOIFIELD']._serialized_start=1411
-  _globals['_AOIFIELD']._serialized_end=1645
-  _globals['_AOIVERSIONGETREQUEST']._serialized_start=95
-  _globals['_AOIVERSIONGETREQUEST']._serialized_end=210
-  _globals['_AOIVERSIONGETRESPONSE']._serialized_start=213
-  _globals['_AOIVERSIONGETRESPONSE']._serialized_end=341
-  _globals['_AOIVERSIONCREATEREQUEST']._serialized_start=343
-  _globals['_AOIVERSIONCREATEREQUEST']._serialized_end=435
-  _globals['_AOIVERSIONCREATERESPONSE']._serialized_start=438
-  _globals['_AOIVERSIONCREATERESPONSE']._serialized_end=568
-  _globals['_AOIVERSIONLISTREQUEST']._serialized_start=571
-  _globals['_AOIVERSIONLISTREQUEST']._serialized_end=1276
-  _globals['_AOIVERSIONLISTREQUEST_LIBRARYTYPE']._serialized_start=1156
-  _globals['_AOIVERSIONLISTREQUEST_LIBRARYTYPE']._serialized_end=1220
-  _globals['_AOIVERSIONLISTREQUEST_SORTORDER']._serialized_start=1222
-  _globals['_AOIVERSIONLISTREQUEST_SORTORDER']._serialized_end=1276
-  _globals['_AOIVERSIONLISTRESPONSE']._serialized_start=1279
-  _globals['_AOIVERSIONLISTRESPONSE']._serialized_end=1408
-  _globals['_AOIVERSIONAPI']._serialized_start=1648
-  _globals['_AOIVERSIONAPI']._serialized_end=1885
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aoi_version_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _AOIFIELD._serialized_start=1001
+  _AOIFIELD._serialized_end=1241
+  _AOIVERSIONGETREQUEST._serialized_start=95
+  _AOIVERSIONGETREQUEST._serialized_end=210
+  _AOIVERSIONGETRESPONSE._serialized_start=213
+  _AOIVERSIONGETRESPONSE._serialized_end=341
+  _AOIVERSIONCREATEREQUEST._serialized_start=343
+  _AOIVERSIONCREATEREQUEST._serialized_end=435
+  _AOIVERSIONCREATERESPONSE._serialized_start=438
+  _AOIVERSIONCREATERESPONSE._serialized_end=568
+  _AOIVERSIONLISTREQUEST._serialized_start=571
+  _AOIVERSIONLISTREQUEST._serialized_end=866
+  _AOIVERSIONLISTRESPONSE._serialized_start=869
+  _AOIVERSIONLISTRESPONSE._serialized_end=998
+  _AOIVERSIONAPI._serialized_start=1244
+  _AOIVERSIONAPI._serialized_end=1481
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/common_models_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/common_models_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: common_models.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x63ommon_models.proto\x12\x07oi.papi\"L\n\nPagination\x12\x12\n\npage_token\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\r\x12\x17\n\x0fnext_page_token\x18\x03 \x01(\tb\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common_models_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_PAGINATION']._serialized_start=32
-  _globals['_PAGINATION']._serialized_end=108
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common_models_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _PAGINATION._serialized_start=32
+  _PAGINATION._serialized_end=108
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/credit_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/credit_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: credit.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
 
 from terrascope_api.models.common_models_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63redit.proto\x12\x0eoi.papi.credit\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\"E\n\x10\x43reditAddRequest\x12\x11\n\tsource_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x01\x12\x0e\n\x06reason\x18\x03 \x01(\t\"(\n\x11\x43reditAddResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"H\n\x13\x43reditRemoveRequest\x12\x11\n\tsource_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x01\x12\x0e\n\x06reason\x18\x03 \x01(\t\"+\n\x14\x43reditRemoveResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"H\n\x13\x43reditRefundRequest\x12\x11\n\tsource_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x01\x12\x0e\n\x06reason\x18\x03 \x01(\t\"+\n\x14\x43reditRefundResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"\x85\x01\n#CreditAlgorithmMultiplierSetRequest\x12\x1c\n\x14\x61lgorithm_version_id\x18\x01 \x01(\t\x12!\n\x19\x61lgorithm_execution_price\x18\x02 \x01(\x01\x12\x1d\n\x15\x61lgorithm_value_price\x18\x03 \x01(\x01\";\n$CreditAlgorithmMultiplierSetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"Y\n$CreditDataSourceMultiplierSetRequest\x12\x16\n\x0e\x64\x61ta_source_id\x18\x01 \x01(\t\x12\x19\n\x11\x64\x61ta_source_price\x18\x02 \x01(\x01\"<\n%CreditDataSourceMultiplierSetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"\xd9\x02\n\x15\x43reditEstimateRequest\x12 \n\x18\x61lgorithm_computation_id\x18\x01 \x01(\t\x12 \n\x18\x61nalysis_computation_ids\x18\x02 \x03(\t\x12S\n\x12\x61nalysis_resources\x18\x03 \x01(\x0b\x32\x37.oi.papi.credit.CreditEstimateRequest.AnalysisResources\x1a\xa6\x01\n\x11\x41nalysisResources\x12\x1a\n\x12\x61oi_collection_ids\x18\x01 \x03(\t\x12\x1b\n\x13\x61nalysis_config_ids\x18\x02 \x03(\t\x12,\n\x08start_ts\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x65nd_ts\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"S\n\x16\x43reditEstimateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x17\n\x0f\x63redit_estimate\x18\x02 \x01(\x01\x12\x0b\n\x03msg\x18\x03 \x01(\t\"N\n\x06\x43redit\x12\x11\n\tsource_id\x18\x01 \x01(\t\x12\x11\n\tavailable\x18\x02 \x01(\x01\x12\x10\n\x08reserved\x18\x03 \x01(\x01\x12\x0c\n\x04used\x18\x04 \x01(\x01\")\n\x14\x43reditSummaryRequest\x12\x11\n\tsource_id\x18\x01 \x01(\t\"T\n\x15\x43reditSummaryResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12&\n\x06\x63redit\x18\x02 \x01(\x0b\x32\x16.oi.papi.credit.Credit\"\xc2\x03\n\x0bTransaction\x12\n\n\x02id\x18\x01 \x01(\t\x12\x18\n\x10\x63redit_source_id\x18\x02 \x01(\t\x12\x0f\n\x07user_id\x18\x03 \x01(\t\x12\x45\n\x10transaction_type\x18\x04 \x01(\x0e\x32+.oi.papi.credit.Transaction.TransactionType\x12\x0e\n\x06\x61mount\x18\x05 \x01(\x01\x12\x0e\n\x06reason\x18\x06 \x01(\t\x12\x31\n\rtransacted_on\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x63redit_available\x18\x08 \x01(\x01\x12\x17\n\x0f\x63redit_reserved\x18\t \x01(\x01\x12\x13\n\x0b\x63redit_used\x18\n \x01(\x01\x12 \n\x18\x61lgorithm_computation_id\x18\x0b \x01(\t\"x\n\x0fTransactionType\x12\x1c\n\x18UNKNOWN_TRANSACTION_TYPE\x10\x00\x12\x07\n\x03\x41\x44\x44\x10\x01\x12\n\n\x06REMOVE\x10\x02\x12\n\n\x06REFUND\x10\x03\x12\x0b\n\x07RESERVE\x10\x04\x12\r\n\tUNRESERVE\x10\x05\x12\n\n\x06\x44\x45\x44UCT\x10\x06\"\xae\x02\n\x19\x43reditTransactionsRequest\x12\'\n\npagination\x18\x01 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\x11\n\tsource_id\x18\x02 \x01(\t\x12\x45\n\x10transaction_type\x18\x03 \x01(\x0e\x32+.oi.papi.credit.Transaction.TransactionType\x12\x35\n\x11min_transacted_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11max_transacted_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x18\x61lgorithm_computation_id\x18\x06 \x01(\t\"\x8d\x01\n\x1a\x43reditTransactionsResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\x31\n\x0ctransactions\x18\x03 \x03(\x0b\x32\x1b.oi.papi.credit.Transaction2\x97\x06\n\tCreditApi\x12J\n\x03\x61\x64\x64\x12 .oi.papi.credit.CreditAddRequest\x1a!.oi.papi.credit.CreditAddResponse\x12S\n\x06remove\x12#.oi.papi.credit.CreditRemoveRequest\x1a$.oi.papi.credit.CreditRemoveResponse\x12S\n\x06refund\x12#.oi.papi.credit.CreditRefundRequest\x1a$.oi.papi.credit.CreditRefundResponse\x12z\n\rset_algorithm\x12\x33.oi.papi.credit.CreditAlgorithmMultiplierSetRequest\x1a\x34.oi.papi.credit.CreditAlgorithmMultiplierSetResponse\x12~\n\x0fset_data_source\x12\x34.oi.papi.credit.CreditDataSourceMultiplierSetRequest\x1a\x35.oi.papi.credit.CreditDataSourceMultiplierSetResponse\x12Y\n\x08\x65stimate\x12%.oi.papi.credit.CreditEstimateRequest\x1a&.oi.papi.credit.CreditEstimateResponse\x12V\n\x07summary\x12$.oi.papi.credit.CreditSummaryRequest\x1a%.oi.papi.credit.CreditSummaryResponse\x12\x65\n\x0ctransactions\x12).oi.papi.credit.CreditTransactionsRequest\x1a*.oi.papi.credit.CreditTransactionsResponseP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63redit.proto\x12\x0eoi.papi.credit\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\"E\n\x10\x43reditAddRequest\x12\x11\n\tsource_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x01\x12\x0e\n\x06reason\x18\x03 \x01(\t\"(\n\x11\x43reditAddResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"H\n\x13\x43reditRemoveRequest\x12\x11\n\tsource_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x01\x12\x0e\n\x06reason\x18\x03 \x01(\t\"+\n\x14\x43reditRemoveResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"H\n\x13\x43reditRefundRequest\x12\x11\n\tsource_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x01\x12\x0e\n\x06reason\x18\x03 \x01(\t\"+\n\x14\x43reditRefundResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"\x85\x01\n#CreditAlgorithmMultiplierSetRequest\x12\x1c\n\x14\x61lgorithm_version_id\x18\x01 \x01(\t\x12!\n\x19\x61lgorithm_execution_price\x18\x02 \x01(\x01\x12\x1d\n\x15\x61lgorithm_value_price\x18\x03 \x01(\x01\";\n$CreditAlgorithmMultiplierSetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"Y\n$CreditDataSourceMultiplierSetRequest\x12\x16\n\x0e\x64\x61ta_source_id\x18\x01 \x01(\t\x12\x19\n\x11\x64\x61ta_source_price\x18\x02 \x01(\x01\"<\n%CreditDataSourceMultiplierSetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"9\n\x15\x43reditEstimateRequest\x12 \n\x18\x61lgorithm_computation_id\x18\x01 \x01(\t\"F\n\x16\x43reditEstimateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x17\n\x0f\x63redit_estimate\x18\x02 \x01(\x01\"N\n\x06\x43redit\x12\x11\n\tsource_id\x18\x01 \x01(\t\x12\x11\n\tavailable\x18\x02 \x01(\x01\x12\x10\n\x08reserved\x18\x03 \x01(\x01\x12\x0c\n\x04used\x18\x04 \x01(\x01\")\n\x14\x43reditSummaryRequest\x12\x11\n\tsource_id\x18\x01 \x01(\t\"T\n\x15\x43reditSummaryResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12&\n\x06\x63redit\x18\x02 \x01(\x0b\x32\x16.oi.papi.credit.Credit\"\xc2\x03\n\x0bTransaction\x12\n\n\x02id\x18\x01 \x01(\t\x12\x18\n\x10\x63redit_source_id\x18\x02 \x01(\t\x12\x0f\n\x07user_id\x18\x03 \x01(\t\x12\x45\n\x10transaction_type\x18\x04 \x01(\x0e\x32+.oi.papi.credit.Transaction.TransactionType\x12\x0e\n\x06\x61mount\x18\x05 \x01(\x01\x12\x0e\n\x06reason\x18\x06 \x01(\t\x12\x31\n\rtransacted_on\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x63redit_available\x18\x08 \x01(\x01\x12\x17\n\x0f\x63redit_reserved\x18\t \x01(\x01\x12\x13\n\x0b\x63redit_used\x18\n \x01(\x01\x12 \n\x18\x61lgorithm_computation_id\x18\x0b \x01(\t\"x\n\x0fTransactionType\x12\x1c\n\x18UNKNOWN_TRANSACTION_TYPE\x10\x00\x12\x07\n\x03\x41\x44\x44\x10\x01\x12\n\n\x06REMOVE\x10\x02\x12\n\n\x06REFUND\x10\x03\x12\x0b\n\x07RESERVE\x10\x04\x12\r\n\tUNRESERVE\x10\x05\x12\n\n\x06\x44\x45\x44UCT\x10\x06\"\xae\x02\n\x19\x43reditTransactionsRequest\x12\'\n\npagination\x18\x01 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\x11\n\tsource_id\x18\x02 \x01(\t\x12\x45\n\x10transaction_type\x18\x03 \x01(\x0e\x32+.oi.papi.credit.Transaction.TransactionType\x12\x35\n\x11min_transacted_on\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11max_transacted_on\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x18\x61lgorithm_computation_id\x18\x06 \x01(\t\"\x8d\x01\n\x1a\x43reditTransactionsResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\x31\n\x0ctransactions\x18\x03 \x03(\x0b\x32\x1b.oi.papi.credit.Transaction2\x97\x06\n\tCreditApi\x12J\n\x03\x61\x64\x64\x12 .oi.papi.credit.CreditAddRequest\x1a!.oi.papi.credit.CreditAddResponse\x12S\n\x06remove\x12#.oi.papi.credit.CreditRemoveRequest\x1a$.oi.papi.credit.CreditRemoveResponse\x12S\n\x06refund\x12#.oi.papi.credit.CreditRefundRequest\x1a$.oi.papi.credit.CreditRefundResponse\x12z\n\rset_algorithm\x12\x33.oi.papi.credit.CreditAlgorithmMultiplierSetRequest\x1a\x34.oi.papi.credit.CreditAlgorithmMultiplierSetResponse\x12~\n\x0fset_data_source\x12\x34.oi.papi.credit.CreditDataSourceMultiplierSetRequest\x1a\x35.oi.papi.credit.CreditDataSourceMultiplierSetResponse\x12Y\n\x08\x65stimate\x12%.oi.papi.credit.CreditEstimateRequest\x1a&.oi.papi.credit.CreditEstimateResponse\x12V\n\x07summary\x12$.oi.papi.credit.CreditSummaryRequest\x1a%.oi.papi.credit.CreditSummaryResponse\x12\x65\n\x0ctransactions\x12).oi.papi.credit.CreditTransactionsRequest\x1a*.oi.papi.credit.CreditTransactionsResponseP\x01\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'credit_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_CREDITADDREQUEST']._serialized_start=86
-  _globals['_CREDITADDREQUEST']._serialized_end=155
-  _globals['_CREDITADDRESPONSE']._serialized_start=157
-  _globals['_CREDITADDRESPONSE']._serialized_end=197
-  _globals['_CREDITREMOVEREQUEST']._serialized_start=199
-  _globals['_CREDITREMOVEREQUEST']._serialized_end=271
-  _globals['_CREDITREMOVERESPONSE']._serialized_start=273
-  _globals['_CREDITREMOVERESPONSE']._serialized_end=316
-  _globals['_CREDITREFUNDREQUEST']._serialized_start=318
-  _globals['_CREDITREFUNDREQUEST']._serialized_end=390
-  _globals['_CREDITREFUNDRESPONSE']._serialized_start=392
-  _globals['_CREDITREFUNDRESPONSE']._serialized_end=435
-  _globals['_CREDITALGORITHMMULTIPLIERSETREQUEST']._serialized_start=438
-  _globals['_CREDITALGORITHMMULTIPLIERSETREQUEST']._serialized_end=571
-  _globals['_CREDITALGORITHMMULTIPLIERSETRESPONSE']._serialized_start=573
-  _globals['_CREDITALGORITHMMULTIPLIERSETRESPONSE']._serialized_end=632
-  _globals['_CREDITDATASOURCEMULTIPLIERSETREQUEST']._serialized_start=634
-  _globals['_CREDITDATASOURCEMULTIPLIERSETREQUEST']._serialized_end=723
-  _globals['_CREDITDATASOURCEMULTIPLIERSETRESPONSE']._serialized_start=725
-  _globals['_CREDITDATASOURCEMULTIPLIERSETRESPONSE']._serialized_end=785
-  _globals['_CREDITESTIMATEREQUEST']._serialized_start=788
-  _globals['_CREDITESTIMATEREQUEST']._serialized_end=1133
-  _globals['_CREDITESTIMATEREQUEST_ANALYSISRESOURCES']._serialized_start=967
-  _globals['_CREDITESTIMATEREQUEST_ANALYSISRESOURCES']._serialized_end=1133
-  _globals['_CREDITESTIMATERESPONSE']._serialized_start=1135
-  _globals['_CREDITESTIMATERESPONSE']._serialized_end=1218
-  _globals['_CREDIT']._serialized_start=1220
-  _globals['_CREDIT']._serialized_end=1298
-  _globals['_CREDITSUMMARYREQUEST']._serialized_start=1300
-  _globals['_CREDITSUMMARYREQUEST']._serialized_end=1341
-  _globals['_CREDITSUMMARYRESPONSE']._serialized_start=1343
-  _globals['_CREDITSUMMARYRESPONSE']._serialized_end=1427
-  _globals['_TRANSACTION']._serialized_start=1430
-  _globals['_TRANSACTION']._serialized_end=1880
-  _globals['_TRANSACTION_TRANSACTIONTYPE']._serialized_start=1760
-  _globals['_TRANSACTION_TRANSACTIONTYPE']._serialized_end=1880
-  _globals['_CREDITTRANSACTIONSREQUEST']._serialized_start=1883
-  _globals['_CREDITTRANSACTIONSREQUEST']._serialized_end=2185
-  _globals['_CREDITTRANSACTIONSRESPONSE']._serialized_start=2188
-  _globals['_CREDITTRANSACTIONSRESPONSE']._serialized_end=2329
-  _globals['_CREDITAPI']._serialized_start=2332
-  _globals['_CREDITAPI']._serialized_end=3123
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'credit_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _CREDITADDREQUEST._serialized_start=86
+  _CREDITADDREQUEST._serialized_end=155
+  _CREDITADDRESPONSE._serialized_start=157
+  _CREDITADDRESPONSE._serialized_end=197
+  _CREDITREMOVEREQUEST._serialized_start=199
+  _CREDITREMOVEREQUEST._serialized_end=271
+  _CREDITREMOVERESPONSE._serialized_start=273
+  _CREDITREMOVERESPONSE._serialized_end=316
+  _CREDITREFUNDREQUEST._serialized_start=318
+  _CREDITREFUNDREQUEST._serialized_end=390
+  _CREDITREFUNDRESPONSE._serialized_start=392
+  _CREDITREFUNDRESPONSE._serialized_end=435
+  _CREDITALGORITHMMULTIPLIERSETREQUEST._serialized_start=438
+  _CREDITALGORITHMMULTIPLIERSETREQUEST._serialized_end=571
+  _CREDITALGORITHMMULTIPLIERSETRESPONSE._serialized_start=573
+  _CREDITALGORITHMMULTIPLIERSETRESPONSE._serialized_end=632
+  _CREDITDATASOURCEMULTIPLIERSETREQUEST._serialized_start=634
+  _CREDITDATASOURCEMULTIPLIERSETREQUEST._serialized_end=723
+  _CREDITDATASOURCEMULTIPLIERSETRESPONSE._serialized_start=725
+  _CREDITDATASOURCEMULTIPLIERSETRESPONSE._serialized_end=785
+  _CREDITESTIMATEREQUEST._serialized_start=787
+  _CREDITESTIMATEREQUEST._serialized_end=844
+  _CREDITESTIMATERESPONSE._serialized_start=846
+  _CREDITESTIMATERESPONSE._serialized_end=916
+  _CREDIT._serialized_start=918
+  _CREDIT._serialized_end=996
+  _CREDITSUMMARYREQUEST._serialized_start=998
+  _CREDITSUMMARYREQUEST._serialized_end=1039
+  _CREDITSUMMARYRESPONSE._serialized_start=1041
+  _CREDITSUMMARYRESPONSE._serialized_end=1125
+  _TRANSACTION._serialized_start=1128
+  _TRANSACTION._serialized_end=1578
+  _TRANSACTION_TRANSACTIONTYPE._serialized_start=1458
+  _TRANSACTION_TRANSACTIONTYPE._serialized_end=1578
+  _CREDITTRANSACTIONSREQUEST._serialized_start=1581
+  _CREDITTRANSACTIONSREQUEST._serialized_end=1883
+  _CREDITTRANSACTIONSRESPONSE._serialized_start=1886
+  _CREDITTRANSACTIONSRESPONSE._serialized_end=2027
+  _CREDITAPI._serialized_start=2030
+  _CREDITAPI._serialized_end=2821
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/data_source_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/data_source_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: data_source.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from terrascope_api.models import data_type_pb2 as data__type__pb2
 
 from terrascope_api.models.data_type_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x64\x61ta_source.proto\x12\x07oi.papi\x1a\x0f\x64\x61ta_type.proto\"\xc0\x01\n\nDataSource\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12%\n\ndata_types\x18\x04 \x03(\x0b\x32\x11.oi.papi.DataType\x12\x1c\n\x14\x64\x65livery_lag_seconds\x18\x05 \x01(\x04\x12\x14\n\x0c\x64isplay_name\x18\x06 \x01(\t\x12\x11\n\tindicator\x18\x07 \x01(\t\x12\x15\n\rdata_explorer\x18\x08 \x01(\x08\"#\n\x14\x44\x61taSourceGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"W\n\x15\x44\x61taSourceGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12)\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\x13.oi.papi.DataSource\",\n\x15\x44\x61taSourceListRequest\x12\x13\n\x0bsearch_text\x18\x01 \x01(\t\"X\n\x16\x44\x61taSourceListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12)\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\x13.oi.papi.DataSource2\x9e\x01\n\rDataSourceAPI\x12\x44\n\x03get\x12\x1d.oi.papi.DataSourceGetRequest\x1a\x1e.oi.papi.DataSourceGetResponse\x12G\n\x04list\x12\x1e.oi.papi.DataSourceListRequest\x1a\x1f.oi.papi.DataSourceListResponseP\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x64\x61ta_source.proto\x12\x07oi.papi\x1a\x0f\x64\x61ta_type.proto\"\xa9\x01\n\nDataSource\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12%\n\ndata_types\x18\x04 \x03(\x0b\x32\x11.oi.papi.DataType\x12\x1c\n\x14\x64\x65livery_lag_seconds\x18\x05 \x01(\x04\x12\x14\n\x0c\x64isplay_name\x18\x06 \x01(\t\x12\x11\n\tindicator\x18\x07 \x01(\t\"#\n\x14\x44\x61taSourceGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"W\n\x15\x44\x61taSourceGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12)\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\x13.oi.papi.DataSource\",\n\x15\x44\x61taSourceListRequest\x12\x13\n\x0bsearch_text\x18\x01 \x01(\t\"X\n\x16\x44\x61taSourceListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12)\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\x13.oi.papi.DataSource2\x9e\x01\n\rDataSourceAPI\x12\x44\n\x03get\x12\x1d.oi.papi.DataSourceGetRequest\x1a\x1e.oi.papi.DataSourceGetResponse\x12G\n\x04list\x12\x1e.oi.papi.DataSourceListRequest\x1a\x1f.oi.papi.DataSourceListResponseP\x00\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'data_source_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_DATASOURCE']._serialized_start=48
-  _globals['_DATASOURCE']._serialized_end=240
-  _globals['_DATASOURCEGETREQUEST']._serialized_start=242
-  _globals['_DATASOURCEGETREQUEST']._serialized_end=277
-  _globals['_DATASOURCEGETRESPONSE']._serialized_start=279
-  _globals['_DATASOURCEGETRESPONSE']._serialized_end=366
-  _globals['_DATASOURCELISTREQUEST']._serialized_start=368
-  _globals['_DATASOURCELISTREQUEST']._serialized_end=412
-  _globals['_DATASOURCELISTRESPONSE']._serialized_start=414
-  _globals['_DATASOURCELISTRESPONSE']._serialized_end=502
-  _globals['_DATASOURCEAPI']._serialized_start=505
-  _globals['_DATASOURCEAPI']._serialized_end=663
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'data_source_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _DATASOURCE._serialized_start=48
+  _DATASOURCE._serialized_end=217
+  _DATASOURCEGETREQUEST._serialized_start=219
+  _DATASOURCEGETREQUEST._serialized_end=254
+  _DATASOURCEGETRESPONSE._serialized_start=256
+  _DATASOURCEGETRESPONSE._serialized_end=343
+  _DATASOURCELISTREQUEST._serialized_start=345
+  _DATASOURCELISTREQUEST._serialized_end=389
+  _DATASOURCELISTRESPONSE._serialized_start=391
+  _DATASOURCELISTRESPONSE._serialized_end=479
+  _DATASOURCEAPI._serialized_start=482
+  _DATASOURCEAPI._serialized_end=640
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/data_type_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/data_type_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: data_type.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0f\x64\x61ta_type.proto\x12\x07oi.papi\x1a\x1cgoogle/protobuf/struct.proto\"\x9a\x01\n\x08\x44\x61taType\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x17\n\x0f\x64\x61ta_source_ids\x18\x04 \x03(\t\x12\x13\n\x0bsensor_type\x18\x05 \x01(\t\x12-\n\x0cquery_schema\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x8e\x01\n\x15\x44\x61taTypeCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x13\n\x0bsensor_type\x18\x04 \x01(\t\x12-\n\x0cquery_schema\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"S\n\x16\x44\x61taTypeCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12$\n\tdata_type\x18\x02 \x01(\x0b\x32\x11.oi.papi.DataType\"#\n\x12\x44\x61taTypeGetRequest\x12\r\n\x05names\x18\x01 \x03(\t\"Q\n\x13\x44\x61taTypeGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12%\n\ndata_types\x18\x02 \x03(\x0b\x32\x11.oi.papi.DataType\"*\n\x13\x44\x61taTypeListRequest\x12\x13\n\x0bsearch_text\x18\x01 \x01(\t\"R\n\x14\x44\x61taTypeListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12%\n\ndata_types\x18\x02 \x03(\x0b\x32\x11.oi.papi.DataType2\xdf\x01\n\x0b\x44\x61taTypeAPI\x12I\n\x06\x63reate\x12\x1e.oi.papi.DataTypeCreateRequest\x1a\x1f.oi.papi.DataTypeCreateResponse\x12@\n\x03get\x12\x1b.oi.papi.DataTypeGetRequest\x1a\x1c.oi.papi.DataTypeGetResponse\x12\x43\n\x04list\x12\x1c.oi.papi.DataTypeListRequest\x1a\x1d.oi.papi.DataTypeListResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0f\x64\x61ta_type.proto\x12\x07oi.papi\"k\n\x08\x44\x61taType\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x17\n\x0f\x64\x61ta_source_ids\x18\x04 \x03(\t\x12\x13\n\x0bsensor_type\x18\x05 \x01(\t\"_\n\x15\x44\x61taTypeCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x13\n\x0bsensor_type\x18\x04 \x01(\t\"S\n\x16\x44\x61taTypeCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12$\n\tdata_type\x18\x02 \x01(\x0b\x32\x11.oi.papi.DataType\"!\n\x12\x44\x61taTypeGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"Q\n\x13\x44\x61taTypeGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12%\n\ndata_types\x18\x02 \x03(\x0b\x32\x11.oi.papi.DataType\"*\n\x13\x44\x61taTypeListRequest\x12\x13\n\x0bsearch_text\x18\x01 \x01(\t\"R\n\x14\x44\x61taTypeListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12%\n\ndata_types\x18\x02 \x03(\x0b\x32\x11.oi.papi.DataType2\xdf\x01\n\x0b\x44\x61taTypeAPI\x12I\n\x06\x63reate\x12\x1e.oi.papi.DataTypeCreateRequest\x1a\x1f.oi.papi.DataTypeCreateResponse\x12@\n\x03get\x12\x1b.oi.papi.DataTypeGetRequest\x1a\x1c.oi.papi.DataTypeGetResponse\x12\x43\n\x04list\x12\x1c.oi.papi.DataTypeListRequest\x1a\x1d.oi.papi.DataTypeListResponseb\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'data_type_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_DATATYPE']._serialized_start=59
-  _globals['_DATATYPE']._serialized_end=213
-  _globals['_DATATYPECREATEREQUEST']._serialized_start=216
-  _globals['_DATATYPECREATEREQUEST']._serialized_end=358
-  _globals['_DATATYPECREATERESPONSE']._serialized_start=360
-  _globals['_DATATYPECREATERESPONSE']._serialized_end=443
-  _globals['_DATATYPEGETREQUEST']._serialized_start=445
-  _globals['_DATATYPEGETREQUEST']._serialized_end=480
-  _globals['_DATATYPEGETRESPONSE']._serialized_start=482
-  _globals['_DATATYPEGETRESPONSE']._serialized_end=563
-  _globals['_DATATYPELISTREQUEST']._serialized_start=565
-  _globals['_DATATYPELISTREQUEST']._serialized_end=607
-  _globals['_DATATYPELISTRESPONSE']._serialized_start=609
-  _globals['_DATATYPELISTRESPONSE']._serialized_end=691
-  _globals['_DATATYPEAPI']._serialized_start=694
-  _globals['_DATATYPEAPI']._serialized_end=917
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'data_type_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _DATATYPE._serialized_start=28
+  _DATATYPE._serialized_end=135
+  _DATATYPECREATEREQUEST._serialized_start=137
+  _DATATYPECREATEREQUEST._serialized_end=232
+  _DATATYPECREATERESPONSE._serialized_start=234
+  _DATATYPECREATERESPONSE._serialized_end=317
+  _DATATYPEGETREQUEST._serialized_start=319
+  _DATATYPEGETREQUEST._serialized_end=352
+  _DATATYPEGETRESPONSE._serialized_start=354
+  _DATATYPEGETRESPONSE._serialized_end=435
+  _DATATYPELISTREQUEST._serialized_start=437
+  _DATATYPELISTREQUEST._serialized_end=479
+  _DATATYPELISTRESPONSE._serialized_start=481
+  _DATATYPELISTRESPONSE._serialized_end=563
+  _DATATYPEAPI._serialized_start=566
+  _DATATYPEAPI._serialized_end=789
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/forgot_password_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/algorithm_manifest_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: forgot_password.proto
-# Protobuf Python Version: 5.26.1
+# source: algorithm_manifest.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
 
 from terrascope_api.models.common_models_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x66orgot_password.proto\x12\x07oi.papi\x1a\x13\x63ommon_models.proto\"/\n\x19UserForgotPasswordRequest\x12\x12\n\nuser_email\x18\x01 \x01(\t\"1\n\x1aUserForgotPasswordResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r2o\n\x11\x46orgotPasswordApi\x12Z\n\x0f\x66orgot_password\x12\".oi.papi.UserForgotPasswordRequest\x1a#.oi.papi.UserForgotPasswordResponseP\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x61lgorithm_manifest.proto\x12\x07oi.papi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x13\x63ommon_models.proto\"4\n!AlgorithmManifestSchemaGetRequest\x12\x0f\n\x07version\x18\x01 \x01(\t\"s\n\"AlgorithmManifestSchemaGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\'\n\x06schema\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct2v\n\x14\x41lgorithmManifestApi\x12^\n\x03get\x12*.oi.papi.AlgorithmManifestSchemaGetRequest\x1a+.oi.papi.AlgorithmManifestSchemaGetResponseP\x01\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'forgot_password_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_USERFORGOTPASSWORDREQUEST']._serialized_start=55
-  _globals['_USERFORGOTPASSWORDREQUEST']._serialized_end=102
-  _globals['_USERFORGOTPASSWORDRESPONSE']._serialized_start=104
-  _globals['_USERFORGOTPASSWORDRESPONSE']._serialized_end=153
-  _globals['_FORGOTPASSWORDAPI']._serialized_start=155
-  _globals['_FORGOTPASSWORDAPI']._serialized_end=266
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'algorithm_manifest_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _ALGORITHMMANIFESTSCHEMAGETREQUEST._serialized_start=88
+  _ALGORITHMMANIFESTSCHEMAGETREQUEST._serialized_end=140
+  _ALGORITHMMANIFESTSCHEMAGETRESPONSE._serialized_start=142
+  _ALGORITHMMANIFESTSCHEMAGETRESPONSE._serialized_end=257
+  _ALGORITHMMANIFESTAPI._serialized_start=259
+  _ALGORITHMMANIFESTAPI._serialized_end=377
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/imagery_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/toi_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: imagery.proto
-# Protobuf Python Version: 5.26.1
+# source: toi.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from terrascope_api.models import common_models_pb2 as common__models__pb2
-from terrascope_api.models import aoi_pb2 as aoi__pb2
-try:
-  common__models__pb2 = aoi__pb2.common__models__pb2
-except AttributeError:
-  common__models__pb2 = aoi__pb2.common_models_pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 from terrascope_api.models.common_models_pb2 import *
-from terrascope_api.models.aoi_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rimagery.proto\x12\x0foi.papi.imagery\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x13\x63ommon_models.proto\x1a\taoi.proto\"\xd8\x04\n\x14ImagerySearchRequest\x12(\n\x06\x61oi_id\x18\x01 \x01(\x0b\x32\x16.oi.papi.AOIIdentifierH\x00\x12\x16\n\x0cgeometry_wkb\x18\x02 \x01(\x0cH\x00\x12\x10\n\x06toi_id\x18\x03 \x01(\tH\x01\x12\x45\n\ntime_range\x18\x04 \x01(\x0b\x32/.oi.papi.imagery.ImagerySearchRequest.TimeRangeH\x01\x12\x16\n\x0e\x64\x61ta_source_id\x18\x05 \x01(\t\x12\x19\n\x11product_spec_name\x18\x06 \x01(\t\x12\x34\n\x13\x64\x61ta_source_filters\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\npagination\x18\t \x01(\x0b\x32\x13.oi.papi.Pagination\x12M\n\x0fsampling_config\x18\n \x01(\x0b\x32\x34.oi.papi.imagery.ImagerySearchRequest.SamplingConfig\x1a\x42\n\x0eSamplingConfig\x12\x17\n\x0f\x66requency_hours\x18\x01 \x01(\r\x12\x17\n\x0ftolerance_hours\x18\x02 \x01(\r\x1aj\n\tTimeRange\x12-\n\tstart_utc\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nfinish_utc\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x06\n\x04\x61reaB\x06\n\x04timeJ\x04\x08\x08\x10\t\"\xd5\x02\n\x15ImagerySearchResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12K\n\x07results\x18\x02 \x03(\x0b\x32:.oi.papi.imagery.ImagerySearchResponse.ImagerySearchResult\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\x1a\xb0\x01\n\x13ImagerySearchResult\x12\n\n\x02id\x18\x01 \x01(\t\x12\x19\n\x11provider_scene_id\x18\x02 \x01(\t\x12\x16\n\x0eimage_geom_wkb\x18\x03 \x01(\x0c\x12/\n\x0b\x61\x63quired_ts\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct2e\n\nImageryApi\x12W\n\x06search\x12%.oi.papi.imagery.ImagerySearchRequest\x1a&.oi.papi.imagery.ImagerySearchResponseP\x02P\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ttoi.proto\x12\x07oi.papi\x1a\x13\x63ommon_models.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xb5\x01\n\x07\x43\x61\x64\x65nce\x12-\n\tfrequency\x18\x01 \x01(\x0e\x32\x1a.oi.papi.Cadence.Frequency\x12\r\n\x05value\x18\x02 \x01(\r\"l\n\tFrequency\x12\x15\n\x11UNKNOWN_FREQUENCY\x10\x00\x12\x0c\n\x08MINUTELY\x10\x01\x12\n\n\x06HOURLY\x10\x02\x12\t\n\x05\x44\x41ILY\x10\x03\x12\n\n\x06WEEKLY\x10\x04\x12\x0b\n\x07MONTHLY\x10\x05\x12\n\n\x06YEARLY\x10\x06\"J\n\nRecurrence\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04rule\x18\x02 \x01(\t\x12\"\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x10.oi.papi.Cadence\"\xe6\x01\n\x03TOI\x12\n\n\x02id\x18\x01 \x01(\t\x12/\n\x0bstart_local\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x66inish_local\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x0brecurrences\x18\x04 \x03(\x0b\x32\x13.oi.papi.Recurrence\x12\x31\n\rexclude_dates\x18\x05 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\"\xe7\x01\n\x10TOICreateRequest\x12/\n\x0bstart_local\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x66inish_local\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x0brecurrences\x18\x03 \x03(\x0b\x32\x13.oi.papi.Recurrence\x12\x31\n\rexclude_dates\x18\x04 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\"C\n\x11TOICreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x19\n\x03toi\x18\x02 \x01(\x0b\x32\x0c.oi.papi.TOI\"\x1f\n\x10TOIDeleteRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"(\n\x11TOIDeleteResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"E\n\rTOIGetRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\"q\n\x0eTOIGetResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12!\n\x0btoi_objects\x18\x02 \x03(\x0b\x32\x0c.oi.papi.TOI\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination\"N\n\x0eTOIListRequest\x12\x13\n\x0bsearch_text\x18\x01 \x01(\t\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\"r\n\x0fTOIListResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12!\n\x0btoi_objects\x18\x02 \x03(\x0b\x32\x0c.oi.papi.TOI\x12\'\n\npagination\x18\x03 \x01(\x0b\x32\x13.oi.papi.Pagination2\xfd\x01\n\x06TOIApi\x12?\n\x06\x63reate\x12\x19.oi.papi.TOICreateRequest\x1a\x1a.oi.papi.TOICreateResponse\x12?\n\x06\x64\x65lete\x12\x19.oi.papi.TOIDeleteRequest\x1a\x1a.oi.papi.TOIDeleteResponse\x12\x36\n\x03get\x12\x16.oi.papi.TOIGetRequest\x1a\x17.oi.papi.TOIGetResponse\x12\x39\n\x04list\x12\x17.oi.papi.TOIListRequest\x1a\x18.oi.papi.TOIListResponseP\x00\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'imagery_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_IMAGERYSEARCHREQUEST']._serialized_start=130
-  _globals['_IMAGERYSEARCHREQUEST']._serialized_end=730
-  _globals['_IMAGERYSEARCHREQUEST_SAMPLINGCONFIG']._serialized_start=534
-  _globals['_IMAGERYSEARCHREQUEST_SAMPLINGCONFIG']._serialized_end=600
-  _globals['_IMAGERYSEARCHREQUEST_TIMERANGE']._serialized_start=602
-  _globals['_IMAGERYSEARCHREQUEST_TIMERANGE']._serialized_end=708
-  _globals['_IMAGERYSEARCHRESPONSE']._serialized_start=733
-  _globals['_IMAGERYSEARCHRESPONSE']._serialized_end=1074
-  _globals['_IMAGERYSEARCHRESPONSE_IMAGERYSEARCHRESULT']._serialized_start=898
-  _globals['_IMAGERYSEARCHRESPONSE_IMAGERYSEARCHRESULT']._serialized_end=1074
-  _globals['_IMAGERYAPI']._serialized_start=1076
-  _globals['_IMAGERYAPI']._serialized_end=1177
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'toi_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _CADENCE._serialized_start=77
+  _CADENCE._serialized_end=258
+  _CADENCE_FREQUENCY._serialized_start=150
+  _CADENCE_FREQUENCY._serialized_end=258
+  _RECURRENCE._serialized_start=260
+  _RECURRENCE._serialized_end=334
+  _TOI._serialized_start=337
+  _TOI._serialized_end=567
+  _TOICREATEREQUEST._serialized_start=570
+  _TOICREATEREQUEST._serialized_end=801
+  _TOICREATERESPONSE._serialized_start=803
+  _TOICREATERESPONSE._serialized_end=870
+  _TOIDELETEREQUEST._serialized_start=872
+  _TOIDELETEREQUEST._serialized_end=903
+  _TOIDELETERESPONSE._serialized_start=905
+  _TOIDELETERESPONSE._serialized_end=945
+  _TOIGETREQUEST._serialized_start=947
+  _TOIGETREQUEST._serialized_end=1016
+  _TOIGETRESPONSE._serialized_start=1018
+  _TOIGETRESPONSE._serialized_end=1131
+  _TOILISTREQUEST._serialized_start=1133
+  _TOILISTREQUEST._serialized_end=1211
+  _TOILISTRESPONSE._serialized_start=1213
+  _TOILISTRESPONSE._serialized_end=1327
+  _TOIAPI._serialized_start=1330
+  _TOIAPI._serialized_end=1583
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/permission_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/permission_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: permission.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from terrascope_api.models import common_models_pb2 as common__models__pb2
 
 from terrascope_api.models.common_models_pb2 import *
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10permission.proto\x12\x12oi.papi.permission\x1a\x13\x63ommon_models.proto\"\xab\x04\n\nPermission\x12\x42\n\rresource_type\x18\x01 \x01(\x0e\x32+.oi.papi.permission.Permission.ResourceType\x12\x14\n\x0cresource_ids\x18\x02 \x03(\t\x12\x13\n\x0bsubject_ids\x18\x03 \x03(\t\x12G\n\x10permission_types\x18\x04 \x03(\x0e\x32-.oi.papi.permission.Permission.PermissionType\"\xda\x01\n\x0cResourceType\x12$\n UNKNOWN_PERMISSION_RESOURCE_TYPE\x10\x00\x12\r\n\tALGORITHM\x10\x01\x12\x19\n\x15\x41LGORITHM_COMPUTATION\x10\x02\x12\x14\n\x10\x41LGORITHM_CONFIG\x10\x03\x12\x0c\n\x08\x41NALYSIS\x10\x04\x12\x18\n\x14\x41NALYSIS_COMPUTATION\x10\x05\x12\x13\n\x0f\x41NALYSIS_CONFIG\x10\x06\x12\x12\n\x0e\x41OI_COLLECTION\x10\x07\x12\n\n\x06RESULT\x10\x08\x12\x07\n\x03TOI\x10\t\"M\n\x0ePermissionType\x12\x1b\n\x17UNKNOWN_PERMISSION_TYPE\x10\x00\x12\x08\n\x04READ\x10\x01\x12\t\n\x05WRITE\x10\x02\x12\t\n\x05\x41\x44MIN\x10\x03\"9\n\x0e\x43ollectionType\x12\x1b\n\x17UNKNOWN_COLLECTION_TYPE\x10\x00\x12\n\n\x06PUBLIC\x10\x01\"N\n\x17PermissionCreateRequest\x12\x33\n\x0bpermissions\x18\x01 \x03(\x0b\x32\x1e.oi.papi.permission.Permission\"/\n\x18PermissionCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\"N\n\x17PermissionDeleteRequest\x12\x33\n\x0bpermissions\x18\x01 \x03(\x0b\x32\x1e.oi.papi.permission.Permission\"/\n\x18PermissionDeleteResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r2\xd9\x01\n\rPermissionApi\x12\x63\n\x06\x63reate\x12+.oi.papi.permission.PermissionCreateRequest\x1a,.oi.papi.permission.PermissionCreateResponse\x12\x63\n\x06\x64\x65lete\x12+.oi.papi.permission.PermissionDeleteRequest\x1a,.oi.papi.permission.PermissionDeleteResponseP\x00\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'permission_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_PERMISSION']._serialized_start=62
-  _globals['_PERMISSION']._serialized_end=617
-  _globals['_PERMISSION_RESOURCETYPE']._serialized_start=261
-  _globals['_PERMISSION_RESOURCETYPE']._serialized_end=479
-  _globals['_PERMISSION_PERMISSIONTYPE']._serialized_start=481
-  _globals['_PERMISSION_PERMISSIONTYPE']._serialized_end=558
-  _globals['_PERMISSION_COLLECTIONTYPE']._serialized_start=560
-  _globals['_PERMISSION_COLLECTIONTYPE']._serialized_end=617
-  _globals['_PERMISSIONCREATEREQUEST']._serialized_start=619
-  _globals['_PERMISSIONCREATEREQUEST']._serialized_end=697
-  _globals['_PERMISSIONCREATERESPONSE']._serialized_start=699
-  _globals['_PERMISSIONCREATERESPONSE']._serialized_end=746
-  _globals['_PERMISSIONDELETEREQUEST']._serialized_start=748
-  _globals['_PERMISSIONDELETEREQUEST']._serialized_end=826
-  _globals['_PERMISSIONDELETERESPONSE']._serialized_start=828
-  _globals['_PERMISSIONDELETERESPONSE']._serialized_end=875
-  _globals['_PERMISSIONAPI']._serialized_start=878
-  _globals['_PERMISSIONAPI']._serialized_end=1095
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'permission_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _PERMISSION._serialized_start=62
+  _PERMISSION._serialized_end=617
+  _PERMISSION_RESOURCETYPE._serialized_start=261
+  _PERMISSION_RESOURCETYPE._serialized_end=479
+  _PERMISSION_PERMISSIONTYPE._serialized_start=481
+  _PERMISSION_PERMISSIONTYPE._serialized_end=558
+  _PERMISSION_COLLECTIONTYPE._serialized_start=560
+  _PERMISSION_COLLECTIONTYPE._serialized_end=617
+  _PERMISSIONCREATEREQUEST._serialized_start=619
+  _PERMISSIONCREATEREQUEST._serialized_end=697
+  _PERMISSIONCREATERESPONSE._serialized_start=699
+  _PERMISSIONCREATERESPONSE._serialized_end=746
+  _PERMISSIONDELETEREQUEST._serialized_start=748
+  _PERMISSIONDELETEREQUEST._serialized_end=826
+  _PERMISSIONDELETERESPONSE._serialized_start=828
+  _PERMISSIONDELETERESPONSE._serialized_end=875
+  _PERMISSIONAPI._serialized_start=878
+  _PERMISSIONAPI._serialized_end=1095
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/system_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/system_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: system.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0csystem.proto\x12\x07oi.papi\x1a\x1cgoogle/api/annotations.proto\"\r\n\x0bPingRequest\"#\n\x0cPingResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r2a\n\tSystemApi\x12T\n\x08get_ping\x12\x14.oi.papi.PingRequest\x1a\x15.oi.papi.PingResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/systemapi/get_pingb\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'system_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_SYSTEMAPI'].methods_by_name['get_ping']._loaded_options = None
-  _globals['_SYSTEMAPI'].methods_by_name['get_ping']._serialized_options = b'\202\323\344\223\002\025\022\023/systemapi/get_ping'
-  _globals['_PINGREQUEST']._serialized_start=55
-  _globals['_PINGREQUEST']._serialized_end=68
-  _globals['_PINGRESPONSE']._serialized_start=70
-  _globals['_PINGRESPONSE']._serialized_end=105
-  _globals['_SYSTEMAPI']._serialized_start=107
-  _globals['_SYSTEMAPI']._serialized_end=204
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'system_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _SYSTEMAPI.methods_by_name['get_ping']._options = None
+  _SYSTEMAPI.methods_by_name['get_ping']._serialized_options = b'\202\323\344\223\002\025\022\023/systemapi/get_ping'
+  _PINGREQUEST._serialized_start=55
+  _PINGREQUEST._serialized_end=68
+  _PINGRESPONSE._serialized_start=70
+  _PINGRESPONSE._serialized_end=105
+  _SYSTEMAPI._serialized_start=107
+  _SYSTEMAPI._serialized_end=204
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/tile_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/tile_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tile.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from terrascope_api.models import common_models_pb2 as common__models__pb2
 
-from terrascope_api.models.common_models_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ntile.proto\x12\x0coi.papi.tile\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13\x63ommon_models.proto\"D\n\x06\x42ounds\x12\r\n\x05x_min\x18\x01 \x01(\x02\x12\r\n\x05y_min\x18\x02 \x01(\x02\x12\r\n\x05x_max\x18\x03 \x01(\x02\x12\r\n\x05y_max\x18\x04 \x01(\x02\"&\n\nTileMatrix\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04zoom\x18\x02 \x01(\x05\"T\n\x0eTileAccessInfo\x12\x14\n\x0curl_template\x18\x01 \x01(\t\x12,\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xd5\x01\n\x07TileSet\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12$\n\x06\x62ounds\x18\x03 \x01(\x0b\x32\x14.oi.papi.tile.Bounds\x12*\n\x08matrices\x18\x04 \x03(\x0b\x32\x18.oi.papi.tile.TileMatrix\x12\x31\n\x0btile_access\x18\x05 \x01(\x0b\x32\x1c.oi.papi.tile.TileAccessInfo\x12+\n\x07\x66rom_ts\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb2\x01\n\x12TileSetListRequest\x12\x11\n\tsearch_id\x18\x01 \x01(\t\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination\x12\x30\n\x0ctile_ts_from\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ntile_ts_to\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"h\n\x13TileSetListResponse\x12(\n\ttile_sets\x18\x01 \x03(\x0b\x32\x15.oi.papi.tile.TileSet\x12\'\n\npagination\x18\x02 \x01(\x0b\x32\x13.oi.papi.Pagination2V\n\x07TileApi\x12K\n\x04list\x12 .oi.papi.tile.TileSetListRequest\x1a!.oi.papi.tile.TileSetListResponseP\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ntile.proto\x12\x0coi.papi.tile\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"D\n\x06\x42ounds\x12\r\n\x05x_min\x18\x01 \x01(\x02\x12\r\n\x05y_min\x18\x02 \x01(\x02\x12\r\n\x05x_max\x18\x03 \x01(\x02\x12\r\n\x05y_max\x18\x04 \x01(\x02\"&\n\nTileMatrix\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04zoom\x18\x02 \x01(\x05\"T\n\x0eTileAccessInfo\x12\x14\n\x0curl_template\x18\x01 \x01(\t\x12,\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xd5\x01\n\x07TileSet\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12$\n\x06\x62ounds\x18\x03 \x01(\x0b\x32\x14.oi.papi.tile.Bounds\x12*\n\x08matrices\x18\x04 \x03(\x0b\x32\x18.oi.papi.tile.TileMatrix\x12\x31\n\x0btile_access\x18\x05 \x01(\x0b\x32\x1c.oi.papi.tile.TileAccessInfo\x12+\n\x07\x66rom_ts\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\'\n\x12TileSetListRequest\x12\x11\n\tsearch_id\x18\x01 \x01(\t\"?\n\x13TileSetListResponse\x12(\n\ttile_sets\x18\x01 \x03(\x0b\x32\x15.oi.papi.tile.TileSet2V\n\x07TileApi\x12K\n\x04list\x12 .oi.papi.tile.TileSetListRequest\x1a!.oi.papi.tile.TileSetListResponseb\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tile_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_BOUNDS']._serialized_start=112
-  _globals['_BOUNDS']._serialized_end=180
-  _globals['_TILEMATRIX']._serialized_start=182
-  _globals['_TILEMATRIX']._serialized_end=220
-  _globals['_TILEACCESSINFO']._serialized_start=222
-  _globals['_TILEACCESSINFO']._serialized_end=306
-  _globals['_TILESET']._serialized_start=309
-  _globals['_TILESET']._serialized_end=522
-  _globals['_TILESETLISTREQUEST']._serialized_start=525
-  _globals['_TILESETLISTREQUEST']._serialized_end=703
-  _globals['_TILESETLISTRESPONSE']._serialized_start=705
-  _globals['_TILESETLISTRESPONSE']._serialized_end=809
-  _globals['_TILEAPI']._serialized_start=811
-  _globals['_TILEAPI']._serialized_end=897
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tile_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _BOUNDS._serialized_start=91
+  _BOUNDS._serialized_end=159
+  _TILEMATRIX._serialized_start=161
+  _TILEMATRIX._serialized_end=199
+  _TILEACCESSINFO._serialized_start=201
+  _TILEACCESSINFO._serialized_end=285
+  _TILESET._serialized_start=288
+  _TILESET._serialized_end=501
+  _TILESETLISTREQUEST._serialized_start=503
+  _TILESETLISTREQUEST._serialized_end=542
+  _TILESETLISTRESPONSE._serialized_start=544
+  _TILESETLISTRESPONSE._serialized_end=607
+  _TILEAPI._serialized_start=609
+  _TILEAPI._serialized_end=695
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/models/token_pb2.py` & `terrascope-api-1.0.5/src/py/terrascope_api/models/token_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: token.proto
-# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from terrascope_api.models import common_models_pb2 as common__models__pb2
 
 from terrascope_api.models.common_models_pb2 import *
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btoken.proto\x12\x07oi.papi\x1a\x13\x63ommon_models.proto\"C\n\x12TokenCreateRequest\x12\x18\n\x10\x64uration_minutes\x18\x01 \x01(\x05\x12\x13\n\x0b\x66or_user_id\x18\x02 \x01(\t\"=\n\x13TokenCreateResponse\x12\x13\n\x0bstatus_code\x18\x01 \x01(\r\x12\x11\n\tjwt_token\x18\x02 \x01(\t2O\n\x08TokenApi\x12\x43\n\x06\x63reate\x12\x1b.oi.papi.TokenCreateRequest\x1a\x1c.oi.papi.TokenCreateResponseP\x00\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'token_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_TOKENCREATEREQUEST']._serialized_start=45
-  _globals['_TOKENCREATEREQUEST']._serialized_end=112
-  _globals['_TOKENCREATERESPONSE']._serialized_start=114
-  _globals['_TOKENCREATERESPONSE']._serialized_end=175
-  _globals['_TOKENAPI']._serialized_start=177
-  _globals['_TOKENAPI']._serialized_end=256
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'token_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _TOKENCREATEREQUEST._serialized_start=45
+  _TOKENCREATEREQUEST._serialized_end=112
+  _TOKENCREATERESPONSE._serialized_start=114
+  _TOKENCREATERESPONSE._serialized_end=175
+  _TOKENAPI._serialized_start=177
+  _TOKENAPI._serialized_end=256
 # @@protoc_insertion_point(module_scope)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/__init__.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,30 +3,23 @@
 from . import algorithm_manifest_pb2_grpc as algorithm_manifest
 from . import algorithm_pb2_grpc as algorithm
 from . import algorithm_version_pb2_grpc as algorithm_version
 from . import analysis_computation_pb2_grpc as analysis_computation
 from . import analysis_config_pb2_grpc as analysis_config
 from . import analysis_pb2_grpc as analysis
 from . import analysis_version_pb2_grpc as analysis_version
-from . import aoi_catalog_pb2_grpc as aoi_catalog
 from . import aoi_collection_pb2_grpc as aoi_collection
-from . import aoi_export_pb2_grpc as aoi_export
 from . import aoi_pb2_grpc as aoi
 from . import aoi_transaction_pb2_grpc as aoi_transaction
 from . import aoi_version_pb2_grpc as aoi_version
 from . import common_models_pb2_grpc as common_models
 from . import credit_pb2_grpc as credit
-from . import data_search_pb2_grpc as data_search
 from . import data_source_pb2_grpc as data_source
 from . import data_type_pb2_grpc as data_type
-from . import forgot_password_pb2_grpc as forgot_password
-from . import imagery_pb2_grpc as imagery
-from . import notification_pb2_grpc as notification
 from . import permission_pb2_grpc as permission
-from . import project_pb2_grpc as project
 from . import result_pb2_grpc as result
 from . import system_pb2_grpc as system
 from . import tile_pb2_grpc as tile
 from . import toi_pb2_grpc as toi
 from . import token_pb2_grpc as token
 from . import user_collection_pb2_grpc as user_collection
 from . import user_pb2_grpc as user
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/algorithm_computation_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/algorithm_computation_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
 from terrascope_api.models import algorithm_computation_pb2 as algorithm__computation__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in algorithm_computation_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
-
 
 class AlgorithmComputationApiStub(object):
     """*************************************************************
     Computation Interface
     *************************************************************
 
     """
@@ -43,30 +18,30 @@
         Args:
             channel: A grpc.Channel.
         """
         self.create = channel.unary_unary(
                 '/oi.papi.AlgorithmComputationApi/create',
                 request_serializer=algorithm__computation__pb2.AlgorithmComputationCreateRequest.SerializeToString,
                 response_deserializer=algorithm__computation__pb2.AlgorithmComputationCreateResponse.FromString,
-                _registered_method=True)
+                )
         self.run = channel.unary_unary(
                 '/oi.papi.AlgorithmComputationApi/run',
                 request_serializer=algorithm__computation__pb2.AlgorithmComputationRunRequest.SerializeToString,
                 response_deserializer=algorithm__computation__pb2.AlgorithmComputationRunResponse.FromString,
-                _registered_method=True)
+                )
         self.get = channel.unary_unary(
                 '/oi.papi.AlgorithmComputationApi/get',
                 request_serializer=algorithm__computation__pb2.AlgorithmComputationGetRequest.SerializeToString,
                 response_deserializer=algorithm__computation__pb2.AlgorithmComputationGetResponse.FromString,
-                _registered_method=True)
+                )
         self.list = channel.unary_unary(
                 '/oi.papi.AlgorithmComputationApi/list',
                 request_serializer=algorithm__computation__pb2.AlgorithmComputationListRequest.SerializeToString,
                 response_deserializer=algorithm__computation__pb2.AlgorithmComputationListResponse.FromString,
-                _registered_method=True)
+                )
 
 
 class AlgorithmComputationApiServicer(object):
     """*************************************************************
     Computation Interface
     *************************************************************
 
@@ -153,103 +128,63 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmComputationApi/create',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmComputationApi/create',
             algorithm__computation__pb2.AlgorithmComputationCreateRequest.SerializeToString,
             algorithm__computation__pb2.AlgorithmComputationCreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def run(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmComputationApi/run',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmComputationApi/run',
             algorithm__computation__pb2.AlgorithmComputationRunRequest.SerializeToString,
             algorithm__computation__pb2.AlgorithmComputationRunResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmComputationApi/get',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmComputationApi/get',
             algorithm__computation__pb2.AlgorithmComputationGetRequest.SerializeToString,
             algorithm__computation__pb2.AlgorithmComputationGetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmComputationApi/list',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmComputationApi/list',
             algorithm__computation__pb2.AlgorithmComputationListRequest.SerializeToString,
             algorithm__computation__pb2.AlgorithmComputationListResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/algorithm_config_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/algorithm_config_pb2_grpc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,58 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
 from terrascope_api.models import algorithm_config_pb2 as algorithm__config__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in algorithm_config_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
-
 
 class AlgorithmConfigApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.create = channel.unary_unary(
                 '/oi.papi.AlgorithmConfigApi/create',
                 request_serializer=algorithm__config__pb2.AlgorithmConfigCreateRequest.SerializeToString,
                 response_deserializer=algorithm__config__pb2.AlgorithmConfigCreateResponse.FromString,
-                _registered_method=True)
+                )
         self.get = channel.unary_unary(
                 '/oi.papi.AlgorithmConfigApi/get',
                 request_serializer=algorithm__config__pb2.AlgorithmConfigGetRequest.SerializeToString,
                 response_deserializer=algorithm__config__pb2.AlgorithmConfigGetResponse.FromString,
-                _registered_method=True)
+                )
         self.list = channel.unary_unary(
                 '/oi.papi.AlgorithmConfigApi/list',
                 request_serializer=algorithm__config__pb2.AlgorithmConfigListRequest.SerializeToString,
                 response_deserializer=algorithm__config__pb2.AlgorithmConfigListResponse.FromString,
-                _registered_method=True)
+                )
         self.update = channel.unary_unary(
                 '/oi.papi.AlgorithmConfigApi/update',
                 request_serializer=algorithm__config__pb2.AlgorithmConfigUpdateRequest.SerializeToString,
                 response_deserializer=algorithm__config__pb2.AlgorithmConfigUpdateResponse.FromString,
-                _registered_method=True)
+                )
         self.deprecate = channel.unary_unary(
                 '/oi.papi.AlgorithmConfigApi/deprecate',
                 request_serializer=algorithm__config__pb2.AlgorithmConfigDeprecateRequest.SerializeToString,
                 response_deserializer=algorithm__config__pb2.AlgorithmConfigDeprecateResponse.FromString,
-                _registered_method=True)
+                )
         self.deactivate = channel.unary_unary(
                 '/oi.papi.AlgorithmConfigApi/deactivate',
                 request_serializer=algorithm__config__pb2.AlgorithmConfigDeactivateRequest.SerializeToString,
                 response_deserializer=algorithm__config__pb2.AlgorithmConfigDeactivateResponse.FromString,
-                _registered_method=True)
+                )
         self.delete = channel.unary_unary(
                 '/oi.papi.AlgorithmConfigApi/delete',
                 request_serializer=algorithm__config__pb2.AlgorithmConfigDeleteRequest.SerializeToString,
                 response_deserializer=algorithm__config__pb2.AlgorithmConfigDeleteResponse.FromString,
-                _registered_method=True)
+                )
 
 
 class AlgorithmConfigApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def create(self, request, context):
         """
@@ -198,184 +173,114 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmConfigApi/create',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmConfigApi/create',
             algorithm__config__pb2.AlgorithmConfigCreateRequest.SerializeToString,
             algorithm__config__pb2.AlgorithmConfigCreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmConfigApi/get',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmConfigApi/get',
             algorithm__config__pb2.AlgorithmConfigGetRequest.SerializeToString,
             algorithm__config__pb2.AlgorithmConfigGetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmConfigApi/list',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmConfigApi/list',
             algorithm__config__pb2.AlgorithmConfigListRequest.SerializeToString,
             algorithm__config__pb2.AlgorithmConfigListResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def update(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmConfigApi/update',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmConfigApi/update',
             algorithm__config__pb2.AlgorithmConfigUpdateRequest.SerializeToString,
             algorithm__config__pb2.AlgorithmConfigUpdateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def deprecate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmConfigApi/deprecate',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmConfigApi/deprecate',
             algorithm__config__pb2.AlgorithmConfigDeprecateRequest.SerializeToString,
             algorithm__config__pb2.AlgorithmConfigDeprecateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def deactivate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmConfigApi/deactivate',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmConfigApi/deactivate',
             algorithm__config__pb2.AlgorithmConfigDeactivateRequest.SerializeToString,
             algorithm__config__pb2.AlgorithmConfigDeactivateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def delete(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmConfigApi/delete',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmConfigApi/delete',
             algorithm__config__pb2.AlgorithmConfigDeleteRequest.SerializeToString,
             algorithm__config__pb2.AlgorithmConfigDeleteResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/algorithm_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/algorithm_pb2_grpc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,43 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
 from terrascope_api.models import algorithm_pb2 as algorithm__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in algorithm_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
-
 
 class AlgorithmApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.create = channel.unary_unary(
                 '/oi.papi.AlgorithmApi/create',
                 request_serializer=algorithm__pb2.AlgorithmCreateRequest.SerializeToString,
                 response_deserializer=algorithm__pb2.AlgorithmCreateResponse.FromString,
-                _registered_method=True)
+                )
         self.update = channel.unary_unary(
                 '/oi.papi.AlgorithmApi/update',
                 request_serializer=algorithm__pb2.AlgorithmUpdateRequest.SerializeToString,
                 response_deserializer=algorithm__pb2.AlgorithmUpdateResponse.FromString,
-                _registered_method=True)
+                )
         self.get = channel.unary_unary(
                 '/oi.papi.AlgorithmApi/get',
                 request_serializer=algorithm__pb2.AlgorithmGetRequest.SerializeToString,
                 response_deserializer=algorithm__pb2.AlgorithmGetResponse.FromString,
-                _registered_method=True)
+                )
         self.list = channel.unary_unary(
                 '/oi.papi.AlgorithmApi/list',
                 request_serializer=algorithm__pb2.AlgorithmListRequest.SerializeToString,
                 response_deserializer=algorithm__pb2.AlgorithmListResponse.FromString,
-                _registered_method=True)
+                )
 
 
 class AlgorithmApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def create(self, request, context):
         """
@@ -141,103 +116,63 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmApi/create',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmApi/create',
             algorithm__pb2.AlgorithmCreateRequest.SerializeToString,
             algorithm__pb2.AlgorithmCreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def update(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmApi/update',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmApi/update',
             algorithm__pb2.AlgorithmUpdateRequest.SerializeToString,
             algorithm__pb2.AlgorithmUpdateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmApi/get',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmApi/get',
             algorithm__pb2.AlgorithmGetRequest.SerializeToString,
             algorithm__pb2.AlgorithmGetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmApi/list',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmApi/list',
             algorithm__pb2.AlgorithmListRequest.SerializeToString,
             algorithm__pb2.AlgorithmListResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/algorithm_version_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/algorithm_version_pb2_grpc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,53 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
 from terrascope_api.models import algorithm_version_pb2 as algorithm__version__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in algorithm_version_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
-
 
 class AlgorithmVersionApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.create = channel.unary_unary(
                 '/oi.papi.AlgorithmVersionApi/create',
                 request_serializer=algorithm__version__pb2.AlgorithmVersionCreateRequest.SerializeToString,
                 response_deserializer=algorithm__version__pb2.AlgorithmVersionCreateResponse.FromString,
-                _registered_method=True)
+                )
         self.get = channel.unary_unary(
                 '/oi.papi.AlgorithmVersionApi/get',
                 request_serializer=algorithm__version__pb2.AlgorithmVersionGetRequest.SerializeToString,
                 response_deserializer=algorithm__version__pb2.AlgorithmVersionGetResponse.FromString,
-                _registered_method=True)
+                )
         self.list = channel.unary_unary(
                 '/oi.papi.AlgorithmVersionApi/list',
                 request_serializer=algorithm__version__pb2.AlgorithmVersionListRequest.SerializeToString,
                 response_deserializer=algorithm__version__pb2.AlgorithmVersionListResponse.FromString,
-                _registered_method=True)
+                )
         self.deprecate = channel.unary_unary(
                 '/oi.papi.AlgorithmVersionApi/deprecate',
                 request_serializer=algorithm__version__pb2.AlgorithmVersionDeprecateRequest.SerializeToString,
                 response_deserializer=algorithm__version__pb2.AlgorithmVersionDeprecateResponse.FromString,
-                _registered_method=True)
+                )
         self.deactivate = channel.unary_unary(
                 '/oi.papi.AlgorithmVersionApi/deactivate',
                 request_serializer=algorithm__version__pb2.AlgorithmVersionDeactivateRequest.SerializeToString,
                 response_deserializer=algorithm__version__pb2.AlgorithmVersionDeactivateResponse.FromString,
-                _registered_method=True)
+                )
         self.activate = channel.unary_unary(
                 '/oi.papi.AlgorithmVersionApi/activate',
                 request_serializer=algorithm__version__pb2.AlgorithmVersionActivateRequest.SerializeToString,
                 response_deserializer=algorithm__version__pb2.AlgorithmVersionActivateResponse.FromString,
-                _registered_method=True)
+                )
 
 
 class AlgorithmVersionApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def create(self, request, context):
         """
@@ -184,157 +159,97 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmVersionApi/create',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmVersionApi/create',
             algorithm__version__pb2.AlgorithmVersionCreateRequest.SerializeToString,
             algorithm__version__pb2.AlgorithmVersionCreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmVersionApi/get',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmVersionApi/get',
             algorithm__version__pb2.AlgorithmVersionGetRequest.SerializeToString,
             algorithm__version__pb2.AlgorithmVersionGetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmVersionApi/list',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmVersionApi/list',
             algorithm__version__pb2.AlgorithmVersionListRequest.SerializeToString,
             algorithm__version__pb2.AlgorithmVersionListResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def deprecate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmVersionApi/deprecate',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmVersionApi/deprecate',
             algorithm__version__pb2.AlgorithmVersionDeprecateRequest.SerializeToString,
             algorithm__version__pb2.AlgorithmVersionDeprecateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def deactivate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmVersionApi/deactivate',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmVersionApi/deactivate',
             algorithm__version__pb2.AlgorithmVersionDeactivateRequest.SerializeToString,
             algorithm__version__pb2.AlgorithmVersionDeactivateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def activate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AlgorithmVersionApi/activate',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AlgorithmVersionApi/activate',
             algorithm__version__pb2.AlgorithmVersionActivateRequest.SerializeToString,
             algorithm__version__pb2.AlgorithmVersionActivateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/analysis_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/analysis_config_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,196 +1,140 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
-from terrascope_api.models import analysis_pb2 as analysis__pb2
+from terrascope_api.models import analysis_config_pb2 as analysis__config__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in analysis_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
 
-
-class AnalysisApiStub(object):
+class AnalysisConfigApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.create = channel.unary_unary(
-                '/oi.papi.AnalysisApi/create',
-                request_serializer=analysis__pb2.AnalysisCreateRequest.SerializeToString,
-                response_deserializer=analysis__pb2.AnalysisCreateResponse.FromString,
-                _registered_method=True)
+                '/oi.papi.AnalysisConfigApi/create',
+                request_serializer=analysis__config__pb2.AnalysisConfigCreateRequest.SerializeToString,
+                response_deserializer=analysis__config__pb2.AnalysisConfigCreateResponse.FromString,
+                )
         self.get = channel.unary_unary(
-                '/oi.papi.AnalysisApi/get',
-                request_serializer=analysis__pb2.AnalysisGetRequest.SerializeToString,
-                response_deserializer=analysis__pb2.AnalysisGetResponse.FromString,
-                _registered_method=True)
+                '/oi.papi.AnalysisConfigApi/get',
+                request_serializer=analysis__config__pb2.AnalysisConfigGetRequest.SerializeToString,
+                response_deserializer=analysis__config__pb2.AnalysisConfigGetResponse.FromString,
+                )
         self.list = channel.unary_unary(
-                '/oi.papi.AnalysisApi/list',
-                request_serializer=analysis__pb2.AnalysisListRequest.SerializeToString,
-                response_deserializer=analysis__pb2.AnalysisListResponse.FromString,
-                _registered_method=True)
+                '/oi.papi.AnalysisConfigApi/list',
+                request_serializer=analysis__config__pb2.AnalysisConfigListRequest.SerializeToString,
+                response_deserializer=analysis__config__pb2.AnalysisConfigListResponse.FromString,
+                )
 
 
-class AnalysisApiServicer(object):
+class AnalysisConfigApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def create(self, request, context):
         """
-        Create a top level Analysis object.
-        This object is lightweight and is used to connect all versions of an Analysis together.
-        Once an Analysis has been created, an AnalysisVersion must be created using a manifest.
-        Next an AnalysisConfig may be created to specify a particular configuration of an AnalysisVersion, which can be used in an AnalysisComputation.
+        Creates a configuration of the specified AnalysisVersion, including concrete values for all of the Analysis parameters.
+        This configuration is stored in the system and the analysis_config is returned to the user.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def get(self, request, context):
         """
-        Retrieve the metadata of a particular analysis.
+        Retrieve the metadata of a particular AnalysisConfig.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def list(self, request, context):
         """
-        Retrieve the metadata for all Analyses that this user has access to and that match the provided search filters, if any.
+        Retrieve the metadata for all AnalysisConfigs that this user has access to and that match the provided search filters.
+        By default, deactivated AnalysisConfigs are not returned. Setting include_deactivated to true will also return any AnalysisConfigs that had been deactivated.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_AnalysisApiServicer_to_server(servicer, server):
+def add_AnalysisConfigApiServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'create': grpc.unary_unary_rpc_method_handler(
                     servicer.create,
-                    request_deserializer=analysis__pb2.AnalysisCreateRequest.FromString,
-                    response_serializer=analysis__pb2.AnalysisCreateResponse.SerializeToString,
+                    request_deserializer=analysis__config__pb2.AnalysisConfigCreateRequest.FromString,
+                    response_serializer=analysis__config__pb2.AnalysisConfigCreateResponse.SerializeToString,
             ),
             'get': grpc.unary_unary_rpc_method_handler(
                     servicer.get,
-                    request_deserializer=analysis__pb2.AnalysisGetRequest.FromString,
-                    response_serializer=analysis__pb2.AnalysisGetResponse.SerializeToString,
+                    request_deserializer=analysis__config__pb2.AnalysisConfigGetRequest.FromString,
+                    response_serializer=analysis__config__pb2.AnalysisConfigGetResponse.SerializeToString,
             ),
             'list': grpc.unary_unary_rpc_method_handler(
                     servicer.list,
-                    request_deserializer=analysis__pb2.AnalysisListRequest.FromString,
-                    response_serializer=analysis__pb2.AnalysisListResponse.SerializeToString,
+                    request_deserializer=analysis__config__pb2.AnalysisConfigListRequest.FromString,
+                    response_serializer=analysis__config__pb2.AnalysisConfigListResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'oi.papi.AnalysisApi', rpc_method_handlers)
+            'oi.papi.AnalysisConfigApi', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class AnalysisApi(object):
+class AnalysisConfigApi(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def create(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AnalysisApi/create',
-            analysis__pb2.AnalysisCreateRequest.SerializeToString,
-            analysis__pb2.AnalysisCreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AnalysisConfigApi/create',
+            analysis__config__pb2.AnalysisConfigCreateRequest.SerializeToString,
+            analysis__config__pb2.AnalysisConfigCreateResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AnalysisApi/get',
-            analysis__pb2.AnalysisGetRequest.SerializeToString,
-            analysis__pb2.AnalysisGetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AnalysisConfigApi/get',
+            analysis__config__pb2.AnalysisConfigGetRequest.SerializeToString,
+            analysis__config__pb2.AnalysisConfigGetResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AnalysisApi/list',
-            analysis__pb2.AnalysisListRequest.SerializeToString,
-            analysis__pb2.AnalysisListResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AnalysisConfigApi/list',
+            analysis__config__pb2.AnalysisConfigListRequest.SerializeToString,
+            analysis__config__pb2.AnalysisConfigListResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/analysis_version_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/analysis_computation_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,202 +1,178 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
-from terrascope_api.models import analysis_version_pb2 as analysis__version__pb2
+from terrascope_api.models import analysis_computation_pb2 as analysis__computation__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in analysis_version_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
 
-
-class AnalysisVersionApiStub(object):
+class AnalysisComputationApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.create = channel.unary_unary(
-                '/oi.papi.AnalysisVersionApi/create',
-                request_serializer=analysis__version__pb2.AnalysisVersionCreateRequest.SerializeToString,
-                response_deserializer=analysis__version__pb2.AnalysisVersionCreateResponse.FromString,
-                _registered_method=True)
+                '/oi.papi.AnalysisComputationApi/create',
+                request_serializer=analysis__computation__pb2.AnalysisComputationCreateRequest.SerializeToString,
+                response_deserializer=analysis__computation__pb2.AnalysisComputationCreateResponse.FromString,
+                )
+        self.run = channel.unary_unary(
+                '/oi.papi.AnalysisComputationApi/run',
+                request_serializer=analysis__computation__pb2.AnalysisComputationRunRequest.SerializeToString,
+                response_deserializer=analysis__computation__pb2.AnalysisComputationRunResponse.FromString,
+                )
         self.get = channel.unary_unary(
-                '/oi.papi.AnalysisVersionApi/get',
-                request_serializer=analysis__version__pb2.AnalysisVersionGetRequest.SerializeToString,
-                response_deserializer=analysis__version__pb2.AnalysisVersionGetResponse.FromString,
-                _registered_method=True)
+                '/oi.papi.AnalysisComputationApi/get',
+                request_serializer=analysis__computation__pb2.AnalysisComputationGetRequest.SerializeToString,
+                response_deserializer=analysis__computation__pb2.AnalysisComputationGetResponse.FromString,
+                )
         self.list = channel.unary_unary(
-                '/oi.papi.AnalysisVersionApi/list',
-                request_serializer=analysis__version__pb2.AnalysisVersionListRequest.SerializeToString,
-                response_deserializer=analysis__version__pb2.AnalysisVersionListResponse.FromString,
-                _registered_method=True)
+                '/oi.papi.AnalysisComputationApi/list',
+                request_serializer=analysis__computation__pb2.AnalysisComputationListRequest.SerializeToString,
+                response_deserializer=analysis__computation__pb2.AnalysisComputationListResponse.FromString,
+                )
 
 
-class AnalysisVersionApiServicer(object):
+class AnalysisComputationApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def create(self, request, context):
         """
-        Given a top level Analysis, create a new version, which must be semantically greater than the previously created version.
-        Once an AnalysisVersion has been created, it is immutable. Any changes require a new version to be created.
-        The purpose of this is to either upgrade the structure of the Analysis DAG OR update the versions of the algorithms assigned to the Analysis.
+        Create the runnable component in the system, by specifying the Analysis to be run, the set of AOIs to be run on, and the TOI.
+        The analysis_computation_id is returned so that it can be run.
+        Note that until an AnalysisComputation has been run, its underlying resources are NOT locked and therefore can be changed.
+        The names of an AlgorithmComputationNode must match that of it's corresponding Analysis' AnalysisAlgorithmNode.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def run(self, request, context):
+        """
+        The first time this endpoint is called, the system initiates the running of the provided analysis_computation_id.
+        This causes credits to be place in pending status and eventually consumed when the AnalysisComputation completes.
+        Credits are consumed as each result is produced. Once an Analysis has been run, all of its underlying constituent parts are considered locked and cannot be modified.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def get(self, request, context):
         """
-        Get the details for a specific AnalysisVersion. By default it does not include the analysis_manifest.
-        Setting include_manifest to true, will also include the manifest in the response for each requested AnalysisVersion.
+        Retrieves the details of the provided AnalysisComputation including its current state and its progress.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def list(self, request, context):
         """
-        List all the AnalysisVersions that the user has access to.
-        Search text will be applied to the entire manifest returning all AnalysisVersions whose manifest contains the search text.
-        Tags will be matched exactly with the tags on the manifest.
-        By default, this method only returns the semantically latest version of each Analysis that has not been deprecated.
-        It does not include manifests in the response.
-        If include_all_versions is set to true, all prior versions of an Analysis including deprecated AnalysisVersions will be returned, as well.
-        If include_manifest is set to true, the corresponding manifest of each AnalysisVersion will also be returned.
+        Lists the details for all AnalysisComputations that the requester has access to including their current state and their progress.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_AnalysisVersionApiServicer_to_server(servicer, server):
+def add_AnalysisComputationApiServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'create': grpc.unary_unary_rpc_method_handler(
                     servicer.create,
-                    request_deserializer=analysis__version__pb2.AnalysisVersionCreateRequest.FromString,
-                    response_serializer=analysis__version__pb2.AnalysisVersionCreateResponse.SerializeToString,
+                    request_deserializer=analysis__computation__pb2.AnalysisComputationCreateRequest.FromString,
+                    response_serializer=analysis__computation__pb2.AnalysisComputationCreateResponse.SerializeToString,
+            ),
+            'run': grpc.unary_unary_rpc_method_handler(
+                    servicer.run,
+                    request_deserializer=analysis__computation__pb2.AnalysisComputationRunRequest.FromString,
+                    response_serializer=analysis__computation__pb2.AnalysisComputationRunResponse.SerializeToString,
             ),
             'get': grpc.unary_unary_rpc_method_handler(
                     servicer.get,
-                    request_deserializer=analysis__version__pb2.AnalysisVersionGetRequest.FromString,
-                    response_serializer=analysis__version__pb2.AnalysisVersionGetResponse.SerializeToString,
+                    request_deserializer=analysis__computation__pb2.AnalysisComputationGetRequest.FromString,
+                    response_serializer=analysis__computation__pb2.AnalysisComputationGetResponse.SerializeToString,
             ),
             'list': grpc.unary_unary_rpc_method_handler(
                     servicer.list,
-                    request_deserializer=analysis__version__pb2.AnalysisVersionListRequest.FromString,
-                    response_serializer=analysis__version__pb2.AnalysisVersionListResponse.SerializeToString,
+                    request_deserializer=analysis__computation__pb2.AnalysisComputationListRequest.FromString,
+                    response_serializer=analysis__computation__pb2.AnalysisComputationListResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'oi.papi.AnalysisVersionApi', rpc_method_handlers)
+            'oi.papi.AnalysisComputationApi', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class AnalysisVersionApi(object):
+class AnalysisComputationApi(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def create(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AnalysisComputationApi/create',
+            analysis__computation__pb2.AnalysisComputationCreateRequest.SerializeToString,
+            analysis__computation__pb2.AnalysisComputationCreateResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def run(request,
             target,
-            '/oi.papi.AnalysisVersionApi/create',
-            analysis__version__pb2.AnalysisVersionCreateRequest.SerializeToString,
-            analysis__version__pb2.AnalysisVersionCreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AnalysisComputationApi/run',
+            analysis__computation__pb2.AnalysisComputationRunRequest.SerializeToString,
+            analysis__computation__pb2.AnalysisComputationRunResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AnalysisVersionApi/get',
-            analysis__version__pb2.AnalysisVersionGetRequest.SerializeToString,
-            analysis__version__pb2.AnalysisVersionGetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AnalysisComputationApi/get',
+            analysis__computation__pb2.AnalysisComputationGetRequest.SerializeToString,
+            analysis__computation__pb2.AnalysisComputationGetResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AnalysisVersionApi/list',
-            analysis__version__pb2.AnalysisVersionListRequest.SerializeToString,
-            analysis__version__pb2.AnalysisVersionListResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AnalysisComputationApi/list',
+            analysis__computation__pb2.AnalysisComputationListRequest.SerializeToString,
+            analysis__computation__pb2.AnalysisComputationListResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/aoi_collection_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/aoi_collection_pb2_grpc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,53 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
 from terrascope_api.models import aoi_collection_pb2 as aoi__collection__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in aoi_collection_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
-
 
 class AOICollectionApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.create = channel.unary_unary(
                 '/oi.papi.AOICollectionApi/create',
                 request_serializer=aoi__collection__pb2.AOICollectionCreateRequest.SerializeToString,
                 response_deserializer=aoi__collection__pb2.AOICollectionCreateResponse.FromString,
-                _registered_method=True)
+                )
         self.get = channel.unary_unary(
                 '/oi.papi.AOICollectionApi/get',
                 request_serializer=aoi__collection__pb2.AOICollectionGetRequest.SerializeToString,
                 response_deserializer=aoi__collection__pb2.AOICollectionGetResponse.FromString,
-                _registered_method=True)
+                )
         self.clone = channel.unary_unary(
                 '/oi.papi.AOICollectionApi/clone',
                 request_serializer=aoi__collection__pb2.AOICollectionCloneRequest.SerializeToString,
                 response_deserializer=aoi__collection__pb2.AOICollectionCloneResponse.FromString,
-                _registered_method=True)
+                )
         self.add = channel.unary_unary(
                 '/oi.papi.AOICollectionApi/add',
                 request_serializer=aoi__collection__pb2.AOICollectionAddRequest.SerializeToString,
                 response_deserializer=aoi__collection__pb2.AOICollectionAddResponse.FromString,
-                _registered_method=True)
+                )
         self.remove = channel.unary_unary(
                 '/oi.papi.AOICollectionApi/remove',
                 request_serializer=aoi__collection__pb2.AOICollectionRemoveRequest.SerializeToString,
                 response_deserializer=aoi__collection__pb2.AOICollectionRemoveResponse.FromString,
-                _registered_method=True)
+                )
         self.list = channel.unary_unary(
                 '/oi.papi.AOICollectionApi/list',
                 request_serializer=aoi__collection__pb2.AOICollectionListRequest.SerializeToString,
                 response_deserializer=aoi__collection__pb2.AOICollectionListResponse.FromString,
-                _registered_method=True)
+                )
 
 
 class AOICollectionApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def create(self, request, context):
         """
@@ -175,157 +150,97 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AOICollectionApi/create',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AOICollectionApi/create',
             aoi__collection__pb2.AOICollectionCreateRequest.SerializeToString,
             aoi__collection__pb2.AOICollectionCreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AOICollectionApi/get',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AOICollectionApi/get',
             aoi__collection__pb2.AOICollectionGetRequest.SerializeToString,
             aoi__collection__pb2.AOICollectionGetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def clone(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AOICollectionApi/clone',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AOICollectionApi/clone',
             aoi__collection__pb2.AOICollectionCloneRequest.SerializeToString,
             aoi__collection__pb2.AOICollectionCloneResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def add(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AOICollectionApi/add',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AOICollectionApi/add',
             aoi__collection__pb2.AOICollectionAddRequest.SerializeToString,
             aoi__collection__pb2.AOICollectionAddResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def remove(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AOICollectionApi/remove',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AOICollectionApi/remove',
             aoi__collection__pb2.AOICollectionRemoveRequest.SerializeToString,
             aoi__collection__pb2.AOICollectionRemoveResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AOICollectionApi/list',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AOICollectionApi/list',
             aoi__collection__pb2.AOICollectionListRequest.SerializeToString,
             aoi__collection__pb2.AOICollectionListResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/aoi_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/aoi_pb2_grpc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,43 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
 from terrascope_api.models import aoi_pb2 as aoi__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in aoi_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
-
 
 class AOIApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.create = channel.unary_unary(
                 '/oi.papi.AOIApi/create',
                 request_serializer=aoi__pb2.AOICreateRequest.SerializeToString,
                 response_deserializer=aoi__pb2.AOICreateResponse.FromString,
-                _registered_method=True)
+                )
         self.get = channel.unary_unary(
                 '/oi.papi.AOIApi/get',
                 request_serializer=aoi__pb2.AOIGetRequest.SerializeToString,
                 response_deserializer=aoi__pb2.AOIGetResponse.FromString,
-                _registered_method=True)
+                )
         self.upload = channel.stream_unary(
                 '/oi.papi.AOIApi/upload',
                 request_serializer=aoi__pb2.AOIUploadRequest.SerializeToString,
                 response_deserializer=aoi__pb2.AOIUploadResponse.FromString,
-                _registered_method=True)
+                )
         self.update = channel.unary_unary(
                 '/oi.papi.AOIApi/update',
                 request_serializer=aoi__pb2.AOIUpdateRequest.SerializeToString,
                 response_deserializer=aoi__pb2.AOIUpdateResponse.FromString,
-                _registered_method=True)
+                )
 
 
 class AOIApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def create(self, request, context):
         """
@@ -143,103 +118,63 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AOIApi/create',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AOIApi/create',
             aoi__pb2.AOICreateRequest.SerializeToString,
             aoi__pb2.AOICreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AOIApi/get',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AOIApi/get',
             aoi__pb2.AOIGetRequest.SerializeToString,
             aoi__pb2.AOIGetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def upload(request_iterator,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.stream_unary(
-            request_iterator,
-            target,
-            '/oi.papi.AOIApi/upload',
+        return grpc.experimental.stream_unary(request_iterator, target, '/oi.papi.AOIApi/upload',
             aoi__pb2.AOIUploadRequest.SerializeToString,
             aoi__pb2.AOIUploadResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def update(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AOIApi/update',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.AOIApi/update',
             aoi__pb2.AOIUpdateRequest.SerializeToString,
             aoi__pb2.AOIUpdateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/aoi_version_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/user_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,196 +1,179 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
-from terrascope_api.models import aoi_version_pb2 as aoi__version__pb2
+from terrascope_api.models import user_pb2 as user__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in aoi_version_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
 
-
-class AOIVersionApiStub(object):
+class UserApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
+        self.login = channel.unary_unary(
+                '/oi.papi.UserApi/login',
+                request_serializer=user__pb2.LoginRequest.SerializeToString,
+                response_deserializer=user__pb2.LoginResponse.FromString,
+                )
         self.create = channel.unary_unary(
-                '/oi.papi.AOIVersionApi/create',
-                request_serializer=aoi__version__pb2.AOIVersionCreateRequest.SerializeToString,
-                response_deserializer=aoi__version__pb2.AOIVersionCreateResponse.FromString,
-                _registered_method=True)
+                '/oi.papi.UserApi/create',
+                request_serializer=user__pb2.UserCreateRequest.SerializeToString,
+                response_deserializer=user__pb2.UserCreateResponse.FromString,
+                )
         self.get = channel.unary_unary(
-                '/oi.papi.AOIVersionApi/get',
-                request_serializer=aoi__version__pb2.AOIVersionGetRequest.SerializeToString,
-                response_deserializer=aoi__version__pb2.AOIVersionGetResponse.FromString,
-                _registered_method=True)
+                '/oi.papi.UserApi/get',
+                request_serializer=user__pb2.UserGetRequest.SerializeToString,
+                response_deserializer=user__pb2.UserGetResponse.FromString,
+                )
         self.list = channel.unary_unary(
-                '/oi.papi.AOIVersionApi/list',
-                request_serializer=aoi__version__pb2.AOIVersionListRequest.SerializeToString,
-                response_deserializer=aoi__version__pb2.AOIVersionListResponse.FromString,
-                _registered_method=True)
+                '/oi.papi.UserApi/list',
+                request_serializer=user__pb2.UserListRequest.SerializeToString,
+                response_deserializer=user__pb2.UserListResponse.FromString,
+                )
 
 
-class AOIVersionApiServicer(object):
+class UserApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
+    def login(self, request, context):
+        """
+        Login using user's email and password.
+        The endpoint returns a JWT access token that is needed to use the API.
+        Note: This endpoint does NOT require token authentication.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def create(self, request, context):
         """
-        Create a new AOIVersion that is tied to the original AOI by reference of the aoi_id.
-        After specifying the aoi modifications, the original is copied and modified. Further, AOIVersions are immutable.
+        Create a new User in the system, assigned to the specified department.
+        This functionality is only available for an admin user.
+        This automatically creates an AOICollection associated to this user.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def get(self, request, context):
         """
-        Get the actual AOI details specified by the provided version. Additionally, choose which metadata fields should be returned.
-        A list of AOICollections that the AOIVersion is a part of is also returned.
+        Returns the details of the specified User. If no User is given, returns details for the requesting User.
+        The specified User must belong to the same UserCollection as the requesting User, otherwise an error is thrown.
+        The user_id is a uuid and is actually the folder ID, so its a subject ID. Access limitations apply.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def list(self, request, context):
         """
-        List the available AOIVersions, including on the latest versions by default that match the specific filters.
-        Additional options include the ability to list out all fields of the AOIVersion by setting the verbose flag to True.
+        List users. Access limitations apply.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_AOIVersionApiServicer_to_server(servicer, server):
+def add_UserApiServicer_to_server(servicer, server):
     rpc_method_handlers = {
+            'login': grpc.unary_unary_rpc_method_handler(
+                    servicer.login,
+                    request_deserializer=user__pb2.LoginRequest.FromString,
+                    response_serializer=user__pb2.LoginResponse.SerializeToString,
+            ),
             'create': grpc.unary_unary_rpc_method_handler(
                     servicer.create,
-                    request_deserializer=aoi__version__pb2.AOIVersionCreateRequest.FromString,
-                    response_serializer=aoi__version__pb2.AOIVersionCreateResponse.SerializeToString,
+                    request_deserializer=user__pb2.UserCreateRequest.FromString,
+                    response_serializer=user__pb2.UserCreateResponse.SerializeToString,
             ),
             'get': grpc.unary_unary_rpc_method_handler(
                     servicer.get,
-                    request_deserializer=aoi__version__pb2.AOIVersionGetRequest.FromString,
-                    response_serializer=aoi__version__pb2.AOIVersionGetResponse.SerializeToString,
+                    request_deserializer=user__pb2.UserGetRequest.FromString,
+                    response_serializer=user__pb2.UserGetResponse.SerializeToString,
             ),
             'list': grpc.unary_unary_rpc_method_handler(
                     servicer.list,
-                    request_deserializer=aoi__version__pb2.AOIVersionListRequest.FromString,
-                    response_serializer=aoi__version__pb2.AOIVersionListResponse.SerializeToString,
+                    request_deserializer=user__pb2.UserListRequest.FromString,
+                    response_serializer=user__pb2.UserListResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'oi.papi.AOIVersionApi', rpc_method_handlers)
+            'oi.papi.UserApi', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class AOIVersionApi(object):
+class UserApi(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def create(request,
+    def login(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.UserApi/login',
+            user__pb2.LoginRequest.SerializeToString,
+            user__pb2.LoginResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def create(request,
             target,
-            '/oi.papi.AOIVersionApi/create',
-            aoi__version__pb2.AOIVersionCreateRequest.SerializeToString,
-            aoi__version__pb2.AOIVersionCreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.UserApi/create',
+            user__pb2.UserCreateRequest.SerializeToString,
+            user__pb2.UserCreateResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AOIVersionApi/get',
-            aoi__version__pb2.AOIVersionGetRequest.SerializeToString,
-            aoi__version__pb2.AOIVersionGetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.UserApi/get',
+            user__pb2.UserGetRequest.SerializeToString,
+            user__pb2.UserGetResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.AOIVersionApi/list',
-            aoi__version__pb2.AOIVersionListRequest.SerializeToString,
-            aoi__version__pb2.AOIVersionListResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.UserApi/list',
+            user__pb2.UserListRequest.SerializeToString,
+            user__pb2.UserListResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/credit_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/credit_pb2_grpc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,63 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
 from terrascope_api.models import credit_pb2 as credit__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in credit_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
-
 
 class CreditApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.add = channel.unary_unary(
                 '/oi.papi.credit.CreditApi/add',
                 request_serializer=credit__pb2.CreditAddRequest.SerializeToString,
                 response_deserializer=credit__pb2.CreditAddResponse.FromString,
-                _registered_method=True)
+                )
         self.remove = channel.unary_unary(
                 '/oi.papi.credit.CreditApi/remove',
                 request_serializer=credit__pb2.CreditRemoveRequest.SerializeToString,
                 response_deserializer=credit__pb2.CreditRemoveResponse.FromString,
-                _registered_method=True)
+                )
         self.refund = channel.unary_unary(
                 '/oi.papi.credit.CreditApi/refund',
                 request_serializer=credit__pb2.CreditRefundRequest.SerializeToString,
                 response_deserializer=credit__pb2.CreditRefundResponse.FromString,
-                _registered_method=True)
+                )
         self.set_algorithm = channel.unary_unary(
                 '/oi.papi.credit.CreditApi/set_algorithm',
                 request_serializer=credit__pb2.CreditAlgorithmMultiplierSetRequest.SerializeToString,
                 response_deserializer=credit__pb2.CreditAlgorithmMultiplierSetResponse.FromString,
-                _registered_method=True)
+                )
         self.set_data_source = channel.unary_unary(
                 '/oi.papi.credit.CreditApi/set_data_source',
                 request_serializer=credit__pb2.CreditDataSourceMultiplierSetRequest.SerializeToString,
                 response_deserializer=credit__pb2.CreditDataSourceMultiplierSetResponse.FromString,
-                _registered_method=True)
+                )
         self.estimate = channel.unary_unary(
                 '/oi.papi.credit.CreditApi/estimate',
                 request_serializer=credit__pb2.CreditEstimateRequest.SerializeToString,
                 response_deserializer=credit__pb2.CreditEstimateResponse.FromString,
-                _registered_method=True)
+                )
         self.summary = channel.unary_unary(
                 '/oi.papi.credit.CreditApi/summary',
                 request_serializer=credit__pb2.CreditSummaryRequest.SerializeToString,
                 response_deserializer=credit__pb2.CreditSummaryResponse.FromString,
-                _registered_method=True)
+                )
         self.transactions = channel.unary_unary(
                 '/oi.papi.credit.CreditApi/transactions',
                 request_serializer=credit__pb2.CreditTransactionsRequest.SerializeToString,
                 response_deserializer=credit__pb2.CreditTransactionsResponse.FromString,
-                _registered_method=True)
+                )
 
 
 class CreditApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def add(self, request, context):
         """
@@ -212,211 +187,131 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.credit.CreditApi/add',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.credit.CreditApi/add',
             credit__pb2.CreditAddRequest.SerializeToString,
             credit__pb2.CreditAddResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def remove(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.credit.CreditApi/remove',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.credit.CreditApi/remove',
             credit__pb2.CreditRemoveRequest.SerializeToString,
             credit__pb2.CreditRemoveResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def refund(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.credit.CreditApi/refund',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.credit.CreditApi/refund',
             credit__pb2.CreditRefundRequest.SerializeToString,
             credit__pb2.CreditRefundResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def set_algorithm(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.credit.CreditApi/set_algorithm',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.credit.CreditApi/set_algorithm',
             credit__pb2.CreditAlgorithmMultiplierSetRequest.SerializeToString,
             credit__pb2.CreditAlgorithmMultiplierSetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def set_data_source(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.credit.CreditApi/set_data_source',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.credit.CreditApi/set_data_source',
             credit__pb2.CreditDataSourceMultiplierSetRequest.SerializeToString,
             credit__pb2.CreditDataSourceMultiplierSetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def estimate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.credit.CreditApi/estimate',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.credit.CreditApi/estimate',
             credit__pb2.CreditEstimateRequest.SerializeToString,
             credit__pb2.CreditEstimateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def summary(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.credit.CreditApi/summary',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.credit.CreditApi/summary',
             credit__pb2.CreditSummaryRequest.SerializeToString,
             credit__pb2.CreditSummaryResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def transactions(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.credit.CreditApi/transactions',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.credit.CreditApi/transactions',
             credit__pb2.CreditTransactionsRequest.SerializeToString,
             credit__pb2.CreditTransactionsResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/data_source_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/data_type_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,148 +1,138 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
-from terrascope_api.models import data_source_pb2 as data__source__pb2
+from terrascope_api.models import data_type_pb2 as data__type__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in data_source_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
 
-
-class DataSourceAPIStub(object):
+class DataTypeAPIStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
+        self.create = channel.unary_unary(
+                '/oi.papi.DataTypeAPI/create',
+                request_serializer=data__type__pb2.DataTypeCreateRequest.SerializeToString,
+                response_deserializer=data__type__pb2.DataTypeCreateResponse.FromString,
+                )
         self.get = channel.unary_unary(
-                '/oi.papi.DataSourceAPI/get',
-                request_serializer=data__source__pb2.DataSourceGetRequest.SerializeToString,
-                response_deserializer=data__source__pb2.DataSourceGetResponse.FromString,
-                _registered_method=True)
+                '/oi.papi.DataTypeAPI/get',
+                request_serializer=data__type__pb2.DataTypeGetRequest.SerializeToString,
+                response_deserializer=data__type__pb2.DataTypeGetResponse.FromString,
+                )
         self.list = channel.unary_unary(
-                '/oi.papi.DataSourceAPI/list',
-                request_serializer=data__source__pb2.DataSourceListRequest.SerializeToString,
-                response_deserializer=data__source__pb2.DataSourceListResponse.FromString,
-                _registered_method=True)
+                '/oi.papi.DataTypeAPI/list',
+                request_serializer=data__type__pb2.DataTypeListRequest.SerializeToString,
+                response_deserializer=data__type__pb2.DataTypeListResponse.FromString,
+                )
 
 
-class DataSourceAPIServicer(object):
+class DataTypeAPIServicer(object):
     """Missing associated documentation comment in .proto file."""
 
+    def create(self, request, context):
+        """
+        Creates a new DataType.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def get(self, request, context):
         """
-        Retrieves all of the details about the specified DataSource.
+        Gets a DataType that the user has access to.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def list(self, request, context):
         """
-        List all available DataSources that the user has access to.
+        List all registered DataType.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_DataSourceAPIServicer_to_server(servicer, server):
+def add_DataTypeAPIServicer_to_server(servicer, server):
     rpc_method_handlers = {
+            'create': grpc.unary_unary_rpc_method_handler(
+                    servicer.create,
+                    request_deserializer=data__type__pb2.DataTypeCreateRequest.FromString,
+                    response_serializer=data__type__pb2.DataTypeCreateResponse.SerializeToString,
+            ),
             'get': grpc.unary_unary_rpc_method_handler(
                     servicer.get,
-                    request_deserializer=data__source__pb2.DataSourceGetRequest.FromString,
-                    response_serializer=data__source__pb2.DataSourceGetResponse.SerializeToString,
+                    request_deserializer=data__type__pb2.DataTypeGetRequest.FromString,
+                    response_serializer=data__type__pb2.DataTypeGetResponse.SerializeToString,
             ),
             'list': grpc.unary_unary_rpc_method_handler(
                     servicer.list,
-                    request_deserializer=data__source__pb2.DataSourceListRequest.FromString,
-                    response_serializer=data__source__pb2.DataSourceListResponse.SerializeToString,
+                    request_deserializer=data__type__pb2.DataTypeListRequest.FromString,
+                    response_serializer=data__type__pb2.DataTypeListResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'oi.papi.DataSourceAPI', rpc_method_handlers)
+            'oi.papi.DataTypeAPI', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class DataSourceAPI(object):
+class DataTypeAPI(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def get(request,
+    def create(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.DataTypeAPI/create',
+            data__type__pb2.DataTypeCreateRequest.SerializeToString,
+            data__type__pb2.DataTypeCreateResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def get(request,
             target,
-            '/oi.papi.DataSourceAPI/get',
-            data__source__pb2.DataSourceGetRequest.SerializeToString,
-            data__source__pb2.DataSourceGetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.DataTypeAPI/get',
+            data__type__pb2.DataTypeGetRequest.SerializeToString,
+            data__type__pb2.DataTypeGetResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.DataSourceAPI/list',
-            data__source__pb2.DataSourceListRequest.SerializeToString,
-            data__source__pb2.DataSourceListResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.DataTypeAPI/list',
+            data__type__pb2.DataTypeListRequest.SerializeToString,
+            data__type__pb2.DataTypeListResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/permission_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/permission_pb2_grpc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,33 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
 from terrascope_api.models import permission_pb2 as permission__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in permission_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
-
 
 class PermissionApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.create = channel.unary_unary(
                 '/oi.papi.permission.PermissionApi/create',
                 request_serializer=permission__pb2.PermissionCreateRequest.SerializeToString,
                 response_deserializer=permission__pb2.PermissionCreateResponse.FromString,
-                _registered_method=True)
+                )
         self.delete = channel.unary_unary(
                 '/oi.papi.permission.PermissionApi/delete',
                 request_serializer=permission__pb2.PermissionDeleteRequest.SerializeToString,
                 response_deserializer=permission__pb2.PermissionDeleteResponse.FromString,
-                _registered_method=True)
+                )
 
 
 class PermissionApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def create(self, request, context):
         """
@@ -103,49 +78,29 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.permission.PermissionApi/create',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.permission.PermissionApi/create',
             permission__pb2.PermissionCreateRequest.SerializeToString,
             permission__pb2.PermissionCreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def delete(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.permission.PermissionApi/delete',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.permission.PermissionApi/delete',
             permission__pb2.PermissionDeleteRequest.SerializeToString,
             permission__pb2.PermissionDeleteResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/toi_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/toi_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,43 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
 from terrascope_api.models import toi_pb2 as toi__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in toi_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
-
 
 class TOIApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.create = channel.unary_unary(
                 '/oi.papi.TOIApi/create',
                 request_serializer=toi__pb2.TOICreateRequest.SerializeToString,
                 response_deserializer=toi__pb2.TOICreateResponse.FromString,
-                _registered_method=True)
+                )
         self.delete = channel.unary_unary(
                 '/oi.papi.TOIApi/delete',
                 request_serializer=toi__pb2.TOIDeleteRequest.SerializeToString,
                 response_deserializer=toi__pb2.TOIDeleteResponse.FromString,
-                _registered_method=True)
+                )
         self.get = channel.unary_unary(
                 '/oi.papi.TOIApi/get',
                 request_serializer=toi__pb2.TOIGetRequest.SerializeToString,
                 response_deserializer=toi__pb2.TOIGetResponse.FromString,
-                _registered_method=True)
+                )
         self.list = channel.unary_unary(
                 '/oi.papi.TOIApi/list',
                 request_serializer=toi__pb2.TOIListRequest.SerializeToString,
                 response_deserializer=toi__pb2.TOIListResponse.FromString,
-                _registered_method=True)
+                )
 
 
 class TOIApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def create(self, request, context):
         """
@@ -138,103 +113,63 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.TOIApi/create',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.TOIApi/create',
             toi__pb2.TOICreateRequest.SerializeToString,
             toi__pb2.TOICreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def delete(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.TOIApi/delete',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.TOIApi/delete',
             toi__pb2.TOIDeleteRequest.SerializeToString,
             toi__pb2.TOIDeleteResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def get(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.TOIApi/get',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.TOIApi/get',
             toi__pb2.TOIGetRequest.SerializeToString,
             toi__pb2.TOIGetResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def list(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.TOIApi/list',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.TOIApi/list',
             toi__pb2.TOIListRequest.SerializeToString,
             toi__pb2.TOIListResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/stubs/token_pb2_grpc.py` & `terrascope-api-1.0.5/src/py/terrascope_api/stubs/token_pb2_grpc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,28 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-import warnings
 
 from terrascope_api.models import token_pb2 as token__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
-GRPC_VERSION = grpc.__version__
-EXPECTED_ERROR_RELEASE = '1.65.0'
-SCHEDULED_RELEASE_DATE = 'June 25, 2024'
-_version_not_supported = False
-
-try:
-    from grpc._utilities import first_version_is_lower
-    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
-except ImportError:
-    _version_not_supported = True
-
-if _version_not_supported:
-    warnings.warn(
-        f'The grpc package installed is at version {GRPC_VERSION},'
-        + f' but the generated code in token_pb2_grpc.py depends on'
-        + f' grpcio>={GRPC_GENERATED_VERSION}.'
-        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
-        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
-        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
-        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
-        RuntimeWarning
-    )
-
 
 class TokenApiStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.create = channel.unary_unary(
                 '/oi.papi.TokenApi/create',
                 request_serializer=token__pb2.TokenCreateRequest.SerializeToString,
                 response_deserializer=token__pb2.TokenCreateResponse.FromString,
-                _registered_method=True)
+                )
 
 
 class TokenApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def create(self, request, context):
         """
@@ -83,22 +58,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(
-            request,
-            target,
-            '/oi.papi.TokenApi/create',
+        return grpc.experimental.unary_unary(request, target, '/oi.papi.TokenApi/create',
             token__pb2.TokenCreateRequest.SerializeToString,
             token__pb2.TokenCreateResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-            _registered_method=True)
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api/terrascope_base_api.py` & `terrascope-api-1.0.5/src/py/terrascope_api/async_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,59 @@
 # Copyright 2017-2021 Orbital Insight Inc., all rights reserved.
 # Contains confidential and trade secret information.
 # Government Users:  Commercial Computer Software - Use governed by
 # terms of Orbital Insight commercial license agreement.
 
 
+# TODO: figure out reuse sync client. async and sync client almost same
 import os
-from abc import ABC, abstractmethod
-
-import json
 
 import grpc
+import json
+from terrascope_api import models
 from terrascope_api import stubs
-
+from terrascope_api.async_interceptors import (
+    ContextInjectorUnaryUnary, ContextInjectorStreamUnary, ContextInjectorUnaryStream, ContextInjectorStreamStream
+)
 
 API_TOKEN = 'TERRASCOPE_API_TOKEN'
 
 
-class TerrascopeBaseApi(ABC):
-    def __init__(self, oi_papi_url, port=443, secure=True, api_token=None, root_certificates_file=None):
+class TerrascopeAsyncClient:
+    def __init__(self, oi_papi_url, port=443, secure=True, api_token=None):
+        self.api = TerrascopeAsyncApi(oi_papi_url, port, secure, api_token=api_token)
+        self.models = models
+
+
+class TerrascopeAsyncApi:
+    def __init__(self, oi_papi_url, port=443, secure=True, api_token=None):
         self._oi_papi_url = oi_papi_url
         self._port = port
-
-        self.api_token = os.environ.get(API_TOKEN, "").strip() if api_token is None else api_token.strip()
+        if api_token is None:
+            api_token = os.environ.get(API_TOKEN)
+            if api_token is None:
+                homedir = os.environ.get('HOME', '/')
+                token_filename = f'{homedir}/.orbital/api_token'
+                try:
+                    with open(token_filename) as fd:
+                        api_token = fd.read()
+                except FileNotFoundError:
+                    pass
+        if api_token is not None:
+            api_token = api_token.strip()
+        self.api_token = api_token
+        if not secure and api_token is not None:
+            raise ValueError('API token cannot be passed over an unsecure connection')
+            # grpc will not transmit the Authorization header over an unsecured channel, which
+            #  makes sense since it would be easy to hijack
+        self.context_injecting_interceptors = [
+            # materialize distributed context from request headers
+            ContextInjectorUnaryUnary(), ContextInjectorUnaryStream(),
+            ContextInjectorStreamUnary(), ContextInjectorStreamStream()
+        ]
         self.options = [('grpc.max_send_message_length', -1),
                         ('grpc.max_receive_message_length', -1),
                         ('grpc.max_metadata_size', 16000)]
         service_config_json = json.dumps({
             "methodConfig": [{
                 "name": [{}],  # Apply retry to all methods by using [{}]
                 "retryPolicy": {
@@ -34,63 +62,57 @@
                     "maxBackoff": "60s",
                     "backoffMultiplier": 2,
                     "retryableStatusCodes": ["UNAVAILABLE"],
                 },
             }]
         })
         self.options.append(("grpc.service_config", service_config_json))
-        self._channel = self._get_channel(self._get_ssl_channel_credentials(
-            secure, root_certificates_file=root_certificates_file))
-
-        # unauthenticated users can access forgot_password
-        self.forgot_password = stubs.forgot_password.ForgotPasswordApiStub(self._channel)
-
-        if self.api_token:
-            self.algorithm = stubs.algorithm.AlgorithmApiStub(self._channel)
-            self.algorithm_version = stubs.algorithm_version.AlgorithmVersionApiStub(self._channel)
-            self.algorithm_config = stubs.algorithm_config.AlgorithmConfigApiStub(self._channel)
-            self.aoi = stubs.aoi.AOIApiStub(self._channel)
-            self.aoi_collection = stubs.aoi_collection.AOICollectionApiStub(self._channel)
-            self.aoi_version = stubs.aoi_version.AOIVersionApiStub(self._channel)
-            self.aoi_catalog = stubs.aoi_catalog.AOICatalogApiStub(self._channel)
-            self.aoi_transaction = stubs.aoi_transaction.AOITransactionApiStub(self._channel)
-            self.aoi_export = stubs.aoi_export.AOIExportApiStub(self._channel)
-            self.algorithm_computation = stubs.algorithm_computation.AlgorithmComputationApiStub(self._channel)
-            self.analysis = stubs.analysis.AnalysisApiStub(self._channel)
-            self.analysis_version = stubs.analysis_version.AnalysisVersionApiStub(self._channel)
-            self.credit = stubs.credit.CreditApiStub(self._channel)
-            self.result = stubs.result.ResultApiStub(self._channel)
-            self.analysis_config = stubs.analysis_config.AnalysisConfigApiStub(self._channel)
-            self.analysis_computation = stubs.analysis_computation.AnalysisComputationApiStub(self._channel)
-            self.system = stubs.system.SystemApiStub(self._channel)
-            self.toi = stubs.toi.TOIApiStub(self._channel)
-            self.permission = stubs.permission.PermissionApiStub(self._channel)
-            self.user = stubs.user.UserApiStub(self._channel)
-            self.user_collection = stubs.user_collection.UserCollectionApiStub(self._channel)
-            self.token = stubs.token.TokenApiStub(self._channel)
-            self.visualization = stubs.visualization.VisualizationApiStub(self._channel)
-            self.tile = stubs.tile.TileApiStub(self._channel)
-            self.imagery = stubs.imagery.ImageryApiStub(self._channel)
-            self.notification = stubs.notification.NotificationApiStub(self._channel)
-            self.data_source = stubs.data_source.DataSourceAPIStub(self._channel)
-            self.data_type = stubs.data_type.DataTypeAPIStub(self._channel)
-            self.data_search = stubs.data_search.DataSearchApiStub(self._channel)
-            self.project = stubs.project.ProjectApiStub(self._channel)
+        self._channel = self._get_secure_channel() if secure else self._get_insecure_channel()
+        self.algorithm = stubs.algorithm.AlgorithmApiStub(self._channel)
+        self.algorithm_version = stubs.algorithm_version.AlgorithmVersionApiStub(self._channel)
+        self.algorithm_config = stubs.algorithm_config.AlgorithmConfigApiStub(self._channel)
+        self.aoi = stubs.aoi.AOIApiStub(self._channel)
+        self.aoi_collection = stubs.aoi_collection.AOICollectionApiStub(self._channel)
+        self.aoi_version = stubs.aoi_version.AOIVersionApiStub(self._channel)
+        self.aoi_transaction = stubs.aoi_transaction.AOITransactionApiStub(self._channel)
+        self.algorithm_computation = stubs.algorithm_computation.AlgorithmComputationApiStub(self._channel)
+        self.analysis = stubs.analysis.AnalysisApiStub(self._channel)
+        self.analysis_version = stubs.analysis_version.AnalysisVersionApiStub(self._channel)
+        self.credit = stubs.credit.CreditApiStub(self._channel)
+        self.result = stubs.result.ResultApiStub(self._channel)
+        self.analysis_config = stubs.analysis_config.AnalysisConfigApiStub(self._channel)
+        self.analysis_computation = stubs.analysis_computation.AnalysisComputationApiStub(self._channel)
+        self.system = stubs.system.SystemApiStub(self._channel)
+        self.toi = stubs.toi.TOIApiStub(self._channel)
+        self.permission = stubs.permission.PermissionApiStub(self._channel)
+        self.user = stubs.user.UserApiStub(self._channel)
+        self.user_collection = stubs.user_collection.UserCollectionApiStub(self._channel)
+        self.token = stubs.token.TokenApiStub(self._channel)
+        self.visualization = stubs.visualization.VisualizationApiStub(self._channel)
+        self.tile = stubs.tile.TileApiStub(self._channel)
+
+        self.data_source = stubs.data_source.DataSourceAPIStub(self._channel)
+        self.data_type = stubs.data_type.DataTypeAPIStub(self._channel)
+
+    def _get_insecure_channel(self):
+        return grpc.aio.insecure_channel(f"{self._oi_papi_url}:{self._port}",
+                                         options=self.options,
+                                         interceptors=self.context_injecting_interceptors)
 
-    def _get_ssl_channel_credentials(self, secure, root_certificates_file=None):
+    def _get_secure_channel(self):
+        ssl_creds = grpc.ssl_channel_credentials(root_certificates=None, private_key=None, certificate_chain=None)
         # note: with all defaults, gRPC will search for cert as described here:
         #  https://github.com/grpc/grpc/blob/7a63bd5407d5e14b30f19a5aaf4b6cd1b80f00e1/include/grpc/grpc_security.h#L287
-        # for local env, use local_channel_credentials:
-        #  https://grpc.github.io/grpc/python/grpc.html#grpc.local_channel_credentials
-        if secure:
-            root_certificates = None
-            if root_certificates_file:
-                with open(root_certificates_file, 'rb') as file:
-                    root_certificates = file.read()
-
-            return grpc.ssl_channel_credentials(root_certificates=root_certificates,
-                                                private_key=None, certificate_chain=None)
-        return grpc.local_channel_credentials()
-
-    @abstractmethod
-    def _get_channel(self, channel_credentials: grpc.ChannelCredentials):
-        ...
+        if self.api_token is not None:
+            token_creds = grpc.access_token_call_credentials(self.api_token)
+            creds = grpc.composite_channel_credentials(ssl_creds, token_creds)
+        else:
+            creds = ssl_creds
+        return grpc.aio.secure_channel(f"{self._oi_papi_url}:{self._port}",
+                                       creds,
+                                       options=self.options,
+                                       compression=None,
+                                       interceptors=self.context_injecting_interceptors)
+
+    # TODO: async destructor
+    def __adel__(self):
+        self._channel.close()
```

### Comparing `terrascope-api-1.0.40.2/src/py/terrascope_api.egg-info/SOURCES.txt` & `terrascope-api-1.0.5/src/py/terrascope_api.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 setup.py
 src/py/terrascope_api/__init__.py
 src/py/terrascope_api/async_client.py
 src/py/terrascope_api/async_interceptors.py
 src/py/terrascope_api/sync_client.py
-src/py/terrascope_api/terrascope_base_api.py
 src/py/terrascope_api.egg-info/PKG-INFO
 src/py/terrascope_api.egg-info/SOURCES.txt
 src/py/terrascope_api.egg-info/dependency_links.txt
 src/py/terrascope_api.egg-info/requires.txt
 src/py/terrascope_api.egg-info/top_level.txt
 src/py/terrascope_api/models/__init__.py
 src/py/terrascope_api/models/algorithm_computation_pb2.py
@@ -17,30 +16,23 @@
 src/py/terrascope_api/models/algorithm_manifest_pb2.py
 src/py/terrascope_api/models/algorithm_pb2.py
 src/py/terrascope_api/models/algorithm_version_pb2.py
 src/py/terrascope_api/models/analysis_computation_pb2.py
 src/py/terrascope_api/models/analysis_config_pb2.py
 src/py/terrascope_api/models/analysis_pb2.py
 src/py/terrascope_api/models/analysis_version_pb2.py
-src/py/terrascope_api/models/aoi_catalog_pb2.py
 src/py/terrascope_api/models/aoi_collection_pb2.py
-src/py/terrascope_api/models/aoi_export_pb2.py
 src/py/terrascope_api/models/aoi_pb2.py
 src/py/terrascope_api/models/aoi_transaction_pb2.py
 src/py/terrascope_api/models/aoi_version_pb2.py
 src/py/terrascope_api/models/common_models_pb2.py
 src/py/terrascope_api/models/credit_pb2.py
-src/py/terrascope_api/models/data_search_pb2.py
 src/py/terrascope_api/models/data_source_pb2.py
 src/py/terrascope_api/models/data_type_pb2.py
-src/py/terrascope_api/models/forgot_password_pb2.py
-src/py/terrascope_api/models/imagery_pb2.py
-src/py/terrascope_api/models/notification_pb2.py
 src/py/terrascope_api/models/permission_pb2.py
-src/py/terrascope_api/models/project_pb2.py
 src/py/terrascope_api/models/result_pb2.py
 src/py/terrascope_api/models/system_pb2.py
 src/py/terrascope_api/models/tile_pb2.py
 src/py/terrascope_api/models/toi_pb2.py
 src/py/terrascope_api/models/token_pb2.py
 src/py/terrascope_api/models/user_collection_pb2.py
 src/py/terrascope_api/models/user_pb2.py
@@ -51,30 +43,23 @@
 src/py/terrascope_api/stubs/algorithm_manifest_pb2_grpc.py
 src/py/terrascope_api/stubs/algorithm_pb2_grpc.py
 src/py/terrascope_api/stubs/algorithm_version_pb2_grpc.py
 src/py/terrascope_api/stubs/analysis_computation_pb2_grpc.py
 src/py/terrascope_api/stubs/analysis_config_pb2_grpc.py
 src/py/terrascope_api/stubs/analysis_pb2_grpc.py
 src/py/terrascope_api/stubs/analysis_version_pb2_grpc.py
-src/py/terrascope_api/stubs/aoi_catalog_pb2_grpc.py
 src/py/terrascope_api/stubs/aoi_collection_pb2_grpc.py
-src/py/terrascope_api/stubs/aoi_export_pb2_grpc.py
 src/py/terrascope_api/stubs/aoi_pb2_grpc.py
 src/py/terrascope_api/stubs/aoi_transaction_pb2_grpc.py
 src/py/terrascope_api/stubs/aoi_version_pb2_grpc.py
 src/py/terrascope_api/stubs/common_models_pb2_grpc.py
 src/py/terrascope_api/stubs/credit_pb2_grpc.py
-src/py/terrascope_api/stubs/data_search_pb2_grpc.py
 src/py/terrascope_api/stubs/data_source_pb2_grpc.py
 src/py/terrascope_api/stubs/data_type_pb2_grpc.py
-src/py/terrascope_api/stubs/forgot_password_pb2_grpc.py
-src/py/terrascope_api/stubs/imagery_pb2_grpc.py
-src/py/terrascope_api/stubs/notification_pb2_grpc.py
 src/py/terrascope_api/stubs/permission_pb2_grpc.py
-src/py/terrascope_api/stubs/project_pb2_grpc.py
 src/py/terrascope_api/stubs/result_pb2_grpc.py
 src/py/terrascope_api/stubs/system_pb2_grpc.py
 src/py/terrascope_api/stubs/tile_pb2_grpc.py
 src/py/terrascope_api/stubs/toi_pb2_grpc.py
 src/py/terrascope_api/stubs/token_pb2_grpc.py
 src/py/terrascope_api/stubs/user_collection_pb2_grpc.py
 src/py/terrascope_api/stubs/user_pb2_grpc.py
```

