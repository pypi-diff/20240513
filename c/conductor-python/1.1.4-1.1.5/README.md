# Comparing `tmp/conductor-python-1.1.4.tar.gz` & `tmp/conductor_python-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conductor-python-1.1.4.tar", last modified: Mon Feb  5 22:01:18 2024, max compression
+gzip compressed data, was "conductor_python-1.1.5.tar", last modified: Mon May 13 15:55:42 2024, max compression
```

## Comparing `conductor-python-1.1.4.tar` & `conductor_python-1.1.5.tar`

### file list

```diff
@@ -1,227 +1,228 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.965081 conductor-python-1.1.4/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-02-05 22:00:56.000000 conductor-python-1.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7651 2024-02-05 22:01:18.965081 conductor-python-1.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6630 2024-02-05 22:00:56.000000 conductor-python-1.1.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1018 2024-02-05 22:01:18.965081 conductor-python-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      171 2024-02-05 22:00:56.000000 conductor-python-1.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.909081 conductor-python-1.1.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.913081 conductor-python-1.1.4/src/conductor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.913081 conductor-python-1.1.4/src/conductor/client/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.917081 conductor-python-1.1.4/src/conductor/client/ai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/ai/__init__.py
--rw-r--r--   0 root         (0) root         (0)      271 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/ai/configuration.py
--rw-r--r--   0 root         (0) root         (0)     2146 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/ai/integrations.py
--rw-r--r--   0 root         (0) root         (0)     5220 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/ai/orchestrator.py
--rw-r--r--   0 root         (0) root         (0)     4557 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/authorization_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.917081 conductor-python-1.1.4/src/conductor/client/automator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/automator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8168 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/automator/task_handler.py
--rw-r--r--   0 root         (0) root         (0)    11409 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/automator/task_runner.py
--rw-r--r--   0 root         (0) root         (0)     4089 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/automator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.917081 conductor-python-1.1.4/src/conductor/client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4489 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/configuration/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.917081 conductor-python-1.1.4/src/conductor/client/configuration/settings/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/configuration/settings/__init__.py
--rw-r--r--   0 root         (0) root         (0)      150 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/configuration/settings/authentication_settings.py
--rw-r--r--   0 root         (0) root         (0)      989 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/configuration/settings/metrics_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.917081 conductor-python-1.1.4/src/conductor/client/event/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/event/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1250 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/event/event_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.921081 conductor-python-1.1.4/src/conductor/client/event/queue/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/event/queue/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1339 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/event/queue/kafka_queue_configuration.py
--rw-r--r--   0 root         (0) root         (0)      851 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/event/queue/queue_configuration.py
--rw-r--r--   0 root         (0) root         (0)      192 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/event/queue/queue_worker_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.921081 conductor-python-1.1.4/src/conductor/client/exceptions/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      446 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/exceptions/api_error.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/exceptions/api_exception_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.921081 conductor-python-1.1.4/src/conductor/client/helpers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6554 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/helpers/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.921081 conductor-python-1.1.4/src/conductor/client/http/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.929081 conductor-python-1.1.4/src/conductor/client/http/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53352 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/application_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    11819 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/authorization_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    33405 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/event_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    29299 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/group_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    90712 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/integration_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    47915 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/metadata_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    30772 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/prompt_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    53765 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/scheduler_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    35501 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/secret_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    66289 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/task_resource_api.py
--rw-r--r--   0 root         (0) root         (0)     7141 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/token_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    17899 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/user_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    19200 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/workflow_bulk_resource_api.py
--rw-r--r--   0 root         (0) root         (0)   123243 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api/workflow_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    28954 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.945081 conductor-python-1.1.4/src/conductor/client/http/models/
--rw-r--r--   0 root         (0) root         (0)     3990 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6113 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/action.py
--rw-r--r--   0 root         (0) root         (0)     4693 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/authorization_request.py
--rw-r--r--   0 root         (0) root         (0)     4031 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/bulk_response.py
--rw-r--r--   0 root         (0) root         (0)     4108 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/conductor_application.py
--rw-r--r--   0 root         (0) root         (0)     7745 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/conductor_user.py
--rw-r--r--   0 root         (0) root         (0)     3869 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/correlation_ids_search_request.py
--rw-r--r--   0 root         (0) root         (0)     2971 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/create_or_update_application_request.py
--rw-r--r--   0 root         (0) root         (0)     5992 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/event_handler.py
--rw-r--r--   0 root         (0) root         (0)     3436 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/external_storage_location.py
--rw-r--r--   0 root         (0) root         (0)     3502 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/generate_token_request.py
--rw-r--r--   0 root         (0) root         (0)     3930 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/group.py
--rw-r--r--   0 root         (0) root         (0)     4149 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/health.py
--rw-r--r--   0 root         (0) root         (0)     4715 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/health_check_status.py
--rw-r--r--   0 root         (0) root         (0)    10565 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/integration.py
--rw-r--r--   0 root         (0) root         (0)     9075 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/integration_api.py
--rw-r--r--   0 root         (0) root         (0)     4454 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/integration_api_update.py
--rw-r--r--   0 root         (0) root         (0)     8468 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/integration_def.py
--rw-r--r--   0 root         (0) root         (0)     5993 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/integration_update.py
--rw-r--r--   0 root         (0) root         (0)     2731 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/permission.py
--rw-r--r--   0 root         (0) root         (0)     4854 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/poll_data.py
--rw-r--r--   0 root         (0) root         (0)     9073 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/prompt_template.py
--rw-r--r--   0 root         (0) root         (0)     7450 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/prompt_test_request.py
--rw-r--r--   0 root         (0) root         (0)     3706 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/rate_limit.py
--rw-r--r--   0 root         (0) root         (0)     6537 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/rerun_workflow_request.py
--rw-r--r--   0 root         (0) root         (0)     2156 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/response.py
--rw-r--r--   0 root         (0) root         (0)     3407 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/role.py
--rw-r--r--   0 root         (0) root         (0)     9583 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/save_schedule_request.py
--rw-r--r--   0 root         (0) root         (0)     3817 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/scrollable_search_result_workflow_summary.py
--rw-r--r--   0 root         (0) root         (0)     3572 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/search_result_task.py
--rw-r--r--   0 root         (0) root         (0)     3677 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/search_result_task_summary.py
--rw-r--r--   0 root         (0) root         (0)     3632 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/search_result_workflow.py
--rw-r--r--   0 root         (0) root         (0)     3962 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/search_result_workflow_schedule_execution_model.py
--rw-r--r--   0 root         (0) root         (0)     3737 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/search_result_workflow_summary.py
--rw-r--r--   0 root         (0) root         (0)     3702 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/skip_task_request.py
--rw-r--r--   0 root         (0) root         (0)     5631 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/start_workflow.py
--rw-r--r--   0 root         (0) root         (0)    10467 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/start_workflow_request.py
--rw-r--r--   0 root         (0) root         (0)     1953 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/state_change_event.py
--rw-r--r--   0 root         (0) root         (0)     5158 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/sub_workflow_params.py
--rw-r--r--   0 root         (0) root         (0)     3718 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/subject_ref.py
--rw-r--r--   0 root         (0) root         (0)     4157 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/tag_object.py
--rw-r--r--   0 root         (0) root         (0)     4148 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/tag_string.py
--rw-r--r--   0 root         (0) root         (0)     3693 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/target_ref.py
--rw-r--r--   0 root         (0) root         (0)    34938 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/task.py
--rw-r--r--   0 root         (0) root         (0)    21491 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/task_def.py
--rw-r--r--   0 root         (0) root         (0)     4916 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/task_details.py
--rw-r--r--   0 root         (0) root         (0)     4083 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/task_exec_log.py
--rw-r--r--   0 root         (0) root         (0)    10711 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/task_result.py
--rw-r--r--   0 root         (0) root         (0)      272 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/task_result_status.py
--rw-r--r--   0 root         (0) root         (0)    17342 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/task_summary.py
--rw-r--r--   0 root         (0) root         (0)      407 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/token.py
--rw-r--r--   0 root         (0) root         (0)     4101 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/upsert_group_request.py
--rw-r--r--   0 root         (0) root         (0)     4697 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/upsert_user_request.py
--rw-r--r--   0 root         (0) root         (0)    25837 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/workflow.py
--rw-r--r--   0 root         (0) root         (0)    17948 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/workflow_def.py
--rw-r--r--   0 root         (0) root         (0)    12696 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/workflow_run.py
--rw-r--r--   0 root         (0) root         (0)    11026 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/workflow_schedule.py
--rw-r--r--   0 root         (0) root         (0)    10715 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/workflow_schedule_execution_model.py
--rw-r--r--   0 root         (0) root         (0)     4769 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/workflow_state_update.py
--rw-r--r--   0 root         (0) root         (0)     6034 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/workflow_status.py
--rw-r--r--   0 root         (0) root         (0)    18136 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/workflow_summary.py
--rw-r--r--   0 root         (0) root         (0)     2876 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/workflow_tag.py
--rw-r--r--   0 root         (0) root         (0)    27000 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/workflow_task.py
--rw-r--r--   0 root         (0) root         (0)    11477 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/models/workflow_test_request.py
--rw-r--r--   0 root         (0) root         (0)    10231 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/rest.py
--rw-r--r--   0 root         (0) root         (0)      345 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/http/thread.py
--rw-r--r--   0 root         (0) root         (0)     3695 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/integration_client.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/metadata_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.949081 conductor-python-1.1.4/src/conductor/client/orkes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.949081 conductor-python-1.1.4/src/conductor/client/orkes/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35385 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/api/tags_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.949081 conductor-python-1.1.4/src/conductor/client/orkes/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/models/access_key.py
--rw-r--r--   0 root         (0) root         (0)      107 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/models/access_key_status.py
--rw-r--r--   0 root         (0) root         (0)      165 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/models/access_type.py
--rw-r--r--   0 root         (0) root         (0)     1409 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/models/created_access_key.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/models/granted_permission.py
--rw-r--r--   0 root         (0) root         (0)      294 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/models/metadata_tag.py
--rw-r--r--   0 root         (0) root         (0)      297 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/models/ratelimit_tag.py
--rw-r--r--   0 root         (0) root         (0)     8561 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/orkes_authorization_client.py
--rw-r--r--   0 root         (0) root         (0)     2142 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/orkes_base_client.py
--rw-r--r--   0 root         (0) root         (0)     3740 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/orkes_integration_client.py
--rw-r--r--   0 root         (0) root         (0)     4173 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/orkes_metadata_client.py
--rw-r--r--   0 root         (0) root         (0)     2525 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/orkes_prompt_client.py
--rw-r--r--   0 root         (0) root         (0)     4009 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/orkes_scheduler_client.py
--rw-r--r--   0 root         (0) root         (0)     1529 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/orkes_secret_client.py
--rw-r--r--   0 root         (0) root         (0)     3512 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/orkes_task_client.py
--rw-r--r--   0 root         (0) root         (0)     7986 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes/orkes_workflow_client.py
--rw-r--r--   0 root         (0) root         (0)     2441 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/orkes_clients.py
--rw-r--r--   0 root         (0) root         (0)     1371 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/prompt_client.py
--rw-r--r--   0 root         (0) root         (0)     2535 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/scheduler_client.py
--rw-r--r--   0 root         (0) root         (0)      974 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/secret_client.py
--rw-r--r--   0 root         (0) root         (0)     2033 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/task_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.953081 conductor-python-1.1.4/src/conductor/client/telemetry/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/telemetry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9334 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/telemetry/metrics_collector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.953081 conductor-python-1.1.4/src/conductor/client/telemetry/model/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/telemetry/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1035 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/telemetry/model/metric_documentation.py
--rw-r--r--   0 root         (0) root         (0)      270 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/telemetry/model/metric_label.py
--rw-r--r--   0 root         (0) root         (0)      716 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/telemetry/model/metric_name.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.953081 conductor-python-1.1.4/src/conductor/client/worker/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/worker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      120 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/worker/exception.py
--rw-r--r--   0 root         (0) root         (0)     5965 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/worker/worker.py
--rw-r--r--   0 root         (0) root         (0)     3492 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/worker/worker_interface.py
--rw-r--r--   0 root         (0) root         (0)     1894 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/worker/worker_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.953081 conductor-python-1.1.4/src/conductor/client/workflow/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14409 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/conductor_workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.953081 conductor-python-1.1.4/src/conductor/client/workflow/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10637 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/executor/workflow_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.961081 conductor-python-1.1.4/src/conductor/client/workflow/task/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1692 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/do_while_task.py
--rw-r--r--   0 root         (0) root         (0)     1402 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/dynamic_fork_task.py
--rw-r--r--   0 root         (0) root         (0)      840 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/dynamic_task.py
--rw-r--r--   0 root         (0) root         (0)     1104 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/event_task.py
--rw-r--r--   0 root         (0) root         (0)     1793 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/fork_task.py
--rw-r--r--   0 root         (0) root         (0)      565 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/get_document.py
--rw-r--r--   0 root         (0) root         (0)     2883 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/http_task.py
--rw-r--r--   0 root         (0) root         (0)     1476 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/human_task.py
--rw-r--r--   0 root         (0) root         (0)      626 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/inline.py
--rw-r--r--   0 root         (0) root         (0)     1035 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/javascript_task.py
--rw-r--r--   0 root         (0) root         (0)      712 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/join_task.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/json_jq_task.py
--rw-r--r--   0 root         (0) root         (0)      608 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/kafka_publish.py
--rw-r--r--   0 root         (0) root         (0)      876 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/kafka_publish_input.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.965081 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_chat_complete.py
--rw-r--r--   0 root         (0) root         (0)      727 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_generate_embeddings.py
--rw-r--r--   0 root         (0) root         (0)     2670 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_index_documents.py
--rw-r--r--   0 root         (0) root         (0)     2037 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_index_text.py
--rw-r--r--   0 root         (0) root         (0)      834 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_query_embeddings.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_search_index.py
--rw-r--r--   0 root         (0) root         (0)     1668 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_text_complete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.965081 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      652 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/utils/embedding_model.py
--rw-r--r--   0 root         (0) root         (0)      647 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/utils/prompt.py
--rw-r--r--   0 root         (0) root         (0)      379 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/set_variable_task.py
--rw-r--r--   0 root         (0) root         (0)      695 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/simple_task.py
--rw-r--r--   0 root         (0) root         (0)      890 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/start_workflow_task.py
--rw-r--r--   0 root         (0) root         (0)     1994 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/sub_workflow_task.py
--rw-r--r--   0 root         (0) root         (0)     2325 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/switch_task.py
--rw-r--r--   0 root         (0) root         (0)     4820 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/task.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/task_type.py
--rw-r--r--   0 root         (0) root         (0)      792 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/terminate_task.py
--rw-r--r--   0 root         (0) root         (0)      126 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/timeout_policy.py
--rw-r--r--   0 root         (0) root         (0)     1468 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/wait_for_webhook_task.py
--rw-r--r--   0 root         (0) root         (0)     1536 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow/task/wait_task.py
--rw-r--r--   0 root         (0) root         (0)     3731 2024-02-05 22:00:56.000000 conductor-python-1.1.4/src/conductor/client/workflow_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 22:01:18.965081 conductor-python-1.1.4/src/conductor_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7651 2024-02-05 22:01:18.000000 conductor-python-1.1.4/src/conductor_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9989 2024-02-05 22:01:18.000000 conductor-python-1.1.4/src/conductor_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-05 22:01:18.000000 conductor-python-1.1.4/src/conductor_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2024-02-05 22:01:18.000000 conductor-python-1.1.4/src/conductor_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-05 22:01:18.000000 conductor-python-1.1.4/src/conductor_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.929597 conductor_python-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-13 15:55:21.000000 conductor_python-1.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10086 2024-05-13 15:55:42.925597 conductor_python-1.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9065 2024-05-13 15:55:21.000000 conductor_python-1.1.5/README.md
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-05-13 15:55:42.929597 conductor_python-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-13 15:55:21.000000 conductor_python-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.869597 conductor_python-1.1.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.873597 conductor_python-1.1.5/src/conductor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.873597 conductor_python-1.1.5/src/conductor/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.877597 conductor_python-1.1.5/src/conductor/client/ai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/ai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      271 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/ai/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/ai/integrations.py
+-rw-r--r--   0 root         (0) root         (0)     5220 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/ai/orchestrator.py
+-rw-r--r--   0 root         (0) root         (0)     4557 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/authorization_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.877597 conductor_python-1.1.5/src/conductor/client/automator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/automator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8168 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/automator/task_handler.py
+-rw-r--r--   0 root         (0) root         (0)    11409 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/automator/task_runner.py
+-rw-r--r--   0 root         (0) root         (0)     4089 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/automator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.877597 conductor_python-1.1.5/src/conductor/client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4489 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/configuration/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.877597 conductor_python-1.1.5/src/conductor/client/configuration/settings/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/configuration/settings/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      150 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/configuration/settings/authentication_settings.py
+-rw-r--r--   0 root         (0) root         (0)      989 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/configuration/settings/metrics_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.877597 conductor_python-1.1.5/src/conductor/client/event/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/event/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/event/event_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.881597 conductor_python-1.1.5/src/conductor/client/event/queue/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/event/queue/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/event/queue/kafka_queue_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      851 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/event/queue/queue_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      192 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/event/queue/queue_worker_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.881597 conductor_python-1.1.5/src/conductor/client/exceptions/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/exceptions/api_error.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/exceptions/api_exception_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.881597 conductor_python-1.1.5/src/conductor/client/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6554 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/helpers/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.881597 conductor_python-1.1.5/src/conductor/client/http/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.889597 conductor_python-1.1.5/src/conductor/client/http/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53352 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/application_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    11819 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/authorization_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    33405 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/event_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    29299 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/group_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    90712 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/integration_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    47915 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/metadata_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    30772 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/prompt_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    53765 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/scheduler_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    35501 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/secret_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    66289 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/task_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)     7141 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/token_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    17899 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/user_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    19200 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/workflow_bulk_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)   123243 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api/workflow_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    28954 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.905597 conductor_python-1.1.5/src/conductor/client/http/models/
+-rw-r--r--   0 root         (0) root         (0)     4057 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6113 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/action.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/authorization_request.py
+-rw-r--r--   0 root         (0) root         (0)     4031 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/bulk_response.py
+-rw-r--r--   0 root         (0) root         (0)     4108 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/conductor_application.py
+-rw-r--r--   0 root         (0) root         (0)     7745 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/conductor_user.py
+-rw-r--r--   0 root         (0) root         (0)     3869 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/correlation_ids_search_request.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/create_or_update_application_request.py
+-rw-r--r--   0 root         (0) root         (0)     5992 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/event_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3436 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/external_storage_location.py
+-rw-r--r--   0 root         (0) root         (0)     3502 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/generate_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/group.py
+-rw-r--r--   0 root         (0) root         (0)     4149 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/health.py
+-rw-r--r--   0 root         (0) root         (0)     4715 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/health_check_status.py
+-rw-r--r--   0 root         (0) root         (0)    10565 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/integration.py
+-rw-r--r--   0 root         (0) root         (0)     9075 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/integration_api.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/integration_api_update.py
+-rw-r--r--   0 root         (0) root         (0)     8468 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/integration_def.py
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/integration_update.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/permission.py
+-rw-r--r--   0 root         (0) root         (0)     4854 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/poll_data.py
+-rw-r--r--   0 root         (0) root         (0)     9073 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/prompt_template.py
+-rw-r--r--   0 root         (0) root         (0)     7450 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/prompt_test_request.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/rate_limit.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/rerun_workflow_request.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/response.py
+-rw-r--r--   0 root         (0) root         (0)     3407 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/role.py
+-rw-r--r--   0 root         (0) root         (0)     9583 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/save_schedule_request.py
+-rw-r--r--   0 root         (0) root         (0)     3817 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/scrollable_search_result_workflow_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/search_result_task.py
+-rw-r--r--   0 root         (0) root         (0)     3677 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/search_result_task_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3632 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/search_result_workflow.py
+-rw-r--r--   0 root         (0) root         (0)     3962 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/search_result_workflow_schedule_execution_model.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/search_result_workflow_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/skip_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     5631 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/start_workflow.py
+-rw-r--r--   0 root         (0) root         (0)    10467 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/start_workflow_request.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/state_change_event.py
+-rw-r--r--   0 root         (0) root         (0)     5158 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/sub_workflow_params.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/subject_ref.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/tag_object.py
+-rw-r--r--   0 root         (0) root         (0)     4148 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/tag_string.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/target_ref.py
+-rw-r--r--   0 root         (0) root         (0)    34938 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/task.py
+-rw-r--r--   0 root         (0) root         (0)    21491 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/task_def.py
+-rw-r--r--   0 root         (0) root         (0)     4916 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/task_details.py
+-rw-r--r--   0 root         (0) root         (0)     4083 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/task_exec_log.py
+-rw-r--r--   0 root         (0) root         (0)    10711 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/task_result.py
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/task_result_status.py
+-rw-r--r--   0 root         (0) root         (0)    17342 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/task_summary.py
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/token.py
+-rw-r--r--   0 root         (0) root         (0)     4101 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/upsert_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     4697 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/upsert_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    25837 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/workflow.py
+-rw-r--r--   0 root         (0) root         (0)    17948 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/workflow_def.py
+-rw-r--r--   0 root         (0) root         (0)    12696 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/workflow_run.py
+-rw-r--r--   0 root         (0) root         (0)    11026 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/workflow_schedule.py
+-rw-r--r--   0 root         (0) root         (0)    10715 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/workflow_schedule_execution_model.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/workflow_state_update.py
+-rw-r--r--   0 root         (0) root         (0)     6730 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/workflow_status.py
+-rw-r--r--   0 root         (0) root         (0)    18136 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/workflow_summary.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/workflow_tag.py
+-rw-r--r--   0 root         (0) root         (0)    27934 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/workflow_task.py
+-rw-r--r--   0 root         (0) root         (0)    11477 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/models/workflow_test_request.py
+-rw-r--r--   0 root         (0) root         (0)    10231 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/rest.py
+-rw-r--r--   0 root         (0) root         (0)      345 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/http/thread.py
+-rw-r--r--   0 root         (0) root         (0)     3695 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/integration_client.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/metadata_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.909597 conductor_python-1.1.5/src/conductor/client/orkes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.909597 conductor_python-1.1.5/src/conductor/client/orkes/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35385 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/api/tags_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.909597 conductor_python-1.1.5/src/conductor/client/orkes/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/models/access_key.py
+-rw-r--r--   0 root         (0) root         (0)      107 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/models/access_key_status.py
+-rw-r--r--   0 root         (0) root         (0)      165 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/models/access_type.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/models/created_access_key.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/models/granted_permission.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/models/metadata_tag.py
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/models/ratelimit_tag.py
+-rw-r--r--   0 root         (0) root         (0)     8561 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/orkes_authorization_client.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/orkes_base_client.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/orkes_integration_client.py
+-rw-r--r--   0 root         (0) root         (0)     4173 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/orkes_metadata_client.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/orkes_prompt_client.py
+-rw-r--r--   0 root         (0) root         (0)     4009 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/orkes_scheduler_client.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/orkes_secret_client.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/orkes_task_client.py
+-rw-r--r--   0 root         (0) root         (0)     7986 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes/orkes_workflow_client.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/orkes_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1371 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/prompt_client.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/scheduler_client.py
+-rw-r--r--   0 root         (0) root         (0)      974 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/secret_client.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/task_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.913597 conductor_python-1.1.5/src/conductor/client/telemetry/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/telemetry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9334 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/telemetry/metrics_collector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.913597 conductor_python-1.1.5/src/conductor/client/telemetry/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/telemetry/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/telemetry/model/metric_documentation.py
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/telemetry/model/metric_label.py
+-rw-r--r--   0 root         (0) root         (0)      716 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/telemetry/model/metric_name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.913597 conductor_python-1.1.5/src/conductor/client/worker/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/worker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      120 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/worker/exception.py
+-rw-r--r--   0 root         (0) root         (0)     5965 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/worker/worker.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/worker/worker_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/worker/worker_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.913597 conductor_python-1.1.5/src/conductor/client/workflow/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14539 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/conductor_workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.913597 conductor_python-1.1.5/src/conductor/client/workflow/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10637 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/executor/workflow_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.921597 conductor_python-1.1.5/src/conductor/client/workflow/task/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/do_while_task.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/dynamic_fork_task.py
+-rw-r--r--   0 root         (0) root         (0)      840 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/dynamic_task.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/event_task.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/fork_task.py
+-rw-r--r--   0 root         (0) root         (0)      565 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/get_document.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/http_poll_task.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/http_task.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/human_task.py
+-rw-r--r--   0 root         (0) root         (0)      626 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/javascript_task.py
+-rw-r--r--   0 root         (0) root         (0)      712 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/join_task.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/json_jq_task.py
+-rw-r--r--   0 root         (0) root         (0)      608 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/kafka_publish.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/kafka_publish_input.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.925597 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_chat_complete.py
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_generate_embeddings.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_index_documents.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_index_text.py
+-rw-r--r--   0 root         (0) root         (0)      834 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_query_embeddings.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_search_index.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_text_complete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.925597 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/utils/embedding_model.py
+-rw-r--r--   0 root         (0) root         (0)      647 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/utils/prompt.py
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/set_variable_task.py
+-rw-r--r--   0 root         (0) root         (0)      695 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/simple_task.py
+-rw-r--r--   0 root         (0) root         (0)      890 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/start_workflow_task.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/sub_workflow_task.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/switch_task.py
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/task.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/task_type.py
+-rw-r--r--   0 root         (0) root         (0)      792 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/terminate_task.py
+-rw-r--r--   0 root         (0) root         (0)      126 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/timeout_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/wait_for_webhook_task.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow/task/wait_task.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2024-05-13 15:55:21.000000 conductor_python-1.1.5/src/conductor/client/workflow_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:55:42.925597 conductor_python-1.1.5/src/conductor_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10086 2024-05-13 15:55:42.000000 conductor_python-1.1.5/src/conductor_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10042 2024-05-13 15:55:42.000000 conductor_python-1.1.5/src/conductor_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 15:55:42.000000 conductor_python-1.1.5/src/conductor_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2024-05-13 15:55:42.000000 conductor_python-1.1.5/src/conductor_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-13 15:55:42.000000 conductor_python-1.1.5/src/conductor_python.egg-info/top_level.txt
```

### Comparing `conductor-python-1.1.4/LICENSE` & `conductor_python-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/PKG-INFO` & `conductor_python-1.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conductor-python
-Version: 1.1.4
+Version: 1.1.5
 Summary: Netflix Conductor Python SDK
 Home-page: https://github.com/conductor-sdk/conductor-python
 Author: Orkes
 Author-email: developers@orkes.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -22,112 +22,102 @@
 Requires-Dist: requests>=2.31.0
 Requires-Dist: typing-extensions>=4.2.0
 Requires-Dist: astor>=0.8.1
 Requires-Dist: shortuuid>=1.0.11
 Requires-Dist: dacite>=1.8.1
 
 # Conductor OSS Python SDK
