# Comparing `tmp/blueapps-4.9.0.tar.gz` & `tmp/blueapps-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blueapps-4.9.0.tar", last modified: Thu Jan 11 13:51:58 2024, max compression
+gzip compressed data, was "dist/blueapps-4.9.1.tar", last modified: Tue Jan 16 01:49:16 2024, max compression
```

## Comparing `blueapps-4.9.0.tar` & `blueapps-4.9.1.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/
--rw-r--r--   0 root         (0) root         (0)      833 2024-01-11 13:49:20.000000 blueapps-4.9.0/test.py
--rw-r--r--   0 root         (0) root         (0)      311 2024-01-11 13:49:20.000000 blueapps-4.9.0/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/apigw_sync/
--rw-r--r--   0 root         (0) root         (0)      160 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/apigw_sync/apps.py
--rw-r--r--   0 root         (0) root         (0)     2524 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/apigw_sync/apigw_sync_settings.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/apigw_sync/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/apigw_sync/management/
--rw-r--r--   0 root         (0) root         (0)      745 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/apigw_sync/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/apigw_sync/management/commands/
--rw-r--r--   0 root         (0) root         (0)      745 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/apigw_sync/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3214 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/apigw_sync/management/commands/sync_saas_apigw.py
--rw-r--r--   0 root         (0) root         (0)     1490 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/apigw_sync/management/commands/generate_api_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/apigw_sync/management/commands/data/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/apigw_sync/management/commands/data/api-resources.yml
--rw-r--r--   0 root         (0) root         (0)     2640 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/apigw_sync/management/commands/data/apigw-definition.yml
--rw-r--r--   0 root         (0) root         (0)     1529 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/apigw_sync/management/commands/generate_apigw_definition.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1809 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/middleware/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/middleware/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/middleware/xss/
--rw-r--r--   0 root         (0) root         (0)     4230 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/middleware/xss/utils.py
--rw-r--r--   0 root         (0) root         (0)     6141 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/middleware/xss/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/middleware/xss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2516 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/middleware/xss/decorators.py
--rw-r--r--   0 root         (0) root         (0)     7918 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/middleware/xss/pxfilter.py
--rw-r--r--   0 root         (0) root         (0)      842 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/middleware/request_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/middleware/bkui/
--rw-r--r--   0 root         (0) root         (0)     1296 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/middleware/bkui/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/middleware/bkui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/utils/
--rw-r--r--   0 root         (0) root         (0)     1119 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/fancy_dict.py
--rw-r--r--   0 root         (0) root         (0)      837 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/unique.py
--rw-r--r--   0 root         (0) root         (0)     1999 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2112 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/crypto.py
--rw-r--r--   0 root         (0) root         (0)     4673 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/request_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/utils/sites/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/utils/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)     1427 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/sites/tencent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/utils/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)     1432 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/sites/ieod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/utils/sites/open/
--rw-r--r--   0 root         (0) root         (0)     1337 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/sites/open/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8325 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/esbclient.py
--rw-r--r--   0 root         (0) root         (0)     1274 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      884 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     2887 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/utils/jwt_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/opentelemetry/
--rw-r--r--   0 root         (0) root         (0)     1389 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/opentelemetry/metrics/
--rw-r--r--   0 root         (0) root         (0)     2658 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/metrics/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      931 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/metrics/server.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/metrics/celery.py
--rw-r--r--   0 root         (0) root         (0)     3500 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/metrics/instrumentor.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/opentelemetry/instrument_app/
--rw-r--r--   0 root         (0) root         (0)     1059 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/instrument_app/apps.py
--rw-r--r--   0 root         (0) root         (0)      837 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/instrument_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/instrument_app/celery.py
--rw-r--r--   0 root         (0) root         (0)     5064 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/setup.py
--rw-r--r--   0 root         (0) root         (0)     1859 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/export.py
--rw-r--r--   0 root         (0) root         (0)     4566 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/instrumentor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/opentelemetry/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/opentelemetry/docs/assets/
--rw-r--r--   0 root         (0) root         (0)   169851 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/docs/assets/local_jaeger.png
--rw-r--r--   0 root         (0) root         (0)     1420 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/docs/metric.md
--rw-r--r--   0 root         (0) root         (0)     3491 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/docs/trace.md
--rw-r--r--   0 root         (0) root         (0)      671 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/README.md
--rw-r--r--   0 root         (0) root         (0)      891 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/opentelemetry/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/core/handler/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/core/handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1593 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/core/handler/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/core/celery/
--rw-r--r--   0 root         (0) root         (0)      835 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/core/celery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1685 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/core/celery/celery.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/core/sites/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/core/sites/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/core/sites/middleware.py
--rw-r--r--   0 root         (0) root         (0)     1409 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/core/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/core/exceptions/
--rw-r--r--   0 root         (0) root         (0)     1520 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/core/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3687 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/core/exceptions/base.py
--rw-r--r--   0 root         (0) root         (0)     3796 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/core/exceptions/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/conf/
--rw-r--r--   0 root         (0) root         (0)     2119 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/conf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/conf/sites/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/conf/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/conf/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)      986 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/conf/sites/tencent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/conf/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)      942 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/conf/sites/ieod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/conf/sites/open/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/conf/sites/open/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1912 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/conf/database.py
--rw-r--r--   0 root         (0) root         (0)     5600 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/conf/log.py
--rw-r--r--   0 root         (0) root         (0)     5445 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/conf/default_settings.py
--rw-r--r--   0 root         (0) root         (0)     3047 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/conf/validators.py
--rw-r--r--   0 root         (0) root         (0)     4096 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/conf/environ.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/dummy/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/dummy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1005 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/dummy/dummy_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/patch/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/patch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5565 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/patch/settings_open_saas.py
--rw-r--r--   0 root         (0) root         (0)     3773 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/patch/log.py
--rw-r--r--   0 root         (0) root         (0)     1745 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/patch/settings_paas_services.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/
--rw-r--r--   0 root         (0) root         (0)     8615 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/components/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/components/ptlogin/
--rw-r--r--   0 root         (0) root         (0)     1023 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/ptlogin/models.py
--rw-r--r--   0 root         (0) root         (0)     3668 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/ptlogin/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/ptlogin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4030 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/ptlogin/backends.py
--rw-r--r--   0 root         (0) root         (0)     1490 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/ptlogin/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/components/weixin/
--rw-r--r--   0 root         (0) root         (0)     4669 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/weixin/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/weixin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4045 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/weixin/backends.py
--rw-r--r--   0 root         (0) root         (0)      907 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/weixin/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/components/bk_jwt/
--rw-r--r--   0 root         (0) root         (0)     2307 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_jwt/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_jwt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5752 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_jwt/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/components/bk_ticket/
--rw-r--r--   0 root         (0) root         (0)     1023 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_ticket/models.py
--rw-r--r--   0 root         (0) root         (0)     3634 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_ticket/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_ticket/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3344 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_ticket/backends.py
--rw-r--r--   0 root         (0) root         (0)      919 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_ticket/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/components/rio/
--rw-r--r--   0 root         (0) root         (0)     3337 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/rio/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/rio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5699 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/rio/backends.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/rio/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/components/null/
--rw-r--r--   0 root         (0) root         (0)      941 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/null/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/components/bk_token/
--rw-r--r--   0 root         (0) root         (0)     1023 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_token/models.py
--rw-r--r--   0 root         (0) root         (0)     4072 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_token/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9552 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_token/backends.py
--rw-r--r--   0 root         (0) root         (0)      916 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/components/bk_token/forms.py
--rw-r--r--   0 root         (0) root         (0)     2850 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/static/account/
--rw-r--r--   0 root         (0) root         (0)     2049 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/static/account/login.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/migrations/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/migrations/0004_create_cache_table.py
--rw-r--r--   0 root         (0) root         (0)     7369 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/migrations/0005_auto_20230818_2320.py
--rw-r--r--   0 root         (0) root         (0)     1866 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/migrations/0003_verifyinfo.py
--rw-r--r--   0 root         (0) root         (0)     1285 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/migrations/0002_init_superuser.py
--rw-r--r--   0 root         (0) root         (0)     1523 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/middlewares.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/handlers/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6812 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/handlers/response.py
--rw-r--r--   0 root         (0) root         (0)     1287 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2165 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/views.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/sites/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/sites/tencent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2025 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/sites/tencent/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/sites/ieod/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2213 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/sites/ieod/conf.py
--rw-r--r--   0 root         (0) root         (0)     2686 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/sites/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/sites/open/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/sites/open/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1976 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/sites/open/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/utils/
--rw-r--r--   0 root         (0) root         (0)      940 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4127 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     1765 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/utils/sms.py
--rw-r--r--   0 root         (0) root         (0)     1946 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/readme.md
--rw-r--r--   0 root         (0) root         (0)     1324 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/urls.py
--rw-r--r--   0 root         (0) root         (0)     1249 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/backends.py
--rw-r--r--   0 root         (0) root         (0)     1122 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/signals.py
--rw-r--r--   0 root         (0) root         (0)     1899 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/management/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/management/commands/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1079 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/management/commands/apigw_clean_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/account/templates/account/
--rw-r--r--   0 root         (0) root         (0)     1905 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/templates/account/login_page.html
--rw-r--r--   0 root         (0) root         (0)     1355 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/templates/account/login_success.html
--rw-r--r--   0 root         (0) root         (0)      645 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/templates/account/login_forbidden.html
--rw-r--r--   0 root         (0) root         (0)     2626 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/conf.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/account/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/contrib/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/
--rw-r--r--   0 root         (0) root         (0)      833 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/test.py
--rw-r--r--   0 root         (0) root         (0)     1041 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/handlers/
--rw-r--r--   0 root         (0) root         (0)     6356 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/__init__.py
--rw-r--r--   0 root         (0) root         (0)      917 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/app.py
--rw-r--r--   0 root         (0) root         (0)     5954 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/base.py
--rw-r--r--   0 root         (0) root         (0)     7158 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/commands/
--rw-r--r--   0 root         (0) root         (0)      931 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2489 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py
--rw-r--r--   0 root         (0) root         (0)     1868 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/commands/celerybeat.py
--rw-r--r--   0 root         (0) root         (0)     1898 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/contrib/bk_commands/management/commands/celery.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/template/
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/template/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps/template/backends/
--rw-r--r--   0 root         (0) root         (0)     4226 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/template/backends/mako.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/template/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3260 2024-01-11 13:49:20.000000 blueapps-4.9.0/blueapps/template/context_processors.py
--rw-r--r--   0 root         (0) root         (0)     4147 2024-01-11 13:49:20.000000 blueapps-4.9.0/setup.py
--rw-r--r--   0 root         (0) root         (0)       67 2024-01-11 13:51:58.000000 blueapps-4.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3492 2024-01-11 13:49:20.000000 blueapps-4.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps.egg-info/
--rw-r--r--   0 root         (0) root         (0)       68 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     6791 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        9 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1042 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     4359 2024-01-11 13:51:58.000000 blueapps-4.9.0/blueapps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4359 2024-01-11 13:51:58.000000 blueapps-4.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7810 2024-01-11 13:49:20.000000 blueapps-4.9.0/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/
+-rw-r--r--   0 root         (0) root         (0)      833 2024-01-16 01:46:29.000000 blueapps-4.9.1/test.py
+-rw-r--r--   0 root         (0) root         (0)      311 2024-01-16 01:46:29.000000 blueapps-4.9.1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/apigw_sync/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/apigw_sync/apps.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/apigw_sync/apigw_sync_settings.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/apigw_sync/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/apigw_sync/management/
+-rw-r--r--   0 root         (0) root         (0)      745 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/apigw_sync/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/apigw_sync/management/commands/
+-rw-r--r--   0 root         (0) root         (0)      745 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/apigw_sync/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3214 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/apigw_sync/management/commands/sync_saas_apigw.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/apigw_sync/management/commands/generate_api_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/apigw_sync/management/commands/data/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/apigw_sync/management/commands/data/api-resources.yml
+-rw-r--r--   0 root         (0) root         (0)     2640 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/apigw_sync/management/commands/data/apigw-definition.yml
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/apigw_sync/management/commands/generate_apigw_definition.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/middleware/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/middleware/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/middleware/xss/
+-rw-r--r--   0 root         (0) root         (0)     4230 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/middleware/xss/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/middleware/xss/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/middleware/xss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/middleware/xss/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     7918 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/middleware/xss/pxfilter.py
+-rw-r--r--   0 root         (0) root         (0)      842 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/middleware/request_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/middleware/bkui/
+-rw-r--r--   0 root         (0) root         (0)     1296 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/middleware/bkui/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/middleware/bkui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/utils/
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/fancy_dict.py
+-rw-r--r--   0 root         (0) root         (0)      837 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/unique.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/crypto.py
+-rw-r--r--   0 root         (0) root         (0)     4673 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/request_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/utils/sites/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/utils/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/sites/tencent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/utils/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)     1432 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/sites/ieod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/utils/sites/open/
+-rw-r--r--   0 root         (0) root         (0)     1337 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/sites/open/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/esbclient.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      884 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2887 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/utils/jwt_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/opentelemetry/
+-rw-r--r--   0 root         (0) root         (0)     1389 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/opentelemetry/metrics/
+-rw-r--r--   0 root         (0) root         (0)     2658 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/metrics/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      931 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/metrics/server.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/metrics/celery.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/metrics/instrumentor.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/opentelemetry/instrument_app/
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/instrument_app/apps.py
+-rw-r--r--   0 root         (0) root         (0)      837 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/instrument_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/instrument_app/celery.py
+-rw-r--r--   0 root         (0) root         (0)     5064 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/export.py
+-rw-r--r--   0 root         (0) root         (0)     4566 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/instrumentor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/opentelemetry/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/opentelemetry/docs/assets/
+-rw-r--r--   0 root         (0) root         (0)   169851 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/docs/assets/local_jaeger.png
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/docs/metric.md
+-rw-r--r--   0 root         (0) root         (0)     3491 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/docs/trace.md
+-rw-r--r--   0 root         (0) root         (0)      671 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/README.md
+-rw-r--r--   0 root         (0) root         (0)      891 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/opentelemetry/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/core/handler/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/core/handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/core/handler/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/core/celery/
+-rw-r--r--   0 root         (0) root         (0)      835 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/core/celery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/core/celery/celery.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/core/sites/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/core/sites/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/core/sites/middleware.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/core/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/core/exceptions/
+-rw-r--r--   0 root         (0) root         (0)     1520 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/core/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3687 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/core/exceptions/base.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/core/exceptions/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/conf/
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/conf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/conf/sites/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/conf/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/conf/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/conf/sites/tencent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/conf/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)      942 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/conf/sites/ieod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/conf/sites/open/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/conf/sites/open/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/conf/database.py
+-rw-r--r--   0 root         (0) root         (0)     5600 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/conf/log.py
+-rw-r--r--   0 root         (0) root         (0)     5484 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/conf/default_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/conf/validators.py
+-rw-r--r--   0 root         (0) root         (0)     4096 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/conf/environ.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/dummy/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/dummy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/dummy/dummy_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/patch/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/patch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/patch/settings_open_saas.py
+-rw-r--r--   0 root         (0) root         (0)     3773 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/patch/log.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/patch/settings_paas_services.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/
+-rw-r--r--   0 root         (0) root         (0)     8615 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/components/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/components/ptlogin/
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/ptlogin/models.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/ptlogin/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/ptlogin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4030 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/ptlogin/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/ptlogin/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/components/weixin/
+-rw-r--r--   0 root         (0) root         (0)     4669 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/weixin/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/weixin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/weixin/backends.py
+-rw-r--r--   0 root         (0) root         (0)      907 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/weixin/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/components/bk_jwt/
+-rw-r--r--   0 root         (0) root         (0)     2307 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_jwt/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_jwt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_jwt/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/components/bk_ticket/
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_ticket/models.py
+-rw-r--r--   0 root         (0) root         (0)     3634 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_ticket/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_ticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_ticket/backends.py
+-rw-r--r--   0 root         (0) root         (0)      919 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_ticket/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/components/rio/
+-rw-r--r--   0 root         (0) root         (0)     3337 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/rio/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/rio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/rio/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/rio/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/components/null/
+-rw-r--r--   0 root         (0) root         (0)      941 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/null/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/components/bk_token/
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_token/models.py
+-rw-r--r--   0 root         (0) root         (0)     4072 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_token/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9552 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_token/backends.py
+-rw-r--r--   0 root         (0) root         (0)      916 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/components/bk_token/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/static/account/
+-rw-r--r--   0 root         (0) root         (0)     2049 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/static/account/login.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/migrations/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/migrations/0004_create_cache_table.py
+-rw-r--r--   0 root         (0) root         (0)     7369 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/migrations/0005_auto_20230818_2320.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/migrations/0003_verifyinfo.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/migrations/0002_init_superuser.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/middlewares.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/handlers/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6812 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/handlers/response.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/views.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/sites/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/sites/tencent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/sites/tencent/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/sites/ieod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/sites/ieod/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/sites/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/sites/open/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/sites/open/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/sites/open/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/utils/
+-rw-r--r--   0 root         (0) root         (0)      940 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/utils/sms.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/readme.md
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/urls.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/signals.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/management/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/management/commands/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/management/commands/apigw_clean_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/account/templates/account/
+-rw-r--r--   0 root         (0) root         (0)     1905 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/templates/account/login_page.html
+-rw-r--r--   0 root         (0) root         (0)     1355 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/templates/account/login_success.html
+-rw-r--r--   0 root         (0) root         (0)      645 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/templates/account/login_forbidden.html
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/conf.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/account/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/contrib/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/
+-rw-r--r--   0 root         (0) root         (0)      833 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/test.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/handlers/
+-rw-r--r--   0 root         (0) root         (0)     6356 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      917 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/app.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/base.py
+-rw-r--r--   0 root         (0) root         (0)     7158 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/templates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/commands/
+-rw-r--r--   0 root         (0) root         (0)      931 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/commands/celerybeat.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/contrib/bk_commands/management/commands/celery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/template/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/template/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps/template/backends/
+-rw-r--r--   0 root         (0) root         (0)     4226 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/template/backends/mako.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/template/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2024-01-16 01:46:29.000000 blueapps-4.9.1/blueapps/template/context_processors.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2024-01-16 01:46:29.000000 blueapps-4.9.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       67 2024-01-16 01:49:16.000000 blueapps-4.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3492 2024-01-16 01:46:29.000000 blueapps-4.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       68 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     6791 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        9 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     4359 2024-01-16 01:49:16.000000 blueapps-4.9.1/blueapps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4359 2024-01-16 01:49:16.000000 blueapps-4.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7810 2024-01-16 01:46:29.000000 blueapps-4.9.1/LICENSE.txt
```

### Comparing `blueapps-4.9.0/test.py` & `blueapps-4.9.1/test.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/apigw_sync/apigw_sync_settings.py` & `blueapps-4.9.1/blueapps/apigw_sync/apigw_sync_settings.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/apigw_sync/management/__init__.py` & `blueapps-4.9.1/blueapps/apigw_sync/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/apigw_sync/management/commands/__init__.py` & `blueapps-4.9.1/blueapps/apigw_sync/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/apigw_sync/management/commands/sync_saas_apigw.py` & `blueapps-4.9.1/blueapps/apigw_sync/management/commands/sync_saas_apigw.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/apigw_sync/management/commands/generate_api_resources.py` & `blueapps-4.9.1/blueapps/apigw_sync/management/commands/generate_api_resources.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/apigw_sync/management/commands/data/api-resources.yml` & `blueapps-4.9.1/blueapps/apigw_sync/management/commands/data/api-resources.yml`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/apigw_sync/management/commands/data/apigw-definition.yml` & `blueapps-4.9.1/blueapps/apigw_sync/management/commands/data/apigw-definition.yml`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/apigw_sync/management/commands/generate_apigw_definition.py` & `blueapps-4.9.1/blueapps/apigw_sync/management/commands/generate_apigw_definition.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/__init__.py` & `blueapps-4.9.1/blueapps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-VERSION = "4.9.0"
+VERSION = "4.9.1"
 __version__ = VERSION
 
 
 RUN_VER = ""
 
 
 def get_run_ver():
