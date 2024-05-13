# Comparing `tmp/modular_sdk-5.1.1.tar.gz` & `tmp/modular_sdk-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_sdk-5.1.1.tar", last modified: Tue Mar 12 13:24:59 2024, max compression
+gzip compressed data, was "modular_sdk-5.1.2.tar", last modified: Mon May 13 14:52:48 2024, max compression
```

## Comparing `modular_sdk-5.1.1.tar` & `modular_sdk-5.1.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.283540 modular_sdk-5.1.1/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    11357 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/LICENSE
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)       22 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     5144 2024-03-12 13:24:59.283540 modular_sdk-5.1.1/PKG-INFO
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3856 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/README.md
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.275540 modular_sdk-5.1.1/modular_sdk/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/__init__.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.275540 modular_sdk-5.1.1/modular_sdk/commons/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4945 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/commons/__init__.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     7945 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/commons/constants.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2045 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/commons/error_helper.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      200 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/commons/exception.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      800 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/commons/helpers.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2642 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/commons/log_helper.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1025 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/commons/time_helper.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3020 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/commons/trace_helper.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.275540 modular_sdk-5.1.1/modular_sdk/connections/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/connections/__init__.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1754 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/connections/mongodb_connection.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4723 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/connections/rabbit_connection.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.275540 modular_sdk-5.1.1/modular_sdk/helpers/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/helpers/__init__.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      985 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/helpers/response_helper.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.279540 modular_sdk-5.1.1/modular_sdk/models/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/__init__.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2125 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/application.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      929 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/base_meta.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      837 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/customer.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      746 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/customer_settings.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1050 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/execution_trace.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      490 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/heartbeat.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1163 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/job.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      662 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/operation_mode.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3804 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/parent.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.279540 modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/__init__.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    22977 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/base_model.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2261 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/base_role_access_model.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     7095 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/base_safe_update_model.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    18251 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      811 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2565 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/region.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      476 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/setting.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4813 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/tenant.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1081 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/models/tenant_settings.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    11580 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/modular.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.279540 modular_sdk-5.1.1/modular_sdk/services/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/__init__.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     7399 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/application_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4559 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/aws_creds_provider.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1311 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/customer_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1828 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/customer_settings_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     5073 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/environment_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      618 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/events_service.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.279540 modular_sdk-5.1.1/modular_sdk/services/impl/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/impl/__init__.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    25795 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/impl/maestro_credentials_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     9500 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/impl/maestro_rabbit_transport_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2913 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/job_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      620 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/lambda_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    19869 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/parent_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3751 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/rabbit_transport_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2602 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/region_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     9806 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/settings_management_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1488 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/sqs_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     7379 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/ssm_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     8390 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/sts_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     8722 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/tenant_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2935 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/tenant_settings_service.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      745 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/services/thread_local_storage_service.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.283540 modular_sdk-5.1.1/modular_sdk/utils/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/utils/__init__.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.283540 modular_sdk-5.1.1/modular_sdk/utils/job_tracer/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/utils/job_tracer/__init__.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      360 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/utils/job_tracer/abstract.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3854 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/utils/job_tracer/generic.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.283540 modular_sdk-5.1.1/modular_sdk/utils/operation_mode/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/utils/operation_mode/__init__.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      776 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/utils/operation_mode/abstract.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2171 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/utils/operation_mode/generic.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.283540 modular_sdk-5.1.1/modular_sdk/utils/runtime_tracer/
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/utils/runtime_tracer/__init__.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1061 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/utils/runtime_tracer/abstract.py
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4091 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/modular_sdk/utils/runtime_tracer/generic.py
-drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-03-12 13:24:59.283540 modular_sdk-5.1.1/modular_sdk.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     5144 2024-03-12 13:24:59.000000 modular_sdk-5.1.1/modular_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2944 2024-03-12 13:24:59.000000 modular_sdk-5.1.1/modular_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        1 2024-03-12 13:24:59.000000 modular_sdk-5.1.1/modular_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      273 2024-03-12 13:24:59.000000 modular_sdk-5.1.1/modular_sdk.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)       18 2024-03-12 13:24:59.000000 modular_sdk-5.1.1/modular_sdk.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      339 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/pyproject.toml
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1133 2024-03-12 13:24:59.283540 modular_sdk-5.1.1/setup.cfg
--rw-rw-r--   0 jenkins   (1002) jenkins   (1002)       38 2024-03-12 13:24:50.000000 modular_sdk-5.1.1/setup.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.611098 modular_sdk-5.1.2/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    11357 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/LICENSE
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)       22 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     5144 2024-05-13 14:52:48.611098 modular_sdk-5.1.2/PKG-INFO
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3856 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/README.md
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.595098 modular_sdk-5.1.2/modular_sdk/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/__init__.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.595098 modular_sdk-5.1.2/modular_sdk/commons/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4945 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/commons/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     7945 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/commons/constants.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2045 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/commons/error_helper.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      200 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/commons/exception.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      800 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/commons/helpers.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2642 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/commons/log_helper.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1025 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/commons/time_helper.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3020 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/commons/trace_helper.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.599098 modular_sdk-5.1.2/modular_sdk/connections/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/connections/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1754 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/connections/mongodb_connection.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4723 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/connections/rabbit_connection.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.599098 modular_sdk-5.1.2/modular_sdk/helpers/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/helpers/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      985 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/helpers/response_helper.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.603098 modular_sdk-5.1.2/modular_sdk/models/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/models/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2125 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/models/application.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      929 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/models/base_meta.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      837 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/models/customer.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      746 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/models/customer_settings.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1050 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/models/execution_trace.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      490 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/models/heartbeat.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1163 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/models/job.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      662 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/models/operation_mode.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3804 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/models/parent.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.603098 modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:25.000000 modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    22977 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/base_model.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2261 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/base_role_access_model.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     7095 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/base_safe_update_model.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    18251 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      811 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2565 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/models/region.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      476 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/models/setting.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4813 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/models/tenant.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1081 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/models/tenant_settings.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    11580 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/modular.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.607098 modular_sdk-5.1.2/modular_sdk/services/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     7399 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/application_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4559 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/aws_creds_provider.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1311 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/customer_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1828 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/customer_settings_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     5073 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/environment_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      618 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/events_service.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.607098 modular_sdk-5.1.2/modular_sdk/services/impl/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/impl/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    25795 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/impl/maestro_credentials_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     9500 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/impl/maestro_rabbit_transport_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2913 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/job_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      620 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/lambda_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    19869 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/parent_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3751 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/rabbit_transport_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2602 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/region_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     9806 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/settings_management_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1488 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/sqs_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     7547 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/ssm_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     8390 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/sts_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     8722 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/tenant_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2935 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/tenant_settings_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      745 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/services/thread_local_storage_service.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.607098 modular_sdk-5.1.2/modular_sdk/utils/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/utils/__init__.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.611098 modular_sdk-5.1.2/modular_sdk/utils/job_tracer/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/utils/job_tracer/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      360 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/utils/job_tracer/abstract.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3854 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/utils/job_tracer/generic.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.611098 modular_sdk-5.1.2/modular_sdk/utils/operation_mode/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/utils/operation_mode/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      776 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/utils/operation_mode/abstract.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2171 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/utils/operation_mode/generic.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.611098 modular_sdk-5.1.2/modular_sdk/utils/runtime_tracer/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/utils/runtime_tracer/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1061 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/utils/runtime_tracer/abstract.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4091 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/modular_sdk/utils/runtime_tracer/generic.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-05-13 14:52:48.611098 modular_sdk-5.1.2/modular_sdk.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     5144 2024-05-13 14:52:48.000000 modular_sdk-5.1.2/modular_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2944 2024-05-13 14:52:48.000000 modular_sdk-5.1.2/modular_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        1 2024-05-13 14:52:48.000000 modular_sdk-5.1.2/modular_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      273 2024-05-13 14:52:48.000000 modular_sdk-5.1.2/modular_sdk.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)       18 2024-05-13 14:52:48.000000 modular_sdk-5.1.2/modular_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      339 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/pyproject.toml
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1133 2024-05-13 14:52:48.611098 modular_sdk-5.1.2/setup.cfg
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)       38 2024-05-13 14:52:26.000000 modular_sdk-5.1.2/setup.py
```

### Comparing `modular_sdk-5.1.1/LICENSE` & `modular_sdk-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/PKG-INFO` & `modular_sdk-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular_sdk
-Version: 5.1.1
+Version: 5.1.2
 Summary: Data level integration for services built atop of Modular Framework
 Home-page: https://github.com/epam/modular-sdk
 Author: EPAM Systems
 Author-email: support@syndicate.team
 License: Apache-2.0
 Project-URL: GitHub, https://github.com/epam/modular-sdk
 Project-URL: Documentation, https://github.com/epam/modular-sdk/blob/main/README.md
