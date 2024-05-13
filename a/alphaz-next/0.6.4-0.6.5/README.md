# Comparing `tmp/alphaz-next-0.6.4.tar.gz` & `tmp/alphaz-next-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.6.4.tar", last modified: Mon May 13 11:35:47 2024, max compression
+gzip compressed data, was "alphaz-next-0.6.5.tar", last modified: Mon May 13 11:44:34 2024, max compression
```

## Comparing `alphaz-next-0.6.4.tar` & `alphaz-next-0.6.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.733655 alphaz-next-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-13 11:35:47.733655 alphaz-next-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.725655 alphaz-next-0.6.4/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.725655 alphaz-next-0.6.4/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.725655 alphaz-next-0.6.4/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.729655 alphaz-next-0.6.4/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.729655 alphaz-next-0.6.4/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/core/responses/ujson_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.729655 alphaz-next-0.6.4/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.725655 alphaz-next-0.6.4/alphaz_next/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.729655 alphaz-next-0.6.4/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.729655 alphaz-next-0.6.4/alphaz_next/models/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.733655 alphaz-next-0.6.4/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/models/config/openapi_config_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.725655 alphaz-next-0.6.4/alphaz_next/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.733655 alphaz-next-0.6.4/alphaz_next/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.733655 alphaz-next-0.6.4/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.733655 alphaz-next-0.6.4/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/utils/logging_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-13 11:35:45.000000 alphaz-next-0.6.4/alphaz_next/utils/loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:47.725655 alphaz-next-0.6.4/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-13 11:35:47.000000 alphaz-next-0.6.4/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-13 11:35:47.000000 alphaz-next-0.6.4/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:35:47.000000 alphaz-next-0.6.4/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-13 11:35:47.000000 alphaz-next-0.6.4/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 11:35:47.000000 alphaz-next-0.6.4/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:35:47.733655 alphaz-next-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-13 11:35:46.000000 alphaz-next-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.832768 alphaz-next-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-13 11:44:34.832768 alphaz-next-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.824768 alphaz-next-0.6.5/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.824768 alphaz-next-0.6.5/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.824768 alphaz-next-0.6.5/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.828768 alphaz-next-0.6.5/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.828768 alphaz-next-0.6.5/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/core/responses/ujson_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.828768 alphaz-next-0.6.5/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.824768 alphaz-next-0.6.5/alphaz_next/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.828768 alphaz-next-0.6.5/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.828768 alphaz-next-0.6.5/alphaz_next/models/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.828768 alphaz-next-0.6.5/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/models/config/openapi_config_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.824768 alphaz-next-0.6.5/alphaz_next/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.828768 alphaz-next-0.6.5/alphaz_next/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.828768 alphaz-next-0.6.5/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.832768 alphaz-next-0.6.5/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/utils/logging_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-13 11:44:29.000000 alphaz-next-0.6.5/alphaz_next/utils/loguru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:44:34.824768 alphaz-next-0.6.5/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-13 11:44:34.000000 alphaz-next-0.6.5/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-13 11:44:34.000000 alphaz-next-0.6.5/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:44:34.000000 alphaz-next-0.6.5/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-13 11:44:34.000000 alphaz-next-0.6.5/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 11:44:34.000000 alphaz-next-0.6.5/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:44:34.832768 alphaz-next-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-13 11:44:33.000000 alphaz-next-0.6.5/setup.py
```

### Comparing `alphaz-next-0.6.4/PKG-INFO` & `alphaz-next-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.6.4
+Version: 0.6.5
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.4.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.5.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.6.4/README.md` & `alphaz-next-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/auth/auth.py` & `alphaz-next-0.6.5/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/_base.py` & `alphaz-next-0.6.5/alphaz_next/core/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # MODULES
 import json
 from typing import Dict, List, Optional, TypedDict, Union
 
 from alphaz_next.core.constants import HeaderEnum
 
 
-class ExtHeaders(TypedDict):
+class ExtHeaders(TypedDict, total=False):
     """
     Represents the extended headers for a response.
 
     Attributes:
-        pagination (Optional[str]): The pagination information.
-        status_description (Optional[Union[str, List[str]]]): The status description.
-        warning (Optional[bool]): Indicates if there is a warning.
+        pagination (str): The pagination information.
+        status_description (Union[str, List[str]]): The status description.
+        warning (bool): Indicates if there is a warning.
     """
 
-    pagination: Optional[str]
-    status_description: Optional[Union[str, List[str]]]
-    warning: Optional[bool]
+    pagination: str
+    status_description: Union[str, List[str]]
+    warning: bool
 
 
 from typing import Dict, Optional
 import json
 
 
 def extend_headers(
```

### Comparing `alphaz-next-0.6.4/alphaz_next/core/_middleware.py` & `alphaz-next-0.6.5/alphaz_next/core/_middleware.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/_telemetry.py` & `alphaz-next-0.6.5/alphaz_next/core/_telemetry.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/application.py` & `alphaz-next-0.6.5/alphaz_next/core/application.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.6.5/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/exceptions.py` & `alphaz-next-0.6.5/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.6.5/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.6.5/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.6.5/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.6.5/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.6.5/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.6.5/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.6.5/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/responses/response.py` & `alphaz-next-0.6.5/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.6.5/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.6.5/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/libs/httpx.py` & `alphaz-next-0.6.5/alphaz_next/libs/httpx.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.6.5/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.6.5/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.6.5/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/models/config/api_config.py` & `alphaz-next-0.6.5/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.6.5/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.6.5/alphaz_next/models/config/config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/models/config/database_config.py` & `alphaz-next-0.6.5/alphaz_next/models/config/database_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.6.5/alphaz_next/models/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.6.5/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.6.5/alphaz_next/tests/utils/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/utils/format.py` & `alphaz-next-0.6.5/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/utils/logger.py` & `alphaz-next-0.6.5/alphaz_next/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.6.5/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next/utils/loguru.py` & `alphaz-next-0.6.5/alphaz_next/utils/loguru.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.6.5/alphaz_next.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.6.4
+Version: 0.6.5
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.4.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.5.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.6.4/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.6.5/alphaz_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.4/setup.py` & `alphaz-next-0.6.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.6.4"
+version = "0.6.5"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 
 EXTRAS_REQUIRE = {
     "dependency-injector": ["dependency-injector"],
```

