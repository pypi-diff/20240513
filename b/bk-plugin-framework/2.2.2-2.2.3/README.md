# Comparing `tmp/bk-plugin-framework-2.2.2.tar.gz` & `tmp/bk-plugin-framework-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk-plugin-framework-2.2.2.tar", max compression
+gzip compressed data, was "bk-plugin-framework-2.2.3.tar", max compression
```

## Comparing `bk-plugin-framework-2.2.2.tar` & `bk-plugin-framework-2.2.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/__init__.py
--rw-r--r--   0        0        0      753 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/__version__.py
--rw-r--r--   0        0        0      846 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/constants.py
--rw-r--r--   0        0        0     2946 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/envs.py
--rw-r--r--   0        0        0     2439 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/hub/__init__.py
--rw-r--r--   0        0        0      941 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/kit/__init__.py
--rw-r--r--   0        0        0     2130 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/kit/api.py
--rw-r--r--   0        0        0      938 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/kit/authentication.py
--rw-r--r--   0        0        0     1496 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/kit/decorators.py
--rw-r--r--   0        0        0     7746 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/kit/plugin.py
--rw-r--r--   0        0        0     4262 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/metrics.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/__init__.py
--rw-r--r--   0        0        0      811 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/__init__.py
--rw-r--r--   0        0        0     4365 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/api.py
--rw-r--r--   0        0        0      923 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/apps.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/celery/__init__.py
--rw-r--r--   0        0        0      915 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/celery/queues.py
--rw-r--r--   0        0        0     3669 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/celery/tasks.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/migrations/__init__.py
--rw-r--r--   0        0        0     1858 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callbacker.py
--rw-r--r--   0        0        0    14138 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/executor.py
--rw-r--r--   0        0        0      807 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/__init__.py
--rw-r--r--   0        0        0      986 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/admin.py
--rw-r--r--   0        0        0      846 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/apps.py
--rw-r--r--   0        0        0     1354 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/log.py
--rw-r--r--   0        0        0     1574 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/migrations/__init__.py
--rw-r--r--   0        0        0     1422 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/models.py
--rw-r--r--   0        0        0      811 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/__init__.py
--rw-r--r--   0        0        0     1022 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/admin.py
--rw-r--r--   0        0        0      948 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/apps.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/celery/__init__.py
--rw-r--r--   0        0        0     1051 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/celery/beat.py
--rw-r--r--   0        0        0     1011 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/celery/queues.py
--rw-r--r--   0        0        0     2560 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/celery/tasks.py
--rw-r--r--   0        0        0     1649 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/migrations/0001_initial.py
--rw-r--r--   0        0        0      407 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/migrations/0002_schedule_finish_at.py
--rw-r--r--   0        0        0      552 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/migrations/0003_auto_20210830_1945.py
--rw-r--r--   0        0        0      430 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/migrations/0004_schedule_scheduling.py
--rw-r--r--   0        0        0      458 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/migrations/0005_schedule_err.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/migrations/__init__.py
--rw-r--r--   0        0        0     2324 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/models.py
--rw-r--r--   0        0        0     1372 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/utils.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/__init__.py
--rw-r--r--   0        0        0      817 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/__init__.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/admin.py
--rw-r--r--   0        0        0     1006 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/__init__.py
--rw-r--r--   0        0        0     2504 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/callback.py
--rw-r--r--   0        0        0     3613 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/detail.py
--rw-r--r--   0        0        0     4350 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/invoke.py
--rw-r--r--   0        0        0     2078 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/logs.py
--rw-r--r--   0        0        0     3534 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/meta.py
--rw-r--r--   0        0        0     1213 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/permissions.py
--rw-r--r--   0        0        0     6028 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/plugin_api_dispatch.py
--rw-r--r--   0        0        0     3961 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/schedule.py
--rw-r--r--   0        0        0      997 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/serializers/__init__.py
--rw-r--r--   0        0        0     1046 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/apps.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/management/__init__.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/management/commands/__init__.py
--rw-r--r--   0        0        0      462 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/management/commands/data/api-definition.yml
--rw-r--r--   0        0        0     3166 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/management/commands/data/api-resources.yml
--rw-r--r--   0        0        0      401 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/management/commands/data/api-strategy-cors.yml
--rw-r--r--   0        0        0     2308 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/management/commands/sync_plugin_apigw.py
--rw-r--r--   0        0        0     1093 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/middlewares.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/migrations/__init__.py
--rw-r--r--   0        0        0     1766 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/urls.py
--rw-r--r--   0        0        0        0 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/debug_panel/__init__.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/debug_panel/management/commands/__init__.py
--rw-r--r--   0        0        0     1753 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/debug_panel/management/commands/rundebugserver.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/debug_panel/migrations/__init__.py
--rw-r--r--   0        0        0      997 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/services/debug_panel/views.py
--rw-r--r--   0        0        0      730 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/utils/__init__.py
--rw-r--r--   0        0        0      981 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/utils/local.py
--rw-r--r--   0        0        0      928 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/utils/log.py
--rw-r--r--   0        0        0     1957 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/utils/module_load.py
--rw-r--r--   0        0        0      705 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/bk_plugin_framework/utils/validations.py
--rw-r--r--   0        0        0      754 2024-03-25 12:43:16.774880 bk-plugin-framework-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     1849 2024-03-25 12:43:30.720255 bk-plugin-framework-2.2.2/setup.py
--rw-r--r--   0        0        0      709 2024-03-25 12:43:30.720504 bk-plugin-framework-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/__init__.py
+-rw-r--r--   0        0        0      753 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/__version__.py
+-rw-r--r--   0        0        0      846 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/constants.py
+-rw-r--r--   0        0        0     2946 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/envs.py
+-rw-r--r--   0        0        0     2439 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/hub/__init__.py
+-rw-r--r--   0        0        0      941 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/kit/__init__.py
+-rw-r--r--   0        0        0     2130 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/kit/api.py
+-rw-r--r--   0        0        0      938 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/kit/authentication.py
+-rw-r--r--   0        0        0     1496 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/kit/decorators.py
+-rw-r--r--   0        0        0     7746 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/kit/plugin.py
+-rw-r--r--   0        0        0     4262 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/metrics.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/__init__.py
+-rw-r--r--   0        0        0      811 2024-05-13 12:00:17.385020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/__init__.py
+-rw-r--r--   0        0        0     4365 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/api.py
+-rw-r--r--   0        0        0      923 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/apps.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/celery/__init__.py
+-rw-r--r--   0        0        0      915 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/celery/queues.py
+-rw-r--r--   0        0        0     3669 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/celery/tasks.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/migrations/__init__.py
+-rw-r--r--   0        0        0     1858 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callbacker.py
+-rw-r--r--   0        0        0    14138 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/executor.py
+-rw-r--r--   0        0        0      807 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/__init__.py
+-rw-r--r--   0        0        0      986 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/admin.py
+-rw-r--r--   0        0        0      846 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/apps.py
+-rw-r--r--   0        0        0     1354 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/log.py
+-rw-r--r--   0        0        0     1574 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/migrations/__init__.py
+-rw-r--r--   0        0        0     1422 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/models.py
+-rw-r--r--   0        0        0      811 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/__init__.py
+-rw-r--r--   0        0        0     1022 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/admin.py
+-rw-r--r--   0        0        0      948 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/apps.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/celery/__init__.py
+-rw-r--r--   0        0        0     1051 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/celery/beat.py
+-rw-r--r--   0        0        0     1011 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/celery/queues.py
+-rw-r--r--   0        0        0     2560 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/celery/tasks.py
+-rw-r--r--   0        0        0     1649 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/migrations/0001_initial.py
+-rw-r--r--   0        0        0      407 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/migrations/0002_schedule_finish_at.py
+-rw-r--r--   0        0        0      552 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/migrations/0003_auto_20210830_1945.py
+-rw-r--r--   0        0        0      430 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/migrations/0004_schedule_scheduling.py
+-rw-r--r--   0        0        0      458 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/migrations/0005_schedule_err.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/migrations/__init__.py
+-rw-r--r--   0        0        0     2324 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/models.py
+-rw-r--r--   0        0        0     1372 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/utils.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/__init__.py
+-rw-r--r--   0        0        0      817 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/__init__.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/admin.py
+-rw-r--r--   0        0        0     1006 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/__init__.py
+-rw-r--r--   0        0        0     2504 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/callback.py
+-rw-r--r--   0        0        0     3613 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/detail.py
+-rw-r--r--   0        0        0     4350 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/invoke.py
+-rw-r--r--   0        0        0     2078 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/logs.py
+-rw-r--r--   0        0        0     3534 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/meta.py
+-rw-r--r--   0        0        0     1213 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/permissions.py
+-rw-r--r--   0        0        0     6028 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/plugin_api_dispatch.py
+-rw-r--r--   0        0        0     3961 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/schedule.py
+-rw-r--r--   0        0        0      997 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/serializers/__init__.py
+-rw-r--r--   0        0        0     1046 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/apps.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/management/__init__.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/management/commands/__init__.py
+-rw-r--r--   0        0        0      503 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/management/commands/data/api-definition.yml
+-rw-r--r--   0        0        0     3166 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/management/commands/data/api-resources.yml
+-rw-r--r--   0        0        0      401 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/management/commands/data/api-strategy-cors.yml
+-rw-r--r--   0        0        0     2308 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/management/commands/sync_plugin_apigw.py
+-rw-r--r--   0        0        0     1093 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/middlewares.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/migrations/__init__.py
+-rw-r--r--   0        0        0     1766 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/urls.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/debug_panel/__init__.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/debug_panel/management/commands/__init__.py
+-rw-r--r--   0        0        0     1753 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/debug_panel/management/commands/rundebugserver.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/debug_panel/migrations/__init__.py
+-rw-r--r--   0        0        0      997 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/services/debug_panel/views.py
+-rw-r--r--   0        0        0      730 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/utils/__init__.py
+-rw-r--r--   0        0        0      981 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/utils/local.py
+-rw-r--r--   0        0        0      928 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/utils/log.py
+-rw-r--r--   0        0        0     1957 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/utils/module_load.py
+-rw-r--r--   0        0        0      705 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/bk_plugin_framework/utils/validations.py
+-rw-r--r--   0        0        0      754 2024-05-13 12:00:17.389020 bk-plugin-framework-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1849 2024-05-13 12:00:31.623146 bk-plugin-framework-2.2.3/setup.py
+-rw-r--r--   0        0        0      709 2024-05-13 12:00:31.623393 bk-plugin-framework-2.2.3/PKG-INFO
```

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/__version__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/__version__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/constants.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/constants.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/envs.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/envs.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/hub/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/kit/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/kit/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/kit/api.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/kit/api.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/kit/authentication.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/kit/authentication.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/kit/decorators.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/kit/decorators.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/kit/plugin.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/kit/plugin.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/metrics.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/metrics.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/api.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/api.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/apps.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/apps.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/celery/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/celery/queues.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/celery/queues.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/celery/tasks.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callback/migrations/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callback/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/callbacker.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/callbacker.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/executor.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/executor.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/admin.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/admin.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/apps.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/apps.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/log.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/log.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/migrations/0001_initial.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/loghub/models.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/loghub/models.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/admin.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/admin.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/apps.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/apps.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/celery/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/celery/beat.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/celery/beat.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/celery/queues.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/celery/queues.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/celery/tasks.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/migrations/0001_initial.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/migrations/0003_auto_20210830_1945.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/migrations/0003_auto_20210830_1945.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/migrations/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/models.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/models.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/runtime/schedule/utils.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/runtime/schedule/utils.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/admin.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/admin.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/callback.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/callback.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/detail.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/detail.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/invoke.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/invoke.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/logs.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/logs.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/meta.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/meta.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/permissions.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/permissions.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/plugin_api_dispatch.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/plugin_api_dispatch.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/schedule.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/schedule.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/api/serializers/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/apps.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/apps.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/management/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/management/commands/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/management/commands/data/api-resources.yml` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/management/commands/data/api-resources.yml`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/management/commands/sync_plugin_apigw.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/management/commands/sync_plugin_apigw.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/middlewares.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/middlewares.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/migrations/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/bpf_service/urls.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/bpf_service/urls.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/debug_panel/management/commands/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/debug_panel/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/debug_panel/management/commands/rundebugserver.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/debug_panel/management/commands/rundebugserver.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/debug_panel/migrations/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/debug_panel/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/services/debug_panel/views.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/services/debug_panel/views.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/utils/__init__.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/utils/local.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/utils/local.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/utils/log.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/utils/log.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/utils/module_load.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/utils/module_load.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/bk_plugin_framework/utils/validations.py` & `bk-plugin-framework-2.2.3/bk_plugin_framework/utils/validations.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.2.2/pyproject.toml` & `bk-plugin-framework-2.2.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "bk-plugin-framework"
-version = "2.2.2"
+version = "2.2.3"
 description = "bk plugin python framework"
 authors = ["Your Name <you@example.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.6.1,<4.0"
 pydantic = "^1.0"
 werkzeug = "^2.0.0"
 apigw-manager = {version = ">=1.0.6, <1.2.0", extras = ["extra"]}
-bk-plugin-runtime = "2.0.5"
+bk-plugin-runtime = "2.0.6"
 jsonschema = ">=2.5.0,<5.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.0"
 black = "^20.8b1"
 pytest-django = "^4.5.2"
 coverage = "^6.2"
```