```

### Comparing `modular_sdk-5.1.1/README.md` & `modular_sdk-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/commons/__init__.py` & `modular_sdk-5.1.2/modular_sdk/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/commons/constants.py` & `modular_sdk-5.1.2/modular_sdk/commons/constants.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/commons/error_helper.py` & `modular_sdk-5.1.2/modular_sdk/commons/error_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/commons/helpers.py` & `modular_sdk-5.1.2/modular_sdk/commons/helpers.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/commons/log_helper.py` & `modular_sdk-5.1.2/modular_sdk/commons/log_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/commons/time_helper.py` & `modular_sdk-5.1.2/modular_sdk/commons/time_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/commons/trace_helper.py` & `modular_sdk-5.1.2/modular_sdk/commons/trace_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/connections/mongodb_connection.py` & `modular_sdk-5.1.2/modular_sdk/connections/mongodb_connection.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/connections/rabbit_connection.py` & `modular_sdk-5.1.2/modular_sdk/connections/rabbit_connection.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/helpers/response_helper.py` & `modular_sdk-5.1.2/modular_sdk/helpers/response_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/application.py` & `modular_sdk-5.1.2/modular_sdk/models/application.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/base_meta.py` & `modular_sdk-5.1.2/modular_sdk/models/base_meta.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/customer.py` & `modular_sdk-5.1.2/modular_sdk/models/customer.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/customer_settings.py` & `modular_sdk-5.1.2/modular_sdk/models/customer_settings.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/execution_trace.py` & `modular_sdk-5.1.2/modular_sdk/models/execution_trace.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/job.py` & `modular_sdk-5.1.2/modular_sdk/models/job.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/operation_mode.py` & `modular_sdk-5.1.2/modular_sdk/models/operation_mode.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/parent.py` & `modular_sdk-5.1.2/modular_sdk/models/parent.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/base_model.py` & `modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/base_model.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/base_role_access_model.py` & `modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/base_role_access_model.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/base_safe_update_model.py` & `modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/base_safe_update_model.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py` & `modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py` & `modular_sdk-5.1.2/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/region.py` & `modular_sdk-5.1.2/modular_sdk/models/region.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/tenant.py` & `modular_sdk-5.1.2/modular_sdk/models/tenant.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/models/tenant_settings.py` & `modular_sdk-5.1.2/modular_sdk/models/tenant_settings.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/modular.py` & `modular_sdk-5.1.2/modular_sdk/modular.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/application_service.py` & `modular_sdk-5.1.2/modular_sdk/services/application_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/aws_creds_provider.py` & `modular_sdk-5.1.2/modular_sdk/services/aws_creds_provider.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/customer_service.py` & `modular_sdk-5.1.2/modular_sdk/services/customer_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/customer_settings_service.py` & `modular_sdk-5.1.2/modular_sdk/services/customer_settings_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/environment_service.py` & `modular_sdk-5.1.2/modular_sdk/services/environment_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/events_service.py` & `modular_sdk-5.1.2/modular_sdk/services/events_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/impl/maestro_credentials_service.py` & `modular_sdk-5.1.2/modular_sdk/services/impl/maestro_credentials_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/impl/maestro_rabbit_transport_service.py` & `modular_sdk-5.1.2/modular_sdk/services/impl/maestro_rabbit_transport_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/job_service.py` & `modular_sdk-5.1.2/modular_sdk/services/job_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/lambda_service.py` & `modular_sdk-5.1.2/modular_sdk/services/lambda_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/parent_service.py` & `modular_sdk-5.1.2/modular_sdk/services/parent_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/rabbit_transport_service.py` & `modular_sdk-5.1.2/modular_sdk/services/rabbit_transport_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/region_service.py` & `modular_sdk-5.1.2/modular_sdk/services/region_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/settings_management_service.py` & `modular_sdk-5.1.2/modular_sdk/services/settings_management_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/sqs_service.py` & `modular_sdk-5.1.2/modular_sdk/services/sqs_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/ssm_service.py` & `modular_sdk-5.1.2/modular_sdk/services/ssm_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,21 @@
 
     def get_parameter(self, name: str) -> Optional[SecretValue]:
         try:
             response = self.client.secrets.kv.v2.read_secret_version(
                 path=name, mount_point=self.mount_point) or {}
         except Exception:  # hvac.InvalidPath
             return
