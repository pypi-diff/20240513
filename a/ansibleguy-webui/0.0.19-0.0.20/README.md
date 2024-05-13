# Comparing `tmp/ansibleguy_webui-0.0.19.tar.gz` & `tmp/ansibleguy_webui-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansibleguy_webui-0.0.19.tar", last modified: Sun May 12 16:25:44 2024, max compression
+gzip compressed data, was "ansibleguy_webui-0.0.20.tar", last modified: Mon May 13 20:10:02 2024, max compression
```

## Comparing `ansibleguy_webui-0.0.19.tar` & `ansibleguy_webui-0.0.20.tar`

### file list

```diff
@@ -1,211 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.280806 ansibleguy_webui-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (127)    33252 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43911 2024-05-12 16:25:44.280806 ansibleguy_webui-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 16:25:42.000000 ansibleguy_webui-0.0.19/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 16:25:44.280806 ansibleguy_webui-0.0.19/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.248806 ansibleguy_webui-0.0.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.248806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.252806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.252806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21503 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    18404 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/job_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/key.py
--rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.256806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/form_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/hardcoded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.256806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/features.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.256806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.260806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/alert_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.260806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    40135 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0004_v0_0_15.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0005_v0_0_18.py
--rw-r--r--   0 runner    (1001) docker     (127)    14987 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0006_v0_0_19.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.260806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/job_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.244806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.260806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/css/aw.css
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/css/aw_mobile.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.260806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/img/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.264806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    17643 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/aw.js
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/aw_nav.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.264806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/credentials.js
--rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/edit.js
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/logs.js
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/manage.js
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/repository.js
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/login.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.264806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/alert.js
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/api_key.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/environment.js
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/permission.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.264806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/body.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.264806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/autoRefresh.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.268806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/add.html
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/add_dir.html
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/add_git.html
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/collapse.html
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/copy.html
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/delete.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/download.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/edit.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/expand.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/return.html
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/run.html
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/sort.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/stop.html
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/refresh.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.268806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/django_saml2_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/django_saml2_auth/denied.html
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/django_saml2_auth/error.html
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/django_saml2_auth/signout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.268806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/email/
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/email/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.268806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/error/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/error/403.html
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/error/500.html
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/error/js_disabled.html
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/fallback.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.268806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/job.html
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/snippet.html
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/snippet_test.html
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/head.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.272806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/credentials.html
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/manage.html
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/repository.html
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/nav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.272806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/password_change_done.html
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/password_change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/remember_user.html
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/saml.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.272806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/rest_framework/api.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.272806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/alert.html
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/alert_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/api_key.html
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/permission.html
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/permission_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.272806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/system/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/system/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/system/environment.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.276806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/form_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.276806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/subps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/util_no_config.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/util_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.276806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.280806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/cli_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/handle_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/web_serve_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/webserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.280806 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43911 2024-05-12 16:25:44.000000 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-05-12 16:25:44.000000 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 16:25:44.000000 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-12 16:25:44.000000 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 16:25:44.000000 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.464903 ansibleguy_webui-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (127)    33252 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43936 2024-05-13 20:10:02.464903 ansibleguy_webui-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 20:10:00.000000 ansibleguy_webui-0.0.20/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:10:02.464903 ansibleguy_webui-0.0.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.428903 ansibleguy_webui-0.0.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.432903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.432903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.436903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21503 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18404 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/job_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.436903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/form_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/hardcoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.440903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.440903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.440903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.444903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    40135 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0004_v0_0_15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0005_v0_0_18.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14987 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0006_v0_0_19.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.444903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/job_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.428903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.444903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/css/aw.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/css/aw_mobile.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.444903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/img/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.444903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    17643 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/aw.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/aw_nav.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.448903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/credentials.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/edit.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/logs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/manage.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/repository.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/login.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.448903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/alert.js
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/api_key.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/environment.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/permission.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.448903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/body.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.448903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/autoRefresh.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.452903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/add.html
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/add_dir.html
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/add_git.html
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/copy.html
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/download.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/expand.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/return.html
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/run.html
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/sort.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/stop.html
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/refresh.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.452903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/django_saml2_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/django_saml2_auth/denied.html
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/django_saml2_auth/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/django_saml2_auth/signout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.452903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/email/
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/email/alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/email/alert.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.452903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/error/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/error/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/error/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/error/js_disabled.html
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/fallback.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.452903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/job.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/snippet.html
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/snippet_test.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/head.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/credentials.html
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/manage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/repository.html
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/nav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/password_change_done.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/password_change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/remember_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/saml.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/rest_framework/api.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/alert_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/api_key.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/permission.html
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/permission_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/system/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/system/environment.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/form_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.460903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/subps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/util_no_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.460903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.464903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/cli_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/handle_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/web_serve_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.464903 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43936 2024-05-13 20:10:02.000000 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-13 20:10:02.000000 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:10:02.000000 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 20:10:02.000000 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 20:10:02.000000 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/top_level.txt
```

### Comparing `ansibleguy_webui-0.0.19/LICENSE.txt` & `ansibleguy_webui-0.0.20/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/PKG-INFO` & `ansibleguy_webui-0.0.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansibleguy-webui
-Version: 0.0.19
+Version: 0.0.20
 Summary: Basic WebUI for using Ansible
 Author-email: AnsibleGuy <contact@ansibleguy.net>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -667,14 +667,15 @@
 Requires-Dist: djangorestframework-api-key==2.*
 Requires-Dist: drf-spectacular
 Requires-Dist: fontawesomefree
 Requires-Dist: crontab
 Requires-Dist: ansible-core
 Requires-Dist: ansible-runner
 Requires-Dist: PyYAML