```

### Comparing `blueapps-4.9.0/blueapps/metrics.py` & `blueapps-4.9.1/blueapps/metrics.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/middleware/__init__.py` & `blueapps-4.9.1/blueapps/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/middleware/xss/utils.py` & `blueapps-4.9.1/blueapps/middleware/xss/utils.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/middleware/xss/middlewares.py` & `blueapps-4.9.1/blueapps/middleware/xss/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/middleware/xss/__init__.py` & `blueapps-4.9.1/blueapps/middleware/xss/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/middleware/xss/decorators.py` & `blueapps-4.9.1/blueapps/middleware/xss/decorators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/middleware/xss/pxfilter.py` & `blueapps-4.9.1/blueapps/middleware/xss/pxfilter.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/middleware/request_provider.py` & `blueapps-4.9.1/blueapps/middleware/request_provider.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/middleware/bkui/middlewares.py` & `blueapps-4.9.1/blueapps/middleware/bkui/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/middleware/bkui/__init__.py` & `blueapps-4.9.1/blueapps/middleware/bkui/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/fancy_dict.py` & `blueapps-4.9.1/blueapps/utils/fancy_dict.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/unique.py` & `blueapps-4.9.1/blueapps/utils/unique.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/__init__.py` & `blueapps-4.9.1/blueapps/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/crypto.py` & `blueapps-4.9.1/blueapps/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/request_provider.py` & `blueapps-4.9.1/blueapps/utils/request_provider.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/sites/__init__.py` & `blueapps-4.9.1/blueapps/utils/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/sites/tencent/__init__.py` & `blueapps-4.9.1/blueapps/utils/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/sites/ieod/__init__.py` & `blueapps-4.9.1/blueapps/utils/sites/ieod/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/sites/open/__init__.py` & `blueapps-4.9.1/blueapps/utils/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/esbclient.py` & `blueapps-4.9.1/blueapps/utils/esbclient.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/tools.py` & `blueapps-4.9.1/blueapps/utils/tools.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/logger.py` & `blueapps-4.9.1/blueapps/utils/logger.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/utils/jwt_client.py` & `blueapps-4.9.1/blueapps/utils/jwt_client.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/utils.py` & `blueapps-4.9.1/blueapps/opentelemetry/utils.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/metrics/middlewares.py` & `blueapps-4.9.1/blueapps/opentelemetry/metrics/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/metrics/__init__.py` & `blueapps-4.9.1/blueapps/opentelemetry/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/metrics/server.py` & `blueapps-4.9.1/blueapps/opentelemetry/metrics/server.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/metrics/celery.py` & `blueapps-4.9.1/blueapps/opentelemetry/metrics/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/metrics/instrumentor.py` & `blueapps-4.9.1/blueapps/opentelemetry/metrics/instrumentor.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/__init__.py` & `blueapps-4.9.1/blueapps/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/instrument_app/apps.py` & `blueapps-4.9.1/blueapps/opentelemetry/instrument_app/apps.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/instrument_app/__init__.py` & `blueapps-4.9.1/blueapps/opentelemetry/instrument_app/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/instrument_app/celery.py` & `blueapps-4.9.1/blueapps/opentelemetry/instrument_app/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/setup.py` & `blueapps-4.9.1/blueapps/opentelemetry/setup.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/export.py` & `blueapps-4.9.1/blueapps/opentelemetry/export.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/instrumentor.py` & `blueapps-4.9.1/blueapps/opentelemetry/instrumentor.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/docs/assets/local_jaeger.png` & `blueapps-4.9.1/blueapps/opentelemetry/docs/assets/local_jaeger.png`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/docs/metric.md` & `blueapps-4.9.1/blueapps/opentelemetry/docs/metric.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/docs/trace.md` & `blueapps-4.9.1/blueapps/opentelemetry/docs/trace.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/README.md` & `blueapps-4.9.1/blueapps/opentelemetry/README.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/opentelemetry/constants.py` & `blueapps-4.9.1/blueapps/opentelemetry/constants.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/core/handler/__init__.py` & `blueapps-4.9.1/blueapps/core/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/core/handler/wsgi.py` & `blueapps-4.9.1/blueapps/core/handler/wsgi.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/core/celery/__init__.py` & `blueapps-4.9.1/blueapps/core/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/core/celery/celery.py` & `blueapps-4.9.1/blueapps/core/celery/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/core/__init__.py` & `blueapps-4.9.1/blueapps/core/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/core/sites/__init__.py` & `blueapps-4.9.1/blueapps/core/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/core/sites/middleware.py` & `blueapps-4.9.1/blueapps/core/sites/middleware.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/core/wsgi.py` & `blueapps-4.9.1/blueapps/core/wsgi.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/core/exceptions/__init__.py` & `blueapps-4.9.1/blueapps/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/core/exceptions/base.py` & `blueapps-4.9.1/blueapps/core/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/core/exceptions/middleware.py` & `blueapps-4.9.1/blueapps/core/exceptions/middleware.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/conf/__init__.py` & `blueapps-4.9.1/blueapps/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/conf/sites/__init__.py` & `blueapps-4.9.1/blueapps/conf/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/conf/sites/tencent/__init__.py` & `blueapps-4.9.1/blueapps/conf/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/conf/sites/ieod/__init__.py` & `blueapps-4.9.1/blueapps/conf/sites/ieod/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/conf/sites/open/__init__.py` & `blueapps-4.9.1/blueapps/conf/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/conf/database.py` & `blueapps-4.9.1/blueapps/conf/database.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/conf/log.py` & `blueapps-4.9.1/blueapps/conf/log.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/conf/default_settings.py` & `blueapps-4.9.1/blueapps/conf/default_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 # close celery hijack root logger
 CELERYD_HIJACK_ROOT_LOGGER = False
 
 # log_dir_prefix
 LOG_DIR_PREFIX = "/app/v3logs/"
 
 # 登录缓存时间配置, 单位秒（与django cache单位一致）
-LOGIN_CACHE_EXPIRED = 60
+LOGIN_CACHE_EXPIRED = int(os.getenv("LOGIN_CACHE_EXPIRED", 60))
 
 # CELERY与RabbitMQ增加60秒心跳设置项
 BROKER_HEARTBEAT = 60
 
 # OTEL TRACE
 OTEL_BK_DATA_TOKEN = os.getenv("OTEL_BK_DATA_TOKEN", "")
 OTEL_GRPC_HOST = os.getenv("OTEL_GRPC_URL", "")
```