-Python SDK for working with https://github.com/conductor-oss/conductor
 
-[Conductor](https://www.conductor-oss.org/) is an open source distributed, scalable and highly available 
-orchestration platform that allows developers to build powerful distributed applications.
-You can find the documentation for Conductor here: [Conductor Docs](https://orkes.io/content)
+Python SDK for working with https://github.com/conductor-oss/conductor.
+
+[Conductor](https://www.conductor-oss.org/) is the leading open-source orchestration platform allowing developers to build highly scalable distributed applications.
+
+Check out the [official documentation for Conductor](https://orkes.io/content).
 
 ## ⭐ Conductor OSS
+
 Show support for the Conductor OSS.  Please help spread the awareness by starring Conductor repo.
 
 [![GitHub stars](https://img.shields.io/github/stars/conductor-oss/conductor.svg?style=social&label=Star&maxAge=)](https://GitHub.com/conductor-oss/conductor/)
 
 ## Content
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
-- [Install SDK](#install-sdk)
+- [Install Conductor Python SDK](#install-conductor-python-sdk)
   - [Get Conductor Python SDK](#get-conductor-python-sdk)
-  - [Setup SDK](#setup-sdk)
-- [Start Conductor Server](#start-conductor-server)
-- [Simple Hello World Application using Conductor](#simple-hello-world-application-using-conductor)
-  - [Step 1: Create a Workflow](#step-1-create-a-workflow)
-  - [Step 2: Write Worker](#step-2-write-worker)
-  - [Step 3: Write _your_ application](#step-3-write-_your_-application)
-- [Using Conductor in your application](#using-conductor-in-your-application)
+- [Hello World Application Using Conductor](#hello-world-application-using-conductor)
+  - [Step 1: Create Workflow](#step-1-create-workflow)
+    - [Creating Workflows by Code](#creating-workflows-by-code)
+    - [(Alternatively) Creating Workflows in JSON](#alternatively-creating-workflows-in-json)
+  - [Step 2: Write Task Worker](#step-2-write-task-worker)
+  - [Step 3: Write _Hello World_ Application](#step-3-write-_hello-world_-application)
+- [Running Workflows on Conductor Standalone (Installed Locally)](#running-workflows-on-conductor-standalone-installed-locally)
+  - [Setup Environment Variable](#setup-environment-variable)
+  - [Start Conductor Server](#start-conductor-server)
+  - [Execute Hello World Application](#execute-hello-world-application)
+- [Running Workflows on Orkes Conductor](#running-workflows-on-orkes-conductor)
+- [Learn More about Conductor Python SDK](#learn-more-about-conductor-python-sdk)
   - [Create and Run Conductor Workers](#create-and-run-conductor-workers)
   - [Create Conductor Workflows](#create-conductor-workflows)
   - [Using Conductor in your Application](#using-conductor-in-your-application)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
-## Install SDK
-Create a virtual environment to build your package
+## Install Conductor Python SDK
+
+Before installing Conductor Python SDK, it is a good practice to set up a dedicated virtual environment as follows:
+
 ```shell
 virtualenv conductor
 source conductor/bin/activate
 ```
 
 ### Get Conductor Python SDK
 
-SDK needs Python 3.9+.
+The SDK requires Python 3.9+. To install the SDK, use the following command:
 
 ```shell
 python3 -m pip install conductor-python
 ```
-### Setup SDK
-
-Point the SDK to the Conductor Server API endpoint
-```shell
-export CONDUCTOR_SERVER_URL=http://localhost:8080/api
-```
-(Optionally) If you are using a Conductor server that requires authentication
-
-[How to obtain the key and secret from the conductor server
-](https://orkes.io/content/docs/getting-started/concepts/access-control)
 
+## Hello World Application Using Conductor
 
-```shell
-export CONDUCTOR_AUTH_KEY=your_key
-export CONDUCTOR_AUTH_SECRET=your_key_secret
-```
-
-## Start Conductor Server
-```shell
-docker run --init -p 8080:8080 -p 5000:5000 conductoross/conductor-standalone:3.15.0
-```
-After starting the server navigate to http://localhost:1234 to ensure the server has started successfully.
+In this section, we will create a simple "Hello World" application that executes a "greetings" workflow managed by Conductor.
 
-## Simple Hello World Application using Conductor
-In this section, we will create a simple "Hello World" application that uses Conductor. 
+### Step 1: Create Workflow
 
-### Step 1: Create a Workflow
+#### Creating Workflows by Code
 
-**Use Code to create workflows**
+Create [greetings_workflow.py](examples/helloworld/greetings_workflow.py) with the following:
 
-Create [greetings_workflow.py](examples/greetings_workflow.py) with the following:
 ```python
 from conductor.client.workflow.conductor_workflow import ConductorWorkflow
 from conductor.client.workflow.executor.workflow_executor import WorkflowExecutor
-from greetings import greet
+from greetings_worker import greet
 
 def greetings_workflow(workflow_executor: WorkflowExecutor) -> ConductorWorkflow:
-    name = 'hello'
+    name = 'greetings'
     workflow = ConductorWorkflow(name=name, executor=workflow_executor)
     workflow.version = 1
     workflow >> greet(task_ref_name='greet_ref', name=workflow.input('name'))
     return workflow
 
 
 ```
 
-**(alternatively) Use JSON to create workflows**
+#### (Alternatively) Creating Workflows in JSON
+
+Create `greetings_workflow.json` with the following:
 
-Create workflow.json with the following:
 ```json
 {
-  "name": "hello",
-  "description": "hello workflow",
+  "name": "greetings",
+  "description": "Sample greetings workflow",
   "version": 1,
   "tasks": [
     {
       "name": "greet",
       "taskReferenceName": "greet_ref",
       "type": "SIMPLE",
       "inputParameters": {
@@ -135,40 +125,44 @@
       }
     }
   ],
   "timeoutPolicy": "TIME_OUT_WF",
   "timeoutSeconds": 60
 }
 ```
-Now, register this workflow with the server:
+
+Workflows must be registered to the Conductor server. Use the API to register the greetings workflow from the JSON file above:
 ```shell
 curl -X POST -H "Content-Type:application/json" \
-http://localhost:8080/api/metadata/workflow -d @workflow.json
+http://localhost:8080/api/metadata/workflow -d @greetings_workflow.json
 ```
+> [!note]
+> To use the Conductor API, the Conductor server must be up and running (see [Running over Conductor standalone (installed locally)](#running-over-conductor-standalone-installed-locally)).
 
-### Step 2: Write Worker
+### Step 2: Write Task Worker
 
-Create [greetings.py](examples/greetings.py) with a simple worker and a workflow function.
+Using Python, a worker represents a function with the worker_task decorator. Create [greetings_worker.py](examples/helloworld/greetings_worker.py) file as illustrated below:
 
 > [!note]
-> A single workflow application can have workers written in different languages.
+> A single workflow can have task workers written in different languages and deployed anywhere, making your workflow polyglot and distributed!
 
 ```python
 from conductor.client.worker.worker_task import worker_task
 
 
 @worker_task(task_definition_name='greet')
 def greet(name: str) -> str:
-    return f'Hello my friend {name}'
+    return f'Hello {name}'
 
 ```
+Now, we are ready to write our main application, which will execute our workflow.
 
-### Step 3: Write _your_ application
+### Step 3: Write _Hello World_ Application
 
-Let's add [greetings_main.py](examples/greetings_main.py) with the `main` method:
+Let's add [helloworld.py](examples/helloworld/helloworld.py) with a `main` method:
 
 ```python
 from conductor.client.automator.task_handler import TaskHandler
 from conductor.client.configuration.configuration import Configuration
 from conductor.client.workflow.conductor_workflow import ConductorWorkflow
 from conductor.client.workflow.executor.workflow_executor import WorkflowExecutor
 from greetings_workflow import greetings_workflow
@@ -177,50 +171,101 @@
 def register_workflow(workflow_executor: WorkflowExecutor) -> ConductorWorkflow:
     workflow = greetings_workflow(workflow_executor=workflow_executor)
     workflow.register(True)
     return workflow
 
 
 def main():
-    # points to http://localhost:8080/api by default
+    # The app is connected to http://localhost:8080/api by default
     api_config = Configuration()
 
     workflow_executor = WorkflowExecutor(configuration=api_config)
 
-    # Needs to be done only when registering a workflow one-time
+    # Registering the workflow (Required only when the app is executed the first time)
     workflow = register_workflow(workflow_executor)
 
+    # Starting the worker polling mechanism
     task_handler = TaskHandler(configuration=api_config)
     task_handler.start_processes()
 
     workflow_run = workflow_executor.execute(name=workflow.name, version=workflow.version,
                                              workflow_input={'name': 'Orkes'})
 
     print(f'\nworkflow result: {workflow_run.output["result"]}\n')
     print(f'see the workflow execution here: {api_config.ui_host}/execution/{workflow_run.workflow_id}\n')
     task_handler.stop_processes()
 
 
 if __name__ == '__main__':
     main()
 ```
+## Running Workflows on Conductor Standalone (Installed Locally)
 
-> [!NOTE]
-> That's it - you just created your first distributed python app!
-> 
+### Setup Environment Variable
 
-## Using Conductor in your application
-There are three main ways you will use Conductor when building durable, resilient, distributed applications.
-1. Write service workers that implements business logic to accomplish a specific goal - such as initiate payment transfer, get user information from database etc. 
-2. Create Conductor workflows that implements application state - A typical workflow implements SAGA pattern
-3. Use Conductor SDK and APIs to manage workflows from your application.
+Set the following environment variable to point the SDK to the Conductor Server API endpoint:
 
-In this guide, we will dive deeper into each of these topic.
+```shell
+export CONDUCTOR_SERVER_URL=http://localhost:8080/api
+```
+### Start Conductor Server
 
-### [Create and Run Conductor Workers](workers.md)
-### [Create Conductor Workflows](workflows.md)
-### [Using Conductor in your Application](conductor_apps.md)
+To start the Conductor server in a standalone mode from a Docker image, type the command below:
 
+```shell
+docker run --init -p 8080:8080 -p 5000:5000 conductoross/conductor-standalone:3.15.0
+```
+To ensure the server has started successfully, open Conductor UI on http://localhost:5000.
 
+### Execute Hello World Application
 
+To run the application, type the following command:
 
+```
+python helloworld.py
+```
+
+Now, the workflow is executed, and its execution status can be viewed from Conductor UI (http://localhost:5000).
+
+Navigate to the **Executions** tab to view the workflow execution.
+
+<img width="1434" alt="Screenshot 2024-03-18 at 12 30 07" src="https://github.com/Srividhya-S-Subramanian/conductor-python-v1/assets/163816773/11e829b6-d46a-4b47-b2cf-0bf524a6ebdc">
+
+## Running Workflows on Orkes Conductor
+
+For running the workflow in Orkes Conductor,
+
+- Update the Conductor server URL to your cluster name.
+
+```shell
+export CONDUCTOR_SERVER_URL=https://[cluster-name].orkesconductor.io/api
+```
+
+- If you want to run the workflow on the Orkes Conductor Playground, set the Conductor Server variable as follows:
+
+```shell
+export CONDUCTOR_SERVER_URL=https://play.orkes.io/api
+```
+
+- Orkes Conductor requires authentication. [Obtain the key and secret from the Conductor server](https://orkes.io/content/how-to-videos/access-key-and-secret) and set the following environment variables.
 
+```shell
+export CONDUCTOR_AUTH_KEY=your_key
+export CONDUCTOR_AUTH_SECRET=your_key_secret
+```
+
+Run the application and view the execution status from Conductor's UI Console.
+
+> [!NOTE]
+> That's it - you just created and executed your first distributed Python app!
+
+## Learn More about Conductor Python SDK
+
+There are three main ways you can use Conductor when building durable, resilient, distributed applications.
+
+1. Write service workers that implement business logic to accomplish a specific goal - such as initiating payment transfer, getting user information from the database, etc.
+2. Create Conductor workflows that implement application state - A typical workflow implements the saga pattern.
+3. Use Conductor SDK and APIs to manage workflows from your application.
+
+### [Create and Run Conductor Workers](workers.md)
+### [Create Conductor Workflows](workflows.md)
+### [Using Conductor in your Application](conductor_apps.md)
```

### Comparing `conductor-python-1.1.4/README.md` & `conductor_python-1.1.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,96 @@
 # Conductor OSS Python SDK
-Python SDK for working with https://github.com/conductor-oss/conductor
 
-[Conductor](https://www.conductor-oss.org/) is an open source distributed, scalable and highly available 
-orchestration platform that allows developers to build powerful distributed applications.
-You can find the documentation for Conductor here: [Conductor Docs](https://orkes.io/content)
+Python SDK for working with https://github.com/conductor-oss/conductor.
+
+[Conductor](https://www.conductor-oss.org/) is the leading open-source orchestration platform allowing developers to build highly scalable distributed applications.
+
+Check out the [official documentation for Conductor](https://orkes.io/content).
 
 ## ⭐ Conductor OSS
+
 Show support for the Conductor OSS.  Please help spread the awareness by starring Conductor repo.
 
 [![GitHub stars](https://img.shields.io/github/stars/conductor-oss/conductor.svg?style=social&label=Star&maxAge=)](https://GitHub.com/conductor-oss/conductor/)
 
 ## Content
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
-- [Install SDK](#install-sdk)
+- [Install Conductor Python SDK](#install-conductor-python-sdk)
   - [Get Conductor Python SDK](#get-conductor-python-sdk)
-  - [Setup SDK](#setup-sdk)
-- [Start Conductor Server](#start-conductor-server)
-- [Simple Hello World Application using Conductor](#simple-hello-world-application-using-conductor)
-  - [Step 1: Create a Workflow](#step-1-create-a-workflow)
-  - [Step 2: Write Worker](#step-2-write-worker)
-  - [Step 3: Write _your_ application](#step-3-write-_your_-application)
-- [Using Conductor in your application](#using-conductor-in-your-application)
+- [Hello World Application Using Conductor](#hello-world-application-using-conductor)
+  - [Step 1: Create Workflow](#step-1-create-workflow)
+    - [Creating Workflows by Code](#creating-workflows-by-code)
+    - [(Alternatively) Creating Workflows in JSON](#alternatively-creating-workflows-in-json)
+  - [Step 2: Write Task Worker](#step-2-write-task-worker)
+  - [Step 3: Write _Hello World_ Application](#step-3-write-_hello-world_-application)
+- [Running Workflows on Conductor Standalone (Installed Locally)](#running-workflows-on-conductor-standalone-installed-locally)
+  - [Setup Environment Variable](#setup-environment-variable)
+  - [Start Conductor Server](#start-conductor-server)
+  - [Execute Hello World Application](#execute-hello-world-application)
+- [Running Workflows on Orkes Conductor](#running-workflows-on-orkes-conductor)
+- [Learn More about Conductor Python SDK](#learn-more-about-conductor-python-sdk)
   - [Create and Run Conductor Workers](#create-and-run-conductor-workers)
   - [Create Conductor Workflows](#create-conductor-workflows)
   - [Using Conductor in your Application](#using-conductor-in-your-application)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
-## Install SDK
-Create a virtual environment to build your package
+## Install Conductor Python SDK
+
+Before installing Conductor Python SDK, it is a good practice to set up a dedicated virtual environment as follows:
+
 ```shell
 virtualenv conductor
 source conductor/bin/activate
 ```
 
 ### Get Conductor Python SDK
 
-SDK needs Python 3.9+.
+The SDK requires Python 3.9+. To install the SDK, use the following command:
 
 ```shell
 python3 -m pip install conductor-python
 ```
-### Setup SDK
-
-Point the SDK to the Conductor Server API endpoint
-```shell
-export CONDUCTOR_SERVER_URL=http://localhost:8080/api
-```
-(Optionally) If you are using a Conductor server that requires authentication
-
-[How to obtain the key and secret from the conductor server
-](https://orkes.io/content/docs/getting-started/concepts/access-control)
 
+## Hello World Application Using Conductor
 
-```shell
-export CONDUCTOR_AUTH_KEY=your_key
-export CONDUCTOR_AUTH_SECRET=your_key_secret
-```
-
-## Start Conductor Server
-```shell
-docker run --init -p 8080:8080 -p 5000:5000 conductoross/conductor-standalone:3.15.0
-```
-After starting the server navigate to http://localhost:1234 to ensure the server has started successfully.
+In this section, we will create a simple "Hello World" application that executes a "greetings" workflow managed by Conductor.
 
-## Simple Hello World Application using Conductor
-In this section, we will create a simple "Hello World" application that uses Conductor. 
+### Step 1: Create Workflow
 
-### Step 1: Create a Workflow
+#### Creating Workflows by Code
 
-**Use Code to create workflows**
+Create [greetings_workflow.py](examples/helloworld/greetings_workflow.py) with the following:
 
-Create [greetings_workflow.py](examples/greetings_workflow.py) with the following:
 ```python
 from conductor.client.workflow.conductor_workflow import ConductorWorkflow
 from conductor.client.workflow.executor.workflow_executor import WorkflowExecutor
-from greetings import greet
+from greetings_worker import greet
 
 def greetings_workflow(workflow_executor: WorkflowExecutor) -> ConductorWorkflow:
-    name = 'hello'
+    name = 'greetings'
     workflow = ConductorWorkflow(name=name, executor=workflow_executor)
     workflow.version = 1
     workflow >> greet(task_ref_name='greet_ref', name=workflow.input('name'))
     return workflow
 
 
 ```
 
-**(alternatively) Use JSON to create workflows**
+#### (Alternatively) Creating Workflows in JSON
+
+Create `greetings_workflow.json` with the following:
 
-Create workflow.json with the following:
 ```json
 {
-  "name": "hello",
-  "description": "hello workflow",
+  "name": "greetings",
+  "description": "Sample greetings workflow",
   "version": 1,
   "tasks": [
     {
       "name": "greet",
       "taskReferenceName": "greet_ref",
       "type": "SIMPLE",
       "inputParameters": {
@@ -108,40 +98,44 @@
       }
     }
   ],
   "timeoutPolicy": "TIME_OUT_WF",
   "timeoutSeconds": 60
 }
 ```
-Now, register this workflow with the server:
+
+Workflows must be registered to the Conductor server. Use the API to register the greetings workflow from the JSON file above:
 ```shell
 curl -X POST -H "Content-Type:application/json" \
-http://localhost:8080/api/metadata/workflow -d @workflow.json
+http://localhost:8080/api/metadata/workflow -d @greetings_workflow.json
 ```
+> [!note]
+> To use the Conductor API, the Conductor server must be up and running (see [Running over Conductor standalone (installed locally)](#running-over-conductor-standalone-installed-locally)).
 
-### Step 2: Write Worker
+### Step 2: Write Task Worker
 
-Create [greetings.py](examples/greetings.py) with a simple worker and a workflow function.
+Using Python, a worker represents a function with the worker_task decorator. Create [greetings_worker.py](examples/helloworld/greetings_worker.py) file as illustrated below:
 
 > [!note]
-> A single workflow application can have workers written in different languages.
+> A single workflow can have task workers written in different languages and deployed anywhere, making your workflow polyglot and distributed!
 
 ```python
 from conductor.client.worker.worker_task import worker_task
 
 
 @worker_task(task_definition_name='greet')
 def greet(name: str) -> str:
-    return f'Hello my friend {name}'
+    return f'Hello {name}'
 
 ```
+Now, we are ready to write our main application, which will execute our workflow.
 
-### Step 3: Write _your_ application
+### Step 3: Write _Hello World_ Application
 
-Let's add [greetings_main.py](examples/greetings_main.py) with the `main` method:
+Let's add [helloworld.py](examples/helloworld/helloworld.py) with a `main` method:
 
 ```python
 from conductor.client.automator.task_handler import TaskHandler
 from conductor.client.configuration.configuration import Configuration
 from conductor.client.workflow.conductor_workflow import ConductorWorkflow
 from conductor.client.workflow.executor.workflow_executor import WorkflowExecutor
 from greetings_workflow import greetings_workflow
@@ -150,50 +144,101 @@
 def register_workflow(workflow_executor: WorkflowExecutor) -> ConductorWorkflow:
     workflow = greetings_workflow(workflow_executor=workflow_executor)
     workflow.register(True)
     return workflow
 
 
 def main():
-    # points to http://localhost:8080/api by default
+    # The app is connected to http://localhost:8080/api by default
     api_config = Configuration()
 
     workflow_executor = WorkflowExecutor(configuration=api_config)
 
-    # Needs to be done only when registering a workflow one-time
+    # Registering the workflow (Required only when the app is executed the first time)
     workflow = register_workflow(workflow_executor)
 
+    # Starting the worker polling mechanism
     task_handler = TaskHandler(configuration=api_config)
     task_handler.start_processes()
 
     workflow_run = workflow_executor.execute(name=workflow.name, version=workflow.version,
                                              workflow_input={'name': 'Orkes'})
 
     print(f'\nworkflow result: {workflow_run.output["result"]}\n')
     print(f'see the workflow execution here: {api_config.ui_host}/execution/{workflow_run.workflow_id}\n')
     task_handler.stop_processes()
 
 
 if __name__ == '__main__':
     main()
 ```
+## Running Workflows on Conductor Standalone (Installed Locally)
 
-> [!NOTE]
-> That's it - you just created your first distributed python app!
-> 
+### Setup Environment Variable
 
-## Using Conductor in your application
-There are three main ways you will use Conductor when building durable, resilient, distributed applications.
-1. Write service workers that implements business logic to accomplish a specific goal - such as initiate payment transfer, get user information from database etc. 
-2. Create Conductor workflows that implements application state - A typical workflow implements SAGA pattern
-3. Use Conductor SDK and APIs to manage workflows from your application.
+Set the following environment variable to point the SDK to the Conductor Server API endpoint:
 
-In this guide, we will dive deeper into each of these topic.
+```shell
+export CONDUCTOR_SERVER_URL=http://localhost:8080/api
+```
+### Start Conductor Server
 
-### [Create and Run Conductor Workers](workers.md)
-### [Create Conductor Workflows](workflows.md)
-### [Using Conductor in your Application](conductor_apps.md)
+To start the Conductor server in a standalone mode from a Docker image, type the command below:
 
+```shell
+docker run --init -p 8080:8080 -p 5000:5000 conductoross/conductor-standalone:3.15.0
+```
+To ensure the server has started successfully, open Conductor UI on http://localhost:5000.
 
+### Execute Hello World Application
 
+To run the application, type the following command:
 
+```
+python helloworld.py
+```
+
+Now, the workflow is executed, and its execution status can be viewed from Conductor UI (http://localhost:5000).
+
+Navigate to the **Executions** tab to view the workflow execution.
+
+<img width="1434" alt="Screenshot 2024-03-18 at 12 30 07" src="https://github.com/Srividhya-S-Subramanian/conductor-python-v1/assets/163816773/11e829b6-d46a-4b47-b2cf-0bf524a6ebdc">
+
+## Running Workflows on Orkes Conductor
+
+For running the workflow in Orkes Conductor,
+
+- Update the Conductor server URL to your cluster name.
+
+```shell
+export CONDUCTOR_SERVER_URL=https://[cluster-name].orkesconductor.io/api
+```
+
+- If you want to run the workflow on the Orkes Conductor Playground, set the Conductor Server variable as follows:
+
+```shell
+export CONDUCTOR_SERVER_URL=https://play.orkes.io/api
+```
+
+- Orkes Conductor requires authentication. [Obtain the key and secret from the Conductor server](https://orkes.io/content/how-to-videos/access-key-and-secret) and set the following environment variables.
 
+```shell
+export CONDUCTOR_AUTH_KEY=your_key
+export CONDUCTOR_AUTH_SECRET=your_key_secret
+```
+
+Run the application and view the execution status from Conductor's UI Console.
+
+> [!NOTE]
+> That's it - you just created and executed your first distributed Python app!
+
+## Learn More about Conductor Python SDK
+
+There are three main ways you can use Conductor when building durable, resilient, distributed applications.
+
+1. Write service workers that implement business logic to accomplish a specific goal - such as initiating payment transfer, getting user information from the database, etc.
+2. Create Conductor workflows that implement application state - A typical workflow implements the saga pattern.
+3. Use Conductor SDK and APIs to manage workflows from your application.
+
+### [Create and Run Conductor Workers](workers.md)
+### [Create Conductor Workflows](workflows.md)
+### [Using Conductor in your Application](conductor_apps.md)
```

### Comparing `conductor-python-1.1.4/setup.cfg` & `conductor_python-1.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/ai/integrations.py` & `conductor_python-1.1.5/src/conductor/client/ai/integrations.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/ai/orchestrator.py` & `conductor_python-1.1.5/src/conductor/client/ai/orchestrator.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/authorization_client.py` & `conductor_python-1.1.5/src/conductor/client/authorization_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/automator/task_handler.py` & `conductor_python-1.1.5/src/conductor/client/automator/task_handler.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/automator/task_runner.py` & `conductor_python-1.1.5/src/conductor/client/automator/task_runner.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/automator/utils.py` & `conductor_python-1.1.5/src/conductor/client/automator/utils.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/configuration/configuration.py` & `conductor_python-1.1.5/src/conductor/client/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/configuration/settings/metrics_settings.py` & `conductor_python-1.1.5/src/conductor/client/configuration/settings/metrics_settings.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/event/event_client.py` & `conductor_python-1.1.5/src/conductor/client/event/event_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/event/queue/kafka_queue_configuration.py` & `conductor_python-1.1.5/src/conductor/client/event/queue/kafka_queue_configuration.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/event/queue/queue_configuration.py` & `conductor_python-1.1.5/src/conductor/client/event/queue/queue_configuration.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/exceptions/api_exception_handler.py` & `conductor_python-1.1.5/src/conductor/client/exceptions/api_exception_handler.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/helpers/helper.py` & `conductor_python-1.1.5/src/conductor/client/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/application_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/application_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/authorization_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/authorization_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/event_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/event_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/group_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/group_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/integration_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/integration_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/metadata_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/metadata_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/prompt_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/prompt_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/scheduler_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/scheduler_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/secret_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/secret_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/task_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/task_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/token_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/token_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/user_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/user_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/workflow_bulk_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/workflow_bulk_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api/workflow_resource_api.py` & `conductor_python-1.1.5/src/conductor/client/http/api/workflow_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/api_client.py` & `conductor_python-1.1.5/src/conductor/client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/__init__.py` & `conductor_python-1.1.5/src/conductor/client/http/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,7 +48,8 @@
 from conductor.client.http.models.workflow_schedule_execution_model import WorkflowScheduleExecutionModel
 from conductor.client.http.models.workflow_status import WorkflowStatus
 from conductor.client.http.models.workflow_summary import WorkflowSummary
 from conductor.client.http.models.workflow_tag import WorkflowTag
 from conductor.client.http.models.integration import Integration
 from conductor.client.http.models.integration_api import IntegrationApi
 from conductor.client.http.models.state_change_event import StateChangeEvent, StateChangeConfig, StateChangeEventType
+from conductor.client.http.models.workflow_task import CacheConfig
```

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/action.py` & `conductor_python-1.1.5/src/conductor/client/http/models/action.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/authorization_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/authorization_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/bulk_response.py` & `conductor_python-1.1.5/src/conductor/client/http/models/bulk_response.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/conductor_application.py` & `conductor_python-1.1.5/src/conductor/client/http/models/conductor_application.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/conductor_user.py` & `conductor_python-1.1.5/src/conductor/client/http/models/conductor_user.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/correlation_ids_search_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/correlation_ids_search_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/create_or_update_application_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/create_or_update_application_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/event_handler.py` & `conductor_python-1.1.5/src/conductor/client/http/models/event_handler.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/external_storage_location.py` & `conductor_python-1.1.5/src/conductor/client/http/models/external_storage_location.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/generate_token_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/generate_token_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/group.py` & `conductor_python-1.1.5/src/conductor/client/http/models/group.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/health.py` & `conductor_python-1.1.5/src/conductor/client/http/models/health.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/health_check_status.py` & `conductor_python-1.1.5/src/conductor/client/http/models/health_check_status.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/integration.py` & `conductor_python-1.1.5/src/conductor/client/http/models/integration.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/integration_api.py` & `conductor_python-1.1.5/src/conductor/client/http/models/integration_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/integration_api_update.py` & `conductor_python-1.1.5/src/conductor/client/http/models/integration_api_update.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/integration_def.py` & `conductor_python-1.1.5/src/conductor/client/http/models/integration_def.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/integration_update.py` & `conductor_python-1.1.5/src/conductor/client/http/models/integration_update.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/permission.py` & `conductor_python-1.1.5/src/conductor/client/http/models/permission.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/poll_data.py` & `conductor_python-1.1.5/src/conductor/client/http/models/poll_data.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/prompt_template.py` & `conductor_python-1.1.5/src/conductor/client/http/models/prompt_template.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/prompt_test_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/prompt_test_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/rate_limit.py` & `conductor_python-1.1.5/src/conductor/client/http/models/rate_limit.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/rerun_workflow_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/rerun_workflow_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/response.py` & `conductor_python-1.1.5/src/conductor/client/http/models/response.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/role.py` & `conductor_python-1.1.5/src/conductor/client/http/models/role.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/save_schedule_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/save_schedule_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/scrollable_search_result_workflow_summary.py` & `conductor_python-1.1.5/src/conductor/client/http/models/scrollable_search_result_workflow_summary.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/search_result_task.py` & `conductor_python-1.1.5/src/conductor/client/http/models/search_result_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/search_result_task_summary.py` & `conductor_python-1.1.5/src/conductor/client/http/models/search_result_task_summary.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/search_result_workflow.py` & `conductor_python-1.1.5/src/conductor/client/http/models/search_result_workflow.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/search_result_workflow_schedule_execution_model.py` & `conductor_python-1.1.5/src/conductor/client/http/models/search_result_workflow_schedule_execution_model.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/search_result_workflow_summary.py` & `conductor_python-1.1.5/src/conductor/client/http/models/search_result_workflow_summary.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/skip_task_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/skip_task_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/start_workflow.py` & `conductor_python-1.1.5/src/conductor/client/http/models/start_workflow.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/start_workflow_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/start_workflow_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/state_change_event.py` & `conductor_python-1.1.5/src/conductor/client/http/models/state_change_event.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/sub_workflow_params.py` & `conductor_python-1.1.5/src/conductor/client/http/models/sub_workflow_params.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/subject_ref.py` & `conductor_python-1.1.5/src/conductor/client/http/models/subject_ref.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/tag_object.py` & `conductor_python-1.1.5/src/conductor/client/http/models/tag_object.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/tag_string.py` & `conductor_python-1.1.5/src/conductor/client/http/models/tag_string.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/target_ref.py` & `conductor_python-1.1.5/src/conductor/client/http/models/target_ref.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/task.py` & `conductor_python-1.1.5/src/conductor/client/http/models/task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/task_def.py` & `conductor_python-1.1.5/src/conductor/client/http/models/task_def.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/task_details.py` & `conductor_python-1.1.5/src/conductor/client/http/models/task_details.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/task_exec_log.py` & `conductor_python-1.1.5/src/conductor/client/http/models/task_exec_log.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/task_result.py` & `conductor_python-1.1.5/src/conductor/client/http/models/task_result.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/task_summary.py` & `conductor_python-1.1.5/src/conductor/client/http/models/task_summary.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/upsert_group_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/upsert_group_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/upsert_user_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/upsert_user_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/workflow.py` & `conductor_python-1.1.5/src/conductor/client/http/models/workflow.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/workflow_def.py` & `conductor_python-1.1.5/src/conductor/client/http/models/workflow_def.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/workflow_run.py` & `conductor_python-1.1.5/src/conductor/client/http/models/workflow_run.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/workflow_schedule.py` & `conductor_python-1.1.5/src/conductor/client/http/models/workflow_schedule.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/workflow_schedule_execution_model.py` & `conductor_python-1.1.5/src/conductor/client/http/models/workflow_schedule_execution_model.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/workflow_state_update.py` & `conductor_python-1.1.5/src/conductor/client/http/models/workflow_state_update.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/workflow_status.py` & `conductor_python-1.1.5/src/conductor/client/http/models/workflow_status.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
+terminal_status = ('COMPLETED', 'FAILED', 'TIMED_OUT', 'TERMINATED')
+successful_status = ('PAUSED', 'COMPLETED')
+running_status = ('RUNNING', 'PAUSED')
 
 class WorkflowStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
@@ -185,14 +188,29 @@
                 result[attr] = value
         if issubclass(WorkflowStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
+    def is_completed(self) -> bool:
+        """Checks if the workflow has completed
+        :return: True if the workflow status is COMPLETED, FAILED or TERMINATED
+        """
+        return self._status in terminal_status
+
+    def is_successful(self) -> bool:
+        """Checks if the workflow has completed in successful state (ie COMPLETED)
+        :return: True if the workflow status is COMPLETED
+        """
+        return self._status in successful_status
+
+    def is_running(self) -> bool:
+        return self.status in running_status
+
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
```

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/workflow_summary.py` & `conductor_python-1.1.5/src/conductor/client/http/models/workflow_summary.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/workflow_tag.py` & `conductor_python-1.1.5/src/conductor/client/http/models/workflow_tag.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/workflow_task.py` & `conductor_python-1.1.5/src/conductor/client/http/models/workflow_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,47 @@
 from typing import List
 
 import six
 
 from conductor.client.http.models.state_change_event import StateChangeConfig, StateChangeEventType, StateChangeEvent
 
 
-class WorkflowTask(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+class CacheConfig(object):
+    swagger_types = {
+        'key': 'str',
+        'ttl_in_second': 'int'
+    }
 
-    Do not edit the class manually.
-    """
+    attribute_map = {
+        'key': 'key',
+        'ttl_in_second': 'ttlInSecond'
+    }
+
+    def __init__(self, key: str, ttl_in_second: int):
+        self._key = key
+        self._ttl_in_second = ttl_in_second
+
+    @property
+    def key(self):
+        return self._key
+
+    @key.setter
+    def key(self, key):
+        self._key = key
+
+    @property
+    def ttl_in_second(self):
+        return self._ttl_in_second
+
+    @ttl_in_second.setter
+    def ttl_in_second(self, ttl_in_second):
+        self._ttl_in_second = ttl_in_second
+
+
+class WorkflowTask(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
@@ -46,15 +74,16 @@
         'async_complete': 'bool',
         'loop_condition': 'str',
         'loop_over': 'list[WorkflowTask]',
         'retry_count': 'int',
         'evaluator_type': 'str',
         'expression': 'str',
         'workflow_task_type': 'str',
-        'on_state_change': 'dict(str, StateChangeConfig)'
+        'on_state_change': 'dict(str, StateChangeConfig)',
+        'cache_config': 'CacheConfig'
     }
 
     attribute_map = {
         'name': 'name',
         'task_reference_name': 'taskReferenceName',
         'description': 'description',
         'input_parameters': 'inputParameters',
@@ -80,25 +109,27 @@
         'async_complete': 'asyncComplete',
         'loop_condition': 'loopCondition',
         'loop_over': 'loopOver',
         'retry_count': 'retryCount',
         'evaluator_type': 'evaluatorType',
         'expression': 'expression',
         'workflow_task_type': 'workflowTaskType',
-        'on_state_change': 'onStateChange'
+        'on_state_change': 'onStateChange',
+        'cache_config': 'cacheConfig'
     }
 
     def __init__(self, name=None, task_reference_name=None, description=None, input_parameters=None, type=None,
                  dynamic_task_name_param=None, case_value_param=None, case_expression=None, script_expression=None,
                  decision_cases=None, dynamic_fork_join_tasks_param=None, dynamic_fork_tasks_param=None,
                  dynamic_fork_tasks_input_param_name=None, default_case=None, fork_tasks=None, start_delay=None,
                  sub_workflow_param=None, join_on=None, sink=None, optional=None, task_definition=None,
                  rate_limited=None, default_exclusive_join_task=None, async_complete=None, loop_condition=None,
                  loop_over=None, retry_count=None, evaluator_type=None, expression=None,
-                 workflow_task_type=None, on_state_change: dict[str, StateChangeConfig] = None):  # noqa: E501
+                 workflow_task_type=None, on_state_change: dict[str, StateChangeConfig] = None,
+                 cache_config: CacheConfig = None):  # noqa: E501
         """WorkflowTask - a model defined in Swagger"""  # noqa: E501
         self._name = None
         self._task_reference_name = None
         self._description = None
         self._input_parameters = None
         self._type = None
         self._dynamic_task_name_param = None
@@ -124,14 +155,15 @@
         self._loop_over = None
         self._retry_count = None
         self._evaluator_type = None
         self._expression = None
         self._workflow_task_type = None
         self.discriminator = None
         self._on_state_change = None
+        self._cache_config = None
         self.name = name
         self.task_reference_name = task_reference_name
         if description is not None:
             self.description = description
         if input_parameters is not None:
             self.input_parameters = input_parameters
         if type is not None:
@@ -184,14 +216,15 @@
             self.evaluator_type = evaluator_type
         if expression is not None:
             self.expression = expression
         if workflow_task_type is not None:
             self.workflow_task_type = workflow_task_type
         if on_state_change is not None:
             self._on_state_change = on_state_change
+        self._cache_config = cache_config
 
     @property
     def name(self):
         """Gets the name of this WorkflowTask.  # noqa: E501
 
 
         :return: The name of this WorkflowTask.  # noqa: E501
@@ -819,17 +852,25 @@
     @property
     def on_state_change(self) -> dict[str, List[StateChangeEvent]]:
         return self._on_state_change
 
     @on_state_change.setter
     def on_state_change(self, state_change: StateChangeConfig):
         self._on_state_change = {
-            state_change.type : state_change.events
+            state_change.type: state_change.events
         }
 
+    @property
+    def cache_config(self) -> CacheConfig:
+        return self._cache_config
+
+    @cache_config.setter
+    def cache_config(self, cache_config: CacheConfig):
+        self._cache_config = cache_config
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `conductor-python-1.1.4/src/conductor/client/http/models/workflow_test_request.py` & `conductor_python-1.1.5/src/conductor/client/http/models/workflow_test_request.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/http/rest.py` & `conductor_python-1.1.5/src/conductor/client/http/rest.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/integration_client.py` & `conductor_python-1.1.5/src/conductor/client/integration_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/metadata_client.py` & `conductor_python-1.1.5/src/conductor/client/metadata_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/api/tags_api.py` & `conductor_python-1.1.5/src/conductor/client/orkes/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/models/access_key.py` & `conductor_python-1.1.5/src/conductor/client/orkes/models/access_key.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/models/created_access_key.py` & `conductor_python-1.1.5/src/conductor/client/orkes/models/created_access_key.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/models/granted_permission.py` & `conductor_python-1.1.5/src/conductor/client/orkes/models/granted_permission.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/orkes_authorization_client.py` & `conductor_python-1.1.5/src/conductor/client/orkes/orkes_authorization_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/orkes_base_client.py` & `conductor_python-1.1.5/src/conductor/client/orkes/orkes_base_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/orkes_integration_client.py` & `conductor_python-1.1.5/src/conductor/client/orkes/orkes_integration_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/orkes_metadata_client.py` & `conductor_python-1.1.5/src/conductor/client/orkes/orkes_metadata_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/orkes_prompt_client.py` & `conductor_python-1.1.5/src/conductor/client/orkes/orkes_prompt_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/orkes_scheduler_client.py` & `conductor_python-1.1.5/src/conductor/client/orkes/orkes_scheduler_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/orkes_secret_client.py` & `conductor_python-1.1.5/src/conductor/client/orkes/orkes_secret_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/orkes_task_client.py` & `conductor_python-1.1.5/src/conductor/client/orkes/orkes_task_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes/orkes_workflow_client.py` & `conductor_python-1.1.5/src/conductor/client/orkes/orkes_workflow_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/orkes_clients.py` & `conductor_python-1.1.5/src/conductor/client/orkes_clients.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/prompt_client.py` & `conductor_python-1.1.5/src/conductor/client/prompt_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/scheduler_client.py` & `conductor_python-1.1.5/src/conductor/client/scheduler_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/secret_client.py` & `conductor_python-1.1.5/src/conductor/client/secret_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/task_client.py` & `conductor_python-1.1.5/src/conductor/client/task_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/telemetry/metrics_collector.py` & `conductor_python-1.1.5/src/conductor/client/telemetry/metrics_collector.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/telemetry/model/metric_documentation.py` & `conductor_python-1.1.5/src/conductor/client/telemetry/model/metric_documentation.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/telemetry/model/metric_name.py` & `conductor_python-1.1.5/src/conductor/client/telemetry/model/metric_name.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/worker/worker.py` & `conductor_python-1.1.5/src/conductor/client/worker/worker.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/worker/worker_interface.py` & `conductor_python-1.1.5/src/conductor/client/worker/worker_interface.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/worker/worker_task.py` & `conductor_python-1.1.5/src/conductor/client/worker/worker_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/conductor_workflow.py` & `conductor_python-1.1.5/src/conductor/client/workflow/conductor_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         start_workflow_request.workflow_def = self.to_workflow_def()
         start_workflow_request.name = self.name
         start_workflow_request.version = self.version
         return self._executor.start_workflow(start_workflow_request)
 
     def execute(self, workflow_input: Any = {}, wait_until_task_ref: str = '', wait_for_seconds: int = 10,
                 request_id: str = None,
-                idempotency_key: str = None, idempotency_strategy : IdempotencyStrategy = IdempotencyStrategy.FAIL) -> WorkflowRun:
+                idempotency_key: str = None, idempotency_strategy : IdempotencyStrategy = IdempotencyStrategy.FAIL, task_to_domain: dict[str, str] = None) -> WorkflowRun:
         """
         Executes a workflow synchronously.  Useful for short duration workflow (e.g. < 20 seconds)
         Parameters
         ----------
         workflow_input Input to the workflow
         wait_until_task_ref wait reference name of the task to wait until before returning the workflow results
         wait_for_seconds amount of time to wait in seconds before returning.
@@ -212,14 +212,16 @@
         request.workflow_def = self.to_workflow_def()
         request.input = workflow_input
         request.name = request.workflow_def.name
         request.version = 1
         if idempotency_key is not None:
             request.idempotency_key = idempotency_key
             request.idempotency_strategy = idempotency_strategy
+        if task_to_domain is not None:
+            request.task_to_domain = task_to_domain
         run = self._executor.execute_workflow(request, wait_until_task_ref=wait_until_task_ref,
                                               wait_for_seconds=wait_for_seconds, request_id=request_id)
 
         return run
 
     def to_workflow_def(self) -> WorkflowDef:
         return WorkflowDef(
```

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/executor/workflow_executor.py` & `conductor_python-1.1.5/src/conductor/client/workflow/executor/workflow_executor.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/do_while_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/do_while_task.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from copy import deepcopy
-from typing import List
+from typing import List, Dict, Any
 
 from typing_extensions import Self
 
 from conductor.client.http.models.workflow_task import WorkflowTask
 from conductor.client.workflow.task.task import TaskInterface, get_task_interface_list_as_workflow_task_list
 from conductor.client.workflow.task.task_type import TaskType
 
@@ -39,7 +39,19 @@
         super().__init__(
             task_ref_name=task_ref_name,
             termination_condition=get_for_loop_condition(
                 task_ref_name, iterations,
             ),
             tasks=tasks,
         )
+
+
+class ForEachTask(DoWhileTask):
+    def __init__(self, task_ref_name: str, tasks: List[TaskInterface], iterate_over:str, variables: List[str] = None) -> Self:
+        super().__init__(
+            task_ref_name=task_ref_name,
+            termination_condition=get_for_loop_condition(
+                task_ref_name, 0,
+            ),
+            tasks=tasks,
+        )
+        super().input_parameter("items", iterate_over)
```

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/dynamic_fork_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/dynamic_fork_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/dynamic_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/dynamic_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/event_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/event_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/fork_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/fork_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/get_document.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/get_document.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/http_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/http_task.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,27 +19,25 @@
 
 class HttpInput:
     swagger_types = {
         '_uri': 'str',
         '_method': 'str',
         '_accept': 'list[str]',
         '_headers': 'dict[str, list[str]]',
-        '_accept': 'str',
         '_content_type': 'str',
         '_connection_time_out': 'int',
         '_read_timeout': 'int',
         '_body': 'str',
     }
 
     attribute_map = {
         '_uri': 'uri',
         '_method': 'method',
         '_accept': 'accept',
         '_headers': 'headers',
-        '_accept': 'accept',
         '_content_type': 'contentType',
         '_connection_time_out': 'connectionTimeOut',
         '_read_timeout': 'readTimeOut',
         '_body': 'body',
     }
 
     def __init__(self,
```

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/human_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/human_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/inline.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/inline.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/javascript_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/javascript_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/join_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/join_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/kafka_publish.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/kafka_publish.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/kafka_publish_input.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/kafka_publish_input.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_chat_complete.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_chat_complete.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_generate_embeddings.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_generate_embeddings.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_index_documents.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_index_documents.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_index_text.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_index_text.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_query_embeddings.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_query_embeddings.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_search_index.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_search_index.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/llm_text_complete.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/llm_text_complete.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/utils/embedding_model.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/utils/embedding_model.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/llm_tasks/utils/prompt.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/llm_tasks/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/simple_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/simple_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/start_workflow_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/start_workflow_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/sub_workflow_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/sub_workflow_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/switch_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/switch_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from typing import Any, Dict, List
 
 from typing_extensions import Self, Union
 
-from conductor.client.http.models.workflow_task import WorkflowTask
+from conductor.client.http.models.workflow_task import WorkflowTask, CacheConfig
 from conductor.client.workflow.task.task_type import TaskType
 
 
 def get_task_interface_list_as_workflow_task_list(*tasks: Self) -> List[WorkflowTask]:
     converted_tasks = []
     for task in tasks:
         converted_tasks.append(task.to_workflow_task())
@@ -19,21 +19,25 @@
     @abstractmethod
     def __init__(self,
                  task_reference_name: str,
                  task_type: TaskType,
                  task_name: str = None,
                  description: str = None,
                  optional: bool = None,
-                 input_parameters: Dict[str, Any] = None) -> Self:
+                 input_parameters: Dict[str, Any] = None,
+                 cache_key : str = None,
+                 cache_ttl_second : int = 0) -> Self:
         self.task_reference_name = task_reference_name
         self.task_type = task_type
         self.name = task_name or task_reference_name
         self.description = description
         self.optional = optional
         self.input_parameters = input_parameters
+        self._cache_key = cache_key
+        self._cache_ttl_second = cache_ttl_second
 
     @property
     def task_reference_name(self) -> str:
         return self._task_reference_name
 
     @task_reference_name.setter
     def task_reference_name(self, task_reference_name: str) -> None:
@@ -57,14 +61,18 @@
 
     @name.setter
     def name(self, name: str) -> None:
         if not isinstance(name, str):
             raise Exception('invalid type')
         self._name = name
 
+    def cache(self, cache_key: str, cache_ttl_second: int):
+        self._cache_key = cache_key
+        self._cache_ttl_second = cache_ttl_second
+
     @property
     def description(self) -> str:
         return self._description
 
     @description.setter
     def description(self, description: str) -> None:
         if description != None and not isinstance(description, str):
@@ -100,28 +108,35 @@
     def input_parameter(self, key: str, value: Any) -> Self:
         if not isinstance(key, str):
             raise Exception('invalid type')
         self._input_parameters[key] = deepcopy(value)
         return self
 
     def to_workflow_task(self) -> WorkflowTask:
+        cache_config = None
+        if self._cache_ttl_second > 0 and self._cache_key is not None:
+            cache_config = CacheConfig(key=self._cache_key, ttl_in_second=self._cache_ttl_second)
         return WorkflowTask(
             name=self._name,
             task_reference_name=self._task_reference_name,
             type=self._task_type.value,
             description=self._description,
             input_parameters=self._input_parameters,
             optional=self._optional,
+            cache_config=cache_config
         )
 
     def output(self, json_path: str = None) -> str:
         if json_path is None:
             return '${' + f'{self.task_reference_name}.output' + '}'
         else:
-            return '${' + f'{self.task_reference_name}.output.{json_path}' + '}'
+            if json_path.startswith('.'):
+                return '${' + f'{self.task_reference_name}.output{json_path}' + '}'
+            else:
+                return '${' + f'{self.task_reference_name}.output.{json_path}' + '}'
 
     def input(self, json_path: str = None, key : str = None, value : Any = None) -> Union[str, Self]:
         if key is not None and value is not None:
             """
             For the backwards compatibility
             """
             return self.input_parameter(key, value)
```

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/task_type.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/task_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     START_WORKFLOW = 'START_WORKFLOW'
     EVENT = 'EVENT'
     WAIT = 'WAIT'
     WAIT_FOR_WEBHOOK = 'WAIT_FOR_WEBHOOK'
     HUMAN = 'HUMAN'
     USER_DEFINED = 'USER_DEFINED'
     HTTP = 'HTTP'
+    HTTP_POLL = 'HTTP_POLL'
     LAMBDA = 'LAMBDA'
     INLINE = 'INLINE'
     EXCLUSIVE_JOIN = 'EXCLUSIVE_JOIN'
     TERMINATE = 'TERMINATE'
     KAFKA_PUBLISH = 'KAFKA_PUBLISH'
     JSON_JQ_TRANSFORM = 'JSON_JQ_TRANSFORM'
     SET_VARIABLE = 'SET_VARIABLE'
```

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/terminate_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/terminate_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/wait_for_webhook_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/wait_for_webhook_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow/task/wait_task.py` & `conductor_python-1.1.5/src/conductor/client/workflow/task/wait_task.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor/client/workflow_client.py` & `conductor_python-1.1.5/src/conductor/client/workflow_client.py`

 * *Files identical despite different names*

### Comparing `conductor-python-1.1.4/src/conductor_python.egg-info/PKG-INFO` & `conductor_python-1.1.5/src/conductor_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conductor-python
-Version: 1.1.4
+Version: 1.1.5
 Summary: Netflix Conductor Python SDK
 Home-page: https://github.com/conductor-sdk/conductor-python
 Author: Orkes
 Author-email: developers@orkes.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -22,112 +22,102 @@
 Requires-Dist: requests>=2.31.0
 Requires-Dist: typing-extensions>=4.2.0
 Requires-Dist: astor>=0.8.1
 Requires-Dist: shortuuid>=1.0.11
 Requires-Dist: dacite>=1.8.1
 
 # Conductor OSS Python SDK
-Python SDK for working with https://github.com/conductor-oss/conductor
 
-[Conductor](https://www.conductor-oss.org/) is an open source distributed, scalable and highly available 
-orchestration platform that allows developers to build powerful distributed applications.
-You can find the documentation for Conductor here: [Conductor Docs](https://orkes.io/content)
+Python SDK for working with https://github.com/conductor-oss/conductor.
+
+[Conductor](https://www.conductor-oss.org/) is the leading open-source orchestration platform allowing developers to build highly scalable distributed applications.
+
+Check out the [official documentation for Conductor](https://orkes.io/content).
 
 ## ⭐ Conductor OSS
+
 Show support for the Conductor OSS.  Please help spread the awareness by starring Conductor repo.
 
 [![GitHub stars](https://img.shields.io/github/stars/conductor-oss/conductor.svg?style=social&label=Star&maxAge=)](https://GitHub.com/conductor-oss/conductor/)
 
 ## Content
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
-- [Install SDK](#install-sdk)
+- [Install Conductor Python SDK](#install-conductor-python-sdk)
   - [Get Conductor Python SDK](#get-conductor-python-sdk)
-  - [Setup SDK](#setup-sdk)
-- [Start Conductor Server](#start-conductor-server)
-- [Simple Hello World Application using Conductor](#simple-hello-world-application-using-conductor)
-  - [Step 1: Create a Workflow](#step-1-create-a-workflow)
-  - [Step 2: Write Worker](#step-2-write-worker)
-  - [Step 3: Write _your_ application](#step-3-write-_your_-application)
-- [Using Conductor in your application](#using-conductor-in-your-application)
+- [Hello World Application Using Conductor](#hello-world-application-using-conductor)
+  - [Step 1: Create Workflow](#step-1-create-workflow)
+    - [Creating Workflows by Code](#creating-workflows-by-code)
+    - [(Alternatively) Creating Workflows in JSON](#alternatively-creating-workflows-in-json)
+  - [Step 2: Write Task Worker](#step-2-write-task-worker)
+  - [Step 3: Write _Hello World_ Application](#step-3-write-_hello-world_-application)
+- [Running Workflows on Conductor Standalone (Installed Locally)](#running-workflows-on-conductor-standalone-installed-locally)
+  - [Setup Environment Variable](#setup-environment-variable)
+  - [Start Conductor Server](#start-conductor-server)
+  - [Execute Hello World Application](#execute-hello-world-application)
+- [Running Workflows on Orkes Conductor](#running-workflows-on-orkes-conductor)
+- [Learn More about Conductor Python SDK](#learn-more-about-conductor-python-sdk)
   - [Create and Run Conductor Workers](#create-and-run-conductor-workers)
   - [Create Conductor Workflows](#create-conductor-workflows)
   - [Using Conductor in your Application](#using-conductor-in-your-application)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
-## Install SDK
-Create a virtual environment to build your package
+## Install Conductor Python SDK
+
+Before installing Conductor Python SDK, it is a good practice to set up a dedicated virtual environment as follows:
+
 ```shell
 virtualenv conductor
 source conductor/bin/activate
 ```
 
 ### Get Conductor Python SDK
 
-SDK needs Python 3.9+.
+The SDK requires Python 3.9+. To install the SDK, use the following command:
 
 ```shell
 python3 -m pip install conductor-python
 ```
-### Setup SDK
-
-Point the SDK to the Conductor Server API endpoint
-```shell
-export CONDUCTOR_SERVER_URL=http://localhost:8080/api
-```
-(Optionally) If you are using a Conductor server that requires authentication
-
-[How to obtain the key and secret from the conductor server
-](https://orkes.io/content/docs/getting-started/concepts/access-control)
 
+## Hello World Application Using Conductor
 
-```shell
-export CONDUCTOR_AUTH_KEY=your_key
-export CONDUCTOR_AUTH_SECRET=your_key_secret
-```
-
-## Start Conductor Server
-```shell
-docker run --init -p 8080:8080 -p 5000:5000 conductoross/conductor-standalone:3.15.0
-```
-After starting the server navigate to http://localhost:1234 to ensure the server has started successfully.
+In this section, we will create a simple "Hello World" application that executes a "greetings" workflow managed by Conductor.
 
-## Simple Hello World Application using Conductor
-In this section, we will create a simple "Hello World" application that uses Conductor. 
+### Step 1: Create Workflow
 
-### Step 1: Create a Workflow
+#### Creating Workflows by Code
 
-**Use Code to create workflows**
+Create [greetings_workflow.py](examples/helloworld/greetings_workflow.py) with the following:
 
-Create [greetings_workflow.py](examples/greetings_workflow.py) with the following:
 ```python
 from conductor.client.workflow.conductor_workflow import ConductorWorkflow
 from conductor.client.workflow.executor.workflow_executor import WorkflowExecutor
-from greetings import greet
+from greetings_worker import greet
 
 def greetings_workflow(workflow_executor: WorkflowExecutor) -> ConductorWorkflow:
-    name = 'hello'
+    name = 'greetings'
     workflow = ConductorWorkflow(name=name, executor=workflow_executor)
     workflow.version = 1
     workflow >> greet(task_ref_name='greet_ref', name=workflow.input('name'))
     return workflow
 
 
 ```
 
-**(alternatively) Use JSON to create workflows**
+#### (Alternatively) Creating Workflows in JSON
+
+Create `greetings_workflow.json` with the following:
 
-Create workflow.json with the following:
 ```json
 {
-  "name": "hello",
-  "description": "hello workflow",
+  "name": "greetings",
+  "description": "Sample greetings workflow",
   "version": 1,
   "tasks": [
     {
       "name": "greet",
       "taskReferenceName": "greet_ref",
       "type": "SIMPLE",
       "inputParameters": {
@@ -135,40 +125,44 @@
       }
     }
   ],
   "timeoutPolicy": "TIME_OUT_WF",
   "timeoutSeconds": 60
 }
 ```
-Now, register this workflow with the server:
+
+Workflows must be registered to the Conductor server. Use the API to register the greetings workflow from the JSON file above:
 ```shell
 curl -X POST -H "Content-Type:application/json" \
-http://localhost:8080/api/metadata/workflow -d @workflow.json
+http://localhost:8080/api/metadata/workflow -d @greetings_workflow.json
 ```
+> [!note]
+> To use the Conductor API, the Conductor server must be up and running (see [Running over Conductor standalone (installed locally)](#running-over-conductor-standalone-installed-locally)).
 
-### Step 2: Write Worker
+### Step 2: Write Task Worker
 
-Create [greetings.py](examples/greetings.py) with a simple worker and a workflow function.
+Using Python, a worker represents a function with the worker_task decorator. Create [greetings_worker.py](examples/helloworld/greetings_worker.py) file as illustrated below:
 
 > [!note]
-> A single workflow application can have workers written in different languages.
+> A single workflow can have task workers written in different languages and deployed anywhere, making your workflow polyglot and distributed!
 
 ```python
 from conductor.client.worker.worker_task import worker_task
 
 
 @worker_task(task_definition_name='greet')
 def greet(name: str) -> str:
-    return f'Hello my friend {name}'
+    return f'Hello {name}'
 
 ```
+Now, we are ready to write our main application, which will execute our workflow.
 
-### Step 3: Write _your_ application
+### Step 3: Write _Hello World_ Application
 
-Let's add [greetings_main.py](examples/greetings_main.py) with the `main` method:
+Let's add [helloworld.py](examples/helloworld/helloworld.py) with a `main` method:
 
 ```python
 from conductor.client.automator.task_handler import TaskHandler
 from conductor.client.configuration.configuration import Configuration
 from conductor.client.workflow.conductor_workflow import ConductorWorkflow
 from conductor.client.workflow.executor.workflow_executor import WorkflowExecutor
 from greetings_workflow import greetings_workflow
@@ -177,50 +171,101 @@
 def register_workflow(workflow_executor: WorkflowExecutor) -> ConductorWorkflow:
     workflow = greetings_workflow(workflow_executor=workflow_executor)
     workflow.register(True)
     return workflow
 
 
 def main():
-    # points to http://localhost:8080/api by default
+    # The app is connected to http://localhost:8080/api by default
     api_config = Configuration()
 
     workflow_executor = WorkflowExecutor(configuration=api_config)
 
-    # Needs to be done only when registering a workflow one-time
+    # Registering the workflow (Required only when the app is executed the first time)
     workflow = register_workflow(workflow_executor)
 
+    # Starting the worker polling mechanism
     task_handler = TaskHandler(configuration=api_config)
     task_handler.start_processes()
 
     workflow_run = workflow_executor.execute(name=workflow.name, version=workflow.version,
                                              workflow_input={'name': 'Orkes'})
 
     print(f'\nworkflow result: {workflow_run.output["result"]}\n')
     print(f'see the workflow execution here: {api_config.ui_host}/execution/{workflow_run.workflow_id}\n')
     task_handler.stop_processes()
 
 
 if __name__ == '__main__':
     main()
 ```
+## Running Workflows on Conductor Standalone (Installed Locally)
 
-> [!NOTE]
-> That's it - you just created your first distributed python app!
-> 
+### Setup Environment Variable
 
-## Using Conductor in your application
-There are three main ways you will use Conductor when building durable, resilient, distributed applications.
-1. Write service workers that implements business logic to accomplish a specific goal - such as initiate payment transfer, get user information from database etc. 
-2. Create Conductor workflows that implements application state - A typical workflow implements SAGA pattern
-3. Use Conductor SDK and APIs to manage workflows from your application.
+Set the following environment variable to point the SDK to the Conductor Server API endpoint:
 
-In this guide, we will dive deeper into each of these topic.
+```shell
+export CONDUCTOR_SERVER_URL=http://localhost:8080/api
+```
+### Start Conductor Server
 
-### [Create and Run Conductor Workers](workers.md)
-### [Create Conductor Workflows](workflows.md)
-### [Using Conductor in your Application](conductor_apps.md)
+To start the Conductor server in a standalone mode from a Docker image, type the command below:
 
+```shell
+docker run --init -p 8080:8080 -p 5000:5000 conductoross/conductor-standalone:3.15.0
+```
+To ensure the server has started successfully, open Conductor UI on http://localhost:5000.
 
+### Execute Hello World Application
 
+To run the application, type the following command:
 
+```
+python helloworld.py
+```
+
+Now, the workflow is executed, and its execution status can be viewed from Conductor UI (http://localhost:5000).
+
+Navigate to the **Executions** tab to view the workflow execution.
+
+<img width="1434" alt="Screenshot 2024-03-18 at 12 30 07" src="https://github.com/Srividhya-S-Subramanian/conductor-python-v1/assets/163816773/11e829b6-d46a-4b47-b2cf-0bf524a6ebdc">
+
+## Running Workflows on Orkes Conductor
+
+For running the workflow in Orkes Conductor,
+
+- Update the Conductor server URL to your cluster name.
+
+```shell
+export CONDUCTOR_SERVER_URL=https://[cluster-name].orkesconductor.io/api
+```
+
+- If you want to run the workflow on the Orkes Conductor Playground, set the Conductor Server variable as follows:
+
+```shell
+export CONDUCTOR_SERVER_URL=https://play.orkes.io/api
+```
+
+- Orkes Conductor requires authentication. [Obtain the key and secret from the Conductor server](https://orkes.io/content/how-to-videos/access-key-and-secret) and set the following environment variables.
 
+```shell
+export CONDUCTOR_AUTH_KEY=your_key
+export CONDUCTOR_AUTH_SECRET=your_key_secret
+```
+
+Run the application and view the execution status from Conductor's UI Console.
+
+> [!NOTE]
+> That's it - you just created and executed your first distributed Python app!
+
+## Learn More about Conductor Python SDK
+
+There are three main ways you can use Conductor when building durable, resilient, distributed applications.
+
+1. Write service workers that implement business logic to accomplish a specific goal - such as initiating payment transfer, getting user information from the database, etc.
+2. Create Conductor workflows that implement application state - A typical workflow implements the saga pattern.
+3. Use Conductor SDK and APIs to manage workflows from your application.
+
+### [Create and Run Conductor Workers](workers.md)
+### [Create Conductor Workflows](workflows.md)
+### [Using Conductor in your Application](conductor_apps.md)
```

### Comparing `conductor-python-1.1.4/src/conductor_python.egg-info/SOURCES.txt` & `conductor_python-1.1.5/src/conductor_python.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -158,14 +158,15 @@
 src/conductor/client/workflow/task/__init__.py
 src/conductor/client/workflow/task/do_while_task.py
 src/conductor/client/workflow/task/dynamic_fork_task.py
 src/conductor/client/workflow/task/dynamic_task.py
 src/conductor/client/workflow/task/event_task.py
 src/conductor/client/workflow/task/fork_task.py
 src/conductor/client/workflow/task/get_document.py
+src/conductor/client/workflow/task/http_poll_task.py
 src/conductor/client/workflow/task/http_task.py
 src/conductor/client/workflow/task/human_task.py
 src/conductor/client/workflow/task/inline.py
 src/conductor/client/workflow/task/javascript_task.py
 src/conductor/client/workflow/task/join_task.py
 src/conductor/client/workflow/task/json_jq_task.py
 src/conductor/client/workflow/task/kafka_publish.py
```