-        return response.get('data', {}).get('data', {}).get(self.key)
+        val = response.get('data', {}).get('data', {}).get(self.key)
+        if isinstance(val, str):
+            try:
+                val = json.loads(val)
+            except json.JSONDecodeError:
+                pass
+        return val
 
     def put_parameter(self, name: str, value: SecretValue,
                       _type='SecureString') -> Optional[str]:
         self.client.secrets.kv.v2.create_or_update_secret(
             path=name,
             secret={self.key: value},
             mount_point=self.mount_point
```

### Comparing `modular_sdk-5.1.1/modular_sdk/services/sts_service.py` & `modular_sdk-5.1.2/modular_sdk/services/sts_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/tenant_service.py` & `modular_sdk-5.1.2/modular_sdk/services/tenant_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/tenant_settings_service.py` & `modular_sdk-5.1.2/modular_sdk/services/tenant_settings_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/services/thread_local_storage_service.py` & `modular_sdk-5.1.2/modular_sdk/services/thread_local_storage_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/utils/job_tracer/generic.py` & `modular_sdk-5.1.2/modular_sdk/utils/job_tracer/generic.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/utils/operation_mode/abstract.py` & `modular_sdk-5.1.2/modular_sdk/utils/operation_mode/abstract.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/utils/operation_mode/generic.py` & `modular_sdk-5.1.2/modular_sdk/utils/operation_mode/generic.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/utils/runtime_tracer/abstract.py` & `modular_sdk-5.1.2/modular_sdk/utils/runtime_tracer/abstract.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk/utils/runtime_tracer/generic.py` & `modular_sdk-5.1.2/modular_sdk/utils/runtime_tracer/generic.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/modular_sdk.egg-info/PKG-INFO` & `modular_sdk-5.1.2/modular_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular_sdk
-Version: 5.1.1
+Version: 5.1.2
 Summary: Data level integration for services built atop of Modular Framework
 Home-page: https://github.com/epam/modular-sdk
 Author: EPAM Systems
 Author-email: support@syndicate.team
 License: Apache-2.0
 Project-URL: GitHub, https://github.com/epam/modular-sdk
 Project-URL: Documentation, https://github.com/epam/modular-sdk/blob/main/README.md
```

### Comparing `modular_sdk-5.1.1/modular_sdk.egg-info/SOURCES.txt` & `modular_sdk-5.1.2/modular_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modular_sdk-5.1.1/setup.cfg` & `modular_sdk-5.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = modular_sdk
-version = 5.1.1
+version = 5.1.2
 python_requires = >=3.10
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 license = Apache-2.0
 description = Data level integration for services built atop of Modular Framework
```