### Comparing `blueapps-4.9.0/blueapps/conf/validators.py` & `blueapps-4.9.1/blueapps/conf/validators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/conf/environ.py` & `blueapps-4.9.1/blueapps/conf/environ.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/dummy/dummy_client.py` & `blueapps-4.9.1/blueapps/dummy/dummy_client.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/patch/__init__.py` & `blueapps-4.9.1/blueapps/patch/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/patch/settings_open_saas.py` & `blueapps-4.9.1/blueapps/patch/settings_open_saas.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/patch/log.py` & `blueapps-4.9.1/blueapps/patch/log.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/patch/settings_paas_services.py` & `blueapps-4.9.1/blueapps/patch/settings_paas_services.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/models.py` & `blueapps-4.9.1/blueapps/account/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/__init__.py` & `blueapps-4.9.1/blueapps/account/components/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/ptlogin/models.py` & `blueapps-4.9.1/blueapps/account/components/ptlogin/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/ptlogin/middlewares.py` & `blueapps-4.9.1/blueapps/account/components/ptlogin/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/ptlogin/__init__.py` & `blueapps-4.9.1/blueapps/account/components/ptlogin/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/ptlogin/backends.py` & `blueapps-4.9.1/blueapps/account/components/ptlogin/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/ptlogin/forms.py` & `blueapps-4.9.1/blueapps/account/components/ptlogin/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/weixin/middlewares.py` & `blueapps-4.9.1/blueapps/account/components/weixin/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/weixin/__init__.py` & `blueapps-4.9.1/blueapps/account/components/weixin/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/weixin/backends.py` & `blueapps-4.9.1/blueapps/account/components/weixin/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/weixin/forms.py` & `blueapps-4.9.1/blueapps/account/components/weixin/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_jwt/middlewares.py` & `blueapps-4.9.1/blueapps/account/components/bk_jwt/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_jwt/__init__.py` & `blueapps-4.9.1/blueapps/account/components/bk_jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_jwt/backends.py` & `blueapps-4.9.1/blueapps/account/components/bk_jwt/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_ticket/models.py` & `blueapps-4.9.1/blueapps/account/components/bk_ticket/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_ticket/middlewares.py` & `blueapps-4.9.1/blueapps/account/components/bk_ticket/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_ticket/__init__.py` & `blueapps-4.9.1/blueapps/account/components/bk_ticket/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_ticket/backends.py` & `blueapps-4.9.1/blueapps/account/components/bk_ticket/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_ticket/forms.py` & `blueapps-4.9.1/blueapps/account/components/bk_ticket/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/rio/middlewares.py` & `blueapps-4.9.1/blueapps/account/components/rio/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/rio/__init__.py` & `blueapps-4.9.1/blueapps/account/components/rio/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/rio/backends.py` & `blueapps-4.9.1/blueapps/account/components/rio/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/rio/forms.py` & `blueapps-4.9.1/blueapps/account/components/rio/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/null/__init__.py` & `blueapps-4.9.1/blueapps/account/components/null/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_token/models.py` & `blueapps-4.9.1/blueapps/account/components/bk_token/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_token/middlewares.py` & `blueapps-4.9.1/blueapps/account/components/bk_token/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_token/__init__.py` & `blueapps-4.9.1/blueapps/account/components/bk_token/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_token/backends.py` & `blueapps-4.9.1/blueapps/account/components/bk_token/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/components/bk_token/forms.py` & `blueapps-4.9.1/blueapps/account/components/bk_token/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/apps.py` & `blueapps-4.9.1/blueapps/account/apps.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/static/account/login.js` & `blueapps-4.9.1/blueapps/account/static/account/login.js`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/migrations/__init__.py` & `blueapps-4.9.1/blueapps/account/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/migrations/0004_create_cache_table.py` & `blueapps-4.9.1/blueapps/account/migrations/0004_create_cache_table.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/migrations/0001_initial.py` & `blueapps-4.9.1/blueapps/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/migrations/0005_auto_20230818_2320.py` & `blueapps-4.9.1/blueapps/account/migrations/0005_auto_20230818_2320.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/migrations/0003_verifyinfo.py` & `blueapps-4.9.1/blueapps/account/migrations/0003_verifyinfo.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/migrations/0002_init_superuser.py` & `blueapps-4.9.1/blueapps/account/migrations/0002_init_superuser.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/middlewares.py` & `blueapps-4.9.1/blueapps/account/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/handlers/__init__.py` & `blueapps-4.9.1/blueapps/account/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/handlers/response.py` & `blueapps-4.9.1/blueapps/account/handlers/response.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/__init__.py` & `blueapps-4.9.1/blueapps/account/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/views.py` & `blueapps-4.9.1/blueapps/account/views.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/decorators.py` & `blueapps-4.9.1/blueapps/account/decorators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/sites/__init__.py` & `blueapps-4.9.1/blueapps/account/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/sites/tencent/__init__.py` & `blueapps-4.9.1/blueapps/account/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/sites/tencent/conf.py` & `blueapps-4.9.1/blueapps/account/sites/tencent/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/sites/ieod/__init__.py` & `blueapps-4.9.1/blueapps/account/sites/ieod/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/sites/ieod/conf.py` & `blueapps-4.9.1/blueapps/account/sites/ieod/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/sites/default.py` & `blueapps-4.9.1/blueapps/account/sites/default.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/sites/open/__init__.py` & `blueapps-4.9.1/blueapps/account/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/sites/open/conf.py` & `blueapps-4.9.1/blueapps/account/sites/open/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/utils/__init__.py` & `blueapps-4.9.1/blueapps/account/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/utils/http.py` & `blueapps-4.9.1/blueapps/account/utils/http.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/utils/sms.py` & `blueapps-4.9.1/blueapps/account/utils/sms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/readme.md` & `blueapps-4.9.1/blueapps/account/readme.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/urls.py` & `blueapps-4.9.1/blueapps/account/urls.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/backends.py` & `blueapps-4.9.1/blueapps/account/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/signals.py` & `blueapps-4.9.1/blueapps/account/signals.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/admin.py` & `blueapps-4.9.1/blueapps/account/admin.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/management/__init__.py` & `blueapps-4.9.1/blueapps/account/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/management/commands/__init__.py` & `blueapps-4.9.1/blueapps/account/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/management/commands/apigw_clean_cache.py` & `blueapps-4.9.1/blueapps/account/management/commands/apigw_clean_cache.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/templates/account/login_page.html` & `blueapps-4.9.1/blueapps/account/templates/account/login_page.html`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/templates/account/login_success.html` & `blueapps-4.9.1/blueapps/account/templates/account/login_success.html`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/templates/account/login_forbidden.html` & `blueapps-4.9.1/blueapps/account/templates/account/login_forbidden.html`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/conf.py` & `blueapps-4.9.1/blueapps/account/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/account/forms.py` & `blueapps-4.9.1/blueapps/account/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/__init__.py` & `blueapps-4.9.1/blueapps/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/test.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/test.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/__init__.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/management/handlers/__init__.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/management/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/management/__init__.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/management/app.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/management/app.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/management/base.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/management/base.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/management/templates.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/management/templates.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/management/commands/__init__.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/management/commands/celerybeat.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/management/commands/celerybeat.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/contrib/bk_commands/management/commands/celery.py` & `blueapps-4.9.1/blueapps/contrib/bk_commands/management/commands/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/template/__init__.py` & `blueapps-4.9.1/blueapps/template/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/template/backends/mako.py` & `blueapps-4.9.1/blueapps/template/backends/mako.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/template/backends/__init__.py` & `blueapps-4.9.1/blueapps/template/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps/template/context_processors.py` & `blueapps-4.9.1/blueapps/template/context_processors.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/setup.py` & `blueapps-4.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/README.md` & `blueapps-4.9.1/README.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps.egg-info/SOURCES.txt` & `blueapps-4.9.1/blueapps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps.egg-info/requires.txt` & `blueapps-4.9.1/blueapps.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `blueapps-4.9.0/blueapps.egg-info/PKG-INFO` & `blueapps-4.9.1/blueapps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapps
-Version: 4.9.0
+Version: 4.9.1
 Summary: development framework for blueking
 Home-page: https://github.com/TencentBlueKing/blueapps
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # 蓝鲸Python开发框架Blueapps
         
@@ -63,11 +63,11 @@
         ## License
         
         基于 MIT 协议， 详细请参考[LICENSE](LICENSE.txt)
         
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: bk-notice
 Provides-Extra: bkcrypto
-Provides-Extra: opentelemetry
 Provides-Extra: apigw-manager
-Provides-Extra: bk-notice
+Provides-Extra: opentelemetry
```

### Comparing `blueapps-4.9.0/PKG-INFO` & `blueapps-4.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapps
-Version: 4.9.0
+Version: 4.9.1
 Summary: development framework for blueking
 Home-page: https://github.com/TencentBlueKing/blueapps
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # 蓝鲸Python开发框架Blueapps
         
@@ -63,11 +63,11 @@
         ## License
         
         基于 MIT 协议， 详细请参考[LICENSE](LICENSE.txt)
         
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: bk-notice
 Provides-Extra: bkcrypto
-Provides-Extra: opentelemetry
 Provides-Extra: apigw-manager
-Provides-Extra: bk-notice
+Provides-Extra: opentelemetry
```

### Comparing `blueapps-4.9.0/LICENSE.txt` & `blueapps-4.9.1/LICENSE.txt`

 * *Files identical despite different names*