+Requires-Dist: premailer
 
 # Basic WebUI for using Ansible
 
 <a href='https://ko-fi.com/ansible0guy' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy me a coffee' />
 
 [![Documentation](https://readthedocs.org/projects/ansible-webui/badge/?version=latest)](https://webui.ansibleguy.net/en/latest/?badge=latest)
 [![Lint](https://github.com/ansibleguy/webui/actions/workflows/lint.yml/badge.svg?branch=latest)](https://github.com/ansibleguy/webui/actions/workflows/lint.yml)
```

### Comparing `ansibleguy_webui-0.0.19/README.md` & `ansibleguy_webui-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/pyproject.toml` & `ansibleguy_webui-0.0.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,12 +29,12 @@
 dependencies = {file = ["requirements.txt"]}
 version = {file = ["VERSION"]}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-"*" = ["*.html", "*.js", "*.css", "*.svg"]
+"*" = ["*.html", "*.js", "*.css", "*.svg", "*.txt"]
 
 # [project.scripts]
 # ansibleguy-webui = "ansibleguy-webui.__main__"
 # ansibleguy-webui-db = "ansibleguy-webui.manage"
```

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/__main__.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/__main__.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/admin.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/admin.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/alert.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/alert.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/base.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/base.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/credentials.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/credentials.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/filesystem.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/filesystem.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/job.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/job.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/job_util.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/job_util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/key.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/key.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/permission.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/permission.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/repository.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/repository.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/system.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/system.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/apps.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/apps.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/defaults.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/environment.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from os import environ
 from functools import cache
 
 from aw.config.defaults import CONFIG_DEFAULTS
 from aw.config.hardcoded import ENV_KEY_CONFIG, ENV_KEY_SAML
 
 AW_ENV_VARS = {
+    'hostnames': ['AW_HOSTNAMES'],
     'port': ['AW_PORT'],
+    'proxy': ['AW_PROXY'],
     'address': ['AW_LISTEN', 'AW_LISTEN_ADDRESS'],
     'timezone': ['AW_TIMEZONE'],
     'secret': ['AW_SECRET'],
     'path_run': ['AW_PATH_RUN'],
     'path_play': ['AW_PATH_PLAY', 'ANSIBLE_PLAYBOOK_DIR'],
     'version': ['AW_VERSION'],
     'deployment': ['AW_ENV'],
```

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/form_metadata.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/form_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,16 @@
             'session_timeout': 'Timeout for WebUI login-sessions',
             'path_ansible_config': 'Ansible Config-File',
             'path_ssh_known_hosts': 'SSH Known-Hosts File',
             'debug': 'Debug Mode',
             # env-vars
             'timezone': 'Timezone',
             'db': 'Database',
+            'hostnames': 'Hostnames',
+            'proxy': 'Using Proxy',
             'db_migrate': 'Database auto-upgrade',
             'serve_static': 'Serving static files',
             'deployment': 'Deployment',
             'version': 'AnsibleGuy WebUI Version',
             'logo_url': 'URL to a Logo to use',
             'ara_server': 'ARA Server URL',
             'global_environment_vars': 'Global Environmental Variables',
@@ -220,12 +222,12 @@
                           'Documentation - Integrations</a>',
             'global_environment_vars': 'Set environmental variables that will be added to every job execution. '
                                        'Comma-separated list of key-value pairs. (VAR1=TEST1,VAR2=0)',
             'mail_server': 'Mail Server to use for Alert Mails. Combination of server and port (default 25)',
             'mail_ssl_verify': 'En- or disable SSL certificate verification. '
                                'If enabled - the certificate SAN has to contain the mail-server FQDN '
                                'and must be issued from a trusted CA',
-            'mail_sender': 'Mail Sender Address to use for Alert Mails',
+            'mail_sender': 'Mail Sender Address to use for Alert Mails. Fallback is mail-user',
             'mail_transport': 'The default port mapping is: 25 = Unencrypted, 465 = SSL, 587 = StartTLS',
         }
     }
 }
```

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/hardcoded.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/hardcoded.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/main.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/main.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/navigation.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/navigation.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/alert.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_email.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_email.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 import ssl
 from pathlib import Path
 from smtplib import SMTP, SMTP_SSL, SMTPResponseException
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 
 from django.template.loader import get_template
+from premailer import transform as html_transform_styles
 
 from aw.base import USERS
 from aw.utils.util import valid_email, is_set
 from aw.utils.debug import log
 from aw.config.main import config
 from aw.model.job import JobExecution
 from aw.settings import get_main_web_address
 from aw.model.system import MAIL_TRANSPORT_TYPE_SSL, MAIL_TRANSPORT_TYPE_STARTTLS
 
 
 def _email_send(server: SMTP, user: USERS, stats: dict, execution: JobExecution, error_msgs: dict):
-    server.login(user=config['mail_user'], password=config['mail_pass'])
+    if is_set(config['mail_pass']):
+        server.login(user=config['mail_user'], password=config['mail_pass'])
+
     msg = MIMEMultipart('alternative')
     msg['Subject'] = f"Ansible WebUI - Job '{execution.job.name}' - {execution.status_name}"
-    msg['From'] = config['mail_sender']
+    msg['From'] = config['mail_sender'] if is_set(config['mail_sender']) else config['mail_user']
     msg['To'] = user.email
 
     tmpl_html, tmpl_text = 'email/alert.html', 'email/alert.txt'
-    if is_set(config['path_template']):
+    if is_set(config['path_template']):  # custom templates
         _tmpl_base = Path(config['path_template'])
         _tmpl_html = _tmpl_base / 'alert.html'
         _tmpl_text = _tmpl_base / 'alert.txt'
         if _tmpl_html.is_file():
             tmpl_html = str(_tmpl_html)
 
         if _tmpl_text.is_file():
             tmpl_text = str(_tmpl_text)
 
     tmpl_ctx = {'execution': execution, 'stats': stats, 'web_addr': get_main_web_address(), 'error_msgs': error_msgs}
     text_content = get_template(tmpl_text).render(tmpl_ctx)
     html_content = get_template(tmpl_html).render(tmpl_ctx)
+    html_content = html_transform_styles(html=html_content, pretty_print=True, allow_network=False)
 
     msg.attach(MIMEText(text_content, 'plain'))
     msg.attach(MIMEText(html_content, 'html'))
 
     server.sendmail(
         from_addr=config['mail_sender'],
         to_addrs=user.email,
```

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_wrapper.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_wrapper.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play_credentials.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play_credentials.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play_util.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play_util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/queue.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/queue.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/repository.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/repository.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/scheduler.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/scheduler.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/threader.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/threader.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/util.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0006_v0_0_19.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0006_v0_0_19.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/alert.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/alert.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/base.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/base.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/job.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/job.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/job_credential.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/job_credential.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/permission.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/permission.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/repository.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/repository.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/system.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/system.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/settings.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # pylint-django
     from aw.config.main import init_config
     init_config()
     from aw.config.main import config, VERSION
 
 
 from aw.config.hardcoded import LOGIN_PATH, ENV_KEY_CONFIG, ENV_KEY_SAML
-from aw.config.defaults import CONFIG_DEFAULTS
+from aw.config.defaults import CONFIG_DEFAULTS, inside_docker
 from aw.utils.deployment import deployment_dev, deployment_prod
 from aw.config.environment import get_aw_env_var_or_default, auth_mode_saml
 from aw.utils.debug import log
 
 BASE_DIR = Path(__file__).resolve().parent.parent
 TEMPLATE_DIRS = [
     BASE_DIR / 'aw' / 'templates/'
@@ -153,15 +153,16 @@
 
 
 def get_main_web_address() -> str:
     if 'AW_HOSTNAMES' not in environ:
         return f'http://localhost:{PORT_WEB}'
 
     _hostname = environ['AW_HOSTNAMES'].split(',', 1)[0]
-    if 'AW_PROXY' in environ:  # we will not know what port the proxy is serving this service.. assume its 443
+    if 'AW_PROXY' in environ or inside_docker():
+        # we will not know what port the proxy is serving this service - assume its 443
         return f'https://{_hostname}'
 
     return f'https://{_hostname}:{PORT_WEB}'
 
 
 if 'AW_PROXY' in environ:
     SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')
```

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/css/aw.css` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/css/aw.css`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/css/aw_mobile.css` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/css/aw_mobile.css`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/img/logo.svg` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/aw.js` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/aw.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/aw_nav.js` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/aw_nav.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/credentials.js` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/credentials.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/edit.js` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/edit.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/logs.js` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/logs.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/manage.js` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/manage.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/repository.js` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/repository.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/login.js` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/login.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/alert.js` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/alert.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/api_key.js` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/api_key.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/permission.js` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/permission.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/body.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/body.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/email/alert.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/email/alert.html`

 * *Files 11% similar despite different names*

```diff
@@ -3,22 +3,16 @@
 <html>
     <head>
         <meta charset="utf-8">
         <style>
             body {
                 padding: 0 0;
                 margin: 0 0;
-                background-color: var(--bg) !important;
-                color: var(--tc1);
-                --bg: #fcfdff;
-                --tc1: #121212;
-            }
-            @media (prefers-color-scheme: dark) {
-                --bg: #121212;
-                --tc1: #fcfdff;
+                background-color: #fcfdff;
+                color: #121212;
             }
             .aw-log-ok, .aw-stats-ok {
                 color: #11D116;
             }
             .aw-log-skip, .aw-stats-skipped, .aw-stats-ignored {
                 color: #1AB899;
             }
```

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/job.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/job.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/snippet.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/snippet.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/head.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/head.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/credentials.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/credentials.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/edit.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/edit.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/logs.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/logs.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/manage.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/manage.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/repository.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/repository.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/nav.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/nav.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/login.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/password_change_done.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/password_change_form.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/saml.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/saml.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/rest_framework/api.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/alert.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/alert.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/api_key.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/api_key.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/permission.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/permission.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/system/config.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/system/config.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/system/environment.html` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/system/environment.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/form_util.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/form_util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/util.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/urls.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/urls.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/crypto.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/debug.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/debug.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/deployment.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/deployment.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/http.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/http.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/permission.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/permission.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/subps.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/subps.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/util.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/version.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/version.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/base.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/base.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/auth.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/auth.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/job.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/job.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/settings.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/settings.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/system.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/system.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/job.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/job.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/main.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/main.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/settings.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/settings.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/system.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/system.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/cli.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/cli.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/cli_init.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/cli_init.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/db.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/db.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/handle_signals.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/handle_signals.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/main.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/main.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/manage.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/manage.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/web_serve_static.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/web_serve_static.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy-webui/webserver.py` & `ansibleguy_webui-0.0.20/src/ansibleguy-webui/webserver.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/PKG-INFO` & `ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansibleguy-webui
-Version: 0.0.19
+Version: 0.0.20
 Summary: Basic WebUI for using Ansible
 Author-email: AnsibleGuy <contact@ansibleguy.net>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -667,14 +667,15 @@
 Requires-Dist: djangorestframework-api-key==2.*
 Requires-Dist: drf-spectacular
 Requires-Dist: fontawesomefree
 Requires-Dist: crontab
 Requires-Dist: ansible-core
 Requires-Dist: ansible-runner
 Requires-Dist: PyYAML
+Requires-Dist: premailer
 
 # Basic WebUI for using Ansible
 
 <a href='https://ko-fi.com/ansible0guy' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy me a coffee' />
 
 [![Documentation](https://readthedocs.org/projects/ansible-webui/badge/?version=latest)](https://webui.ansibleguy.net/en/latest/?badge=latest)
 [![Lint](https://github.com/ansibleguy/webui/actions/workflows/lint.yml/badge.svg?branch=latest)](https://github.com/ansibleguy/webui/actions/workflows/lint.yml)
```

### Comparing `ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/SOURCES.txt` & `ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 src/ansibleguy-webui/aw/templates/button/icon/run.html
 src/ansibleguy-webui/aw/templates/button/icon/sort.html
 src/ansibleguy-webui/aw/templates/button/icon/stop.html
 src/ansibleguy-webui/aw/templates/django_saml2_auth/denied.html
 src/ansibleguy-webui/aw/templates/django_saml2_auth/error.html
 src/ansibleguy-webui/aw/templates/django_saml2_auth/signout.html
 src/ansibleguy-webui/aw/templates/email/alert.html
+src/ansibleguy-webui/aw/templates/email/alert.txt
 src/ansibleguy-webui/aw/templates/error/403.html
 src/ansibleguy-webui/aw/templates/error/500.html
 src/ansibleguy-webui/aw/templates/error/js_disabled.html
 src/ansibleguy-webui/aw/templates/forms/base.html
 src/ansibleguy-webui/aw/templates/forms/job.html
 src/ansibleguy-webui/aw/templates/forms/snippet.html
 src/ansibleguy-webui/aw/templates/forms/snippet_test.html
```