### Comparing `bk-plugin-framework-2.2.2/setup.py` & `bk-plugin-framework-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,22 +28,22 @@
 
 package_data = \
 {'': ['*'],
  'bk_plugin_framework.services.bpf_service.management.commands': ['data/*']}
 
 install_requires = \
 ['apigw-manager[extra]>=1.0.6,<1.2.0',
- 'bk-plugin-runtime==2.0.5',
+ 'bk-plugin-runtime==2.0.6',
  'jsonschema>=2.5.0,<5.0.0',
  'pydantic>=1.0,<2.0',
  'werkzeug>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'bk-plugin-framework',
-    'version': '2.2.2',
+    'version': '2.2.3',
     'description': 'bk plugin python framework',
     'long_description': None,
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `bk-plugin-framework-2.2.2/PKG-INFO` & `bk-plugin-framework-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bk-plugin-framework
-Version: 2.2.2
+Version: 2.2.3
 Summary: bk plugin python framework
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: apigw-manager[extra] (>=1.0.6,<1.2.0)
-Requires-Dist: bk-plugin-runtime (==2.0.5)
+Requires-Dist: bk-plugin-runtime (==2.0.6)
 Requires-Dist: jsonschema (>=2.5.0,<5.0.0)
 Requires-Dist: pydantic (>=1.0,<2.0)
 Requires-Dist: werkzeug (>=2.0.0,<3.0.0)
```

