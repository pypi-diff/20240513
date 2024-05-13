# Comparing `tmp/ob-metaflow-stubs-3.2.tar.gz` & `tmp/ob-metaflow-stubs-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-stubs-3.2.tar", last modified: Tue May  7 00:05:42 2024, max compression
+gzip compressed data, was "ob-metaflow-stubs-3.3.tar", last modified: Mon May 13 17:42:15 2024, max compression
```

## Comparing `ob-metaflow-stubs-3.2.tar` & `ob-metaflow-stubs-3.3.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.550550 ob-metaflow-stubs-3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 00:05:18.000000 ob-metaflow-stubs-3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 00:05:42.546550 ob-metaflow-stubs-3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-07 00:05:18.000000 ob-metaflow-stubs-3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.530550 ob-metaflow-stubs-3.2/metaflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.530550 ob-metaflow-stubs-3.2/metaflow-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/client/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/client/filecache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/clone_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/flowspec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/generated_for.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/includefile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.530550 ob-metaflow-stubs-3.2/metaflow-stubs/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/metadata/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/metadata/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/metaflow_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/metaflow_current.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.530550 ob-metaflow-stubs-3.2/metaflow-stubs/mflog/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/mflog/mflog.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/multicore_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/parameters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.534550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.534550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/airflow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/airflow_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/airflow_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.534550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.534550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/argo_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/argo_events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/argo_workflows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.538550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/aws_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.538550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/batch/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/batch/batch_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.538550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.538550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.538550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/azure_credential.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/azure_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/azure_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.542550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_creator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_datastore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.542550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/basic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/card.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.542550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/components.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/component_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/catch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.542550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/local.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.542550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/s3/s3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/s3/s3util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/debug_logger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/debug_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/environment_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/events_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.542550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/frameworks/pytorch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.546550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/gs_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.546550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/kubernetes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/package_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/parallel_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/perimeters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/project_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.546550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/conda_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/conda_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/pypi_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/resources_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/retry_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.546550 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/secrets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/storage_executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/tag_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/plugins/timeout_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/procpoll.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.546550 ob-metaflow-stubs-3.2/metaflow-stubs/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/profilers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/pylint_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-07 00:05:40.000000 ob-metaflow-stubs-3.2/metaflow-stubs/tagging_util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:05:42.546550 ob-metaflow-stubs-3.2/ob_metaflow_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 00:05:42.000000 ob-metaflow-stubs-3.2/ob_metaflow_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-07 00:05:42.000000 ob-metaflow-stubs-3.2/ob_metaflow_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:05:42.000000 ob-metaflow-stubs-3.2/ob_metaflow_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 00:05:42.000000 ob-metaflow-stubs-3.2/ob_metaflow_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 00:05:42.550550 ob-metaflow-stubs-3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-07 00:05:18.000000 ob-metaflow-stubs-3.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 00:05:18.000000 ob-metaflow-stubs-3.2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 17:41:58.000000 ob-metaflow-stubs-3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-13 17:41:58.000000 ob-metaflow-stubs-3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.055098 ob-metaflow-stubs-3.3/metaflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.059098 ob-metaflow-stubs-3.3/metaflow-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/client/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/client/filecache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/clone_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/flowspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/generated_for.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/includefile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.059098 ob-metaflow-stubs-3.3/metaflow-stubs/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/metadata/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/metadata/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/metaflow_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/metaflow_current.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.059098 ob-metaflow-stubs-3.3/metaflow-stubs/mflog/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/mflog/mflog.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/multicore_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/parameters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.059098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/aws_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.067098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.067098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_credential.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.067098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_creator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_datastore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.067098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/basic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/card.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/components.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/component_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/catch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/local.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/debug_logger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/debug_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/environment_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/events_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/frameworks/pytorch.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/package_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/parallel_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/perimeters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/project_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/conda_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/conda_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/pypi_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/resources_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/retry_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/storage_executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/tag_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/timeout_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/procpoll.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/metaflow-stubs/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/profilers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/pylint_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/tagging_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-13 17:42:15.000000 ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-13 17:41:58.000000 ob-metaflow-stubs-3.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 17:41:58.000000 ob-metaflow-stubs-3.3/version.py
```

### Comparing `ob-metaflow-stubs-3.2/PKG-INFO` & `ob-metaflow-stubs-3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.2
+Version: 3.3
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/__init__.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.513974                                        #
+# Generated on 2024-05-13T17:42:14.215304                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import io
-    import metaflow.parameters
-    import datetime
     import typing
-    import metaflow.events
+    import datetime
+    import metaflow._vendor.click.types
+    import metaflow.parameters
+    import metaflow.client.core
     import metaflow.plugins.datatools.s3.s3
-    import metaflow.datastore.inputs
     import metaflow.metaflow_current
-    import metaflow.client.core
-    import metaflow._vendor.click.types
+    import metaflow.events
+    import metaflow.datastore.inputs
+    import io
 FlowSpecDerived = typing.TypeVar("FlowSpecDerived", bound="FlowSpec", contravariant=False, covariant=False)
 StepFlag = typing.NewType("StepFlag", bool)
 
 CURRENT_DIRECTORY: str
 
 INFO_FILE: str
 
@@ -722,144 +722,110 @@
     -------
     Union[Callable[[FlowSpecDerived, StepFlag], None], Callable[[FlowSpecDerived, Any, StepFlag], None]]
         Function that is a Metaflow Step
     """
     ...
 
 @typing.overload
-def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
-    
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    Specifies that the step will success under all circumstances.
     
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
     """
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
+def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
     """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
-    
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    Specifies that the step will success under all circumstances.
     
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
     """
     ...
 
 @typing.overload
-def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the resources needed when executing this step.
-    
-    Use `@resources` to specify the resource requirements
-    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    Creates a human-readable report, a Metaflow Card, after this step completes.
     
-    You can choose the compute layer on the command line by executing e.g.
-    ```
-    python myflow.py run --with batch
-    ```
-    or
-    ```
-    python myflow.py run --with kubernetes
-    ```
-    which executes the flow on the desired system using the
-    requirements specified in `@resources`.
+    Note that you may add multiple `@card` decorators in a step with different parameters.
     
     Parameters
     ----------
-    cpu : int, default 1
-        Number of CPUs required for this step.
-    gpu : int, default 0
-        Number of GPUs required for this step.
-    disk : int, optional, default None
-        Disk size (in MB) required for this step. Only applies on Kubernetes.
-    memory : int, default 4096
-        Memory size (in MB) required for this step.
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
     """
     ...
 
 @typing.overload
-def resources(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def resources(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def resources(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None):
+def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
     """
-    Specifies the resources needed when executing this step.
-    
-    Use `@resources` to specify the resource requirements
-    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    Creates a human-readable report, a Metaflow Card, after this step completes.
     
-    You can choose the compute layer on the command line by executing e.g.
-    ```
-    python myflow.py run --with batch
-    ```
-    or
-    ```
-    python myflow.py run --with kubernetes
-    ```
-    which executes the flow on the desired system using the
-    requirements specified in `@resources`.
+    Note that you may add multiple `@card` decorators in a step with different parameters.
     
     Parameters
     ----------
-    cpu : int, default 1
-        Number of CPUs required for this step.
-    gpu : int, default 0
-        Number of GPUs required for this step.
-    disk : int, optional, default None
-        Disk size (in MB) required for this step. Only applies on Kubernetes.
-    memory : int, default 4096
-        Memory size (in MB) required for this step.
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
     """
     ...
 
 @typing.overload
 def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the number of times the task corresponding
@@ -909,90 +875,136 @@
         Number of times to retry this task.
     minutes_between_retries : int, default 2
         Number of minutes between retries.
     """
     ...
 
 @typing.overload
-def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies environment variables to be set prior to the execution of a step.
+    Specifies the resources needed when executing this step.
+    
+    Use `@resources` to specify the resource requirements
+    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    
+    You can choose the compute layer on the command line by executing e.g.
+    ```
+    python myflow.py run --with batch
+    ```
+    or
+    ```
+    python myflow.py run --with kubernetes
+    ```
+    which executes the flow on the desired system using the
+    requirements specified in `@resources`.
     
     Parameters
     ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
+    cpu : int, default 1
+        Number of CPUs required for this step.
+    gpu : int, default 0
+        Number of GPUs required for this step.
+    disk : int, optional, default None
+        Disk size (in MB) required for this step. Only applies on Kubernetes.
+    memory : int, default 4096
+        Memory size (in MB) required for this step.
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
 @typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def resources(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def resources(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
+def resources(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None):
     """
-    Specifies environment variables to be set prior to the execution of a step.
+    Specifies the resources needed when executing this step.
+    
+    Use `@resources` to specify the resource requirements
+    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    
+    You can choose the compute layer on the command line by executing e.g.
+    ```
+    python myflow.py run --with batch
+    ```
+    or
+    ```
+    python myflow.py run --with kubernetes
+    ```
+    which executes the flow on the desired system using the
+    requirements specified in `@resources`.
     
     Parameters
     ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
+    cpu : int, default 1
+        Number of CPUs required for this step.
+    gpu : int, default 0
+        Number of GPUs required for this step.
+    disk : int, optional, default None
+        Disk size (in MB) required for this step. Only applies on Kubernetes.
+    memory : int, default 4096
+        Memory size (in MB) required for this step.
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
 @typing.overload
-def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies that the step will success under all circumstances.
+    Specifies the PyPI packages for the step.
     
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
+    Information in this decorator will augment any
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
+    packages : Dict[str, str], default: {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
+def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
     """
-    Specifies that the step will success under all circumstances.
+    Specifies the PyPI packages for the step.
     
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
+    Information in this decorator will augment any
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
+    packages : Dict[str, str], default: {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, shared_memory: typing.Optional[int] = None, port: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that this step should execute on Kubernetes.
     
@@ -1048,59 +1060,74 @@
         Shared memory size (in MiB) required for this step
     port: int, optional
         Port number to specify in the Kubernetes job object
     """
     ...
 
 @typing.overload
-def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the PyPI packages for the step.
-    
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
+    Specifies environment variables to be set prior to the execution of a step.
     
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
     """
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
+def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
     """
-    Specifies the PyPI packages for the step.
+    Specifies environment variables to be set prior to the execution of a step.
     
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
+    Parameters
+    ----------
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
+    """
+    ...
+
+@typing.overload
+def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
     
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
+    """
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
+    """
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
+    
+    Parameters
+    ----------
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
     """
     ...
 
 @typing.overload
 def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the Conda environment for the step.
@@ -1154,94 +1181,67 @@
         that the version used will correspond to the version of the Python interpreter used to start the run.
     disabled : bool, default False
         If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
+    Specifies a timeout for your step.
     
-    Note that you may add multiple `@card` decorators in a step with different parameters.
+    This decorator is useful if this step may hang indefinitely.
     
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
     
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
+    Parameters
+    ----------
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
+def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
     """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
-    
-    Note that you may add multiple `@card` decorators in a step with different parameters.
-    
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
+    Specifies a timeout for your step.
     
+    This decorator is useful if this step may hang indefinitely.
     
-    """
-    ...
-
-@typing.overload
-def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
     
-    Parameters
-    ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
-    """
-    ...
-
-@typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
-    """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
     Parameters
     ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
 def batch(*, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
@@ -1385,14 +1385,63 @@
         List of strings containing options for the chosen log driver. The configurable values
         depend on the `log driver` chosen. Validation of these options is not supported yet.
         Example usage: ["awslogs-group:aws/batch/job"]
     """
     ...
 
 @typing.overload
+def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the Conda environment for all steps of the flow.
+    
+    Use `@conda_base` to set common libraries required by all
+    steps and use `@conda` to specify step-specific additions.
+    
+    Parameters
+    ----------
+    packages : Dict[str, str], default {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables Conda.
+    """
+    ...
+
+@typing.overload
+def conda_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def conda_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
+    """
+    Specifies the Conda environment for all steps of the flow.
+    
+    Use `@conda_base` to set common libraries required by all
+    steps and use `@conda` to specify step-specific additions.
+    
+    Parameters
+    ----------
+    packages : Dict[str, str], default {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables Conda.
+    """
+    ...
+
+@typing.overload
 def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the flow(s) that this flow depends on.
     
     ```
     @trigger_on_finish(flow='FooFlow')
     ```
@@ -1487,14 +1536,32 @@
     options : Dict[str, Any], default {}
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
+def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies what flows belong to the same project.
+    
+    A project-specific namespace is created for all flows that
+    use the same `@project(name)`.
+    
+    Parameters
+    ----------
+    name : str
+        Project name. Make sure that the name is unique amongst all
+        projects that use the same production scheduler. The name may
+        contain only lowercase alphanumeric characters and underscores.
+    
+    
+    """
+    ...
+
 @typing.overload
 def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the times when the flow should be run when running on a
     production scheduler.
     
     Parameters
@@ -1536,14 +1603,98 @@
         specified by this expression.
     timezone : str, optional, default None
         Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
         which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
     """
     ...
 
+def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
+    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
+    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
+    added as a flow decorators. Adding more than one decorator will ensure that `start` step
+    starts only after all sensors finish.
+    
+    Parameters
+    ----------
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    bucket_key : Union[str, List[str]]
+        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
+        When it's specified as a full s3:// url, please leave `bucket_name` as None
+    bucket_name : str
+        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
+        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
+    wildcard_match : bool
+        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
+    aws_conn_id : str
+        a reference to the s3 connection on Airflow. (Default: None)
+    verify : bool
+        Whether or not to verify SSL certificates for S3 connection. (Default: None)
+    """
+    ...
+
+def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
+    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
+    
+    Parameters
+    ----------
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    external_dag_id : str
+        The dag_id that contains the task you want to wait for.
+    external_task_ids : List[str]
+        The list of task_ids that you want to wait for.
+        If None (default value) the sensor waits for the DAG. (Default: None)
+    allowed_states : List[str]
+        Iterable of allowed states, (Default: ['success'])
+    failed_states : List[str]
+        Iterable of failed or dis-allowed states. (Default: None)
+    execution_delta : datetime.timedelta
+        time difference with the previous execution to look at,
+        the default is the same logical date as the current task or DAG. (Default: None)
+    check_existence: bool
+        Set to True to check if the external task exists or check if
+        the DAG to wait for exists. (Default: True)
+    """
+    ...
+
 @typing.overload
 def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the PyPI packages for all steps of the flow.
     
     Use `@pypi_base` to set common packages required by all
     steps and use `@pypi` to specify step-specific overrides.
@@ -1670,165 +1821,14 @@
     options : Dict[str, Any], default {}
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
-def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
-    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
-    
-    Parameters
-    ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    external_dag_id : str
-        The dag_id that contains the task you want to wait for.
-    external_task_ids : List[str]
-        The list of task_ids that you want to wait for.
-        If None (default value) the sensor waits for the DAG. (Default: None)
-    allowed_states : List[str]
-        Iterable of allowed states, (Default: ['success'])
-    failed_states : List[str]
-        Iterable of failed or dis-allowed states. (Default: None)
-    execution_delta : datetime.timedelta
-        time difference with the previous execution to look at,
-        the default is the same logical date as the current task or DAG. (Default: None)
-    check_existence: bool
-        Set to True to check if the external task exists or check if
-        the DAG to wait for exists. (Default: True)
-    """
-    ...
-
-def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies what flows belong to the same project.
-    
-    A project-specific namespace is created for all flows that
-    use the same `@project(name)`.
-    
-    Parameters
-    ----------
-    name : str
-        Project name. Make sure that the name is unique amongst all
-        projects that use the same production scheduler. The name may
-        contain only lowercase alphanumeric characters and underscores.
-    
-    
-    """
-    ...
-
-def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
-    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
-    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
-    added as a flow decorators. Adding more than one decorator will ensure that `start` step
-    starts only after all sensors finish.
-    
-    Parameters
-    ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    bucket_key : Union[str, List[str]]
-        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
-        When it's specified as a full s3:// url, please leave `bucket_name` as None
-    bucket_name : str
-        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
-        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
-    wildcard_match : bool
-        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
-    aws_conn_id : str
-        a reference to the s3 connection on Airflow. (Default: None)
-    verify : bool
-        Whether or not to verify SSL certificates for S3 connection. (Default: None)
-    """
-    ...
-
-@typing.overload
-def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the Conda environment for all steps of the flow.
-    
-    Use `@conda_base` to set common libraries required by all
-    steps and use `@conda` to specify step-specific additions.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables Conda.
-    """
-    ...
-
-@typing.overload
-def conda_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def conda_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
-    """
-    Specifies the Conda environment for all steps of the flow.
-    
-    Use `@conda_base` to set common libraries required by all
-    steps and use `@conda` to specify step-specific additions.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables Conda.
-    """
-    ...
-
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
     pass None to this call.
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/cards.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/cards.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.534816                                        #
+# Generated on 2024-05-13T17:42:14.238947                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
+    import typing
     import metaflow.plugins.cards.card_client
     import metaflow.plugins.cards.card_modules.components
     import metaflow.plugins.cards.card_modules.basic
-    import typing
+    import metaflow.plugins.cards.card_modules.card
     import metaflow
 
 def get_cards(task: typing.Union[str, "metaflow.Task"], id: typing.Optional[str] = None, type: typing.Optional[str] = None, follow_resumed: bool = True) -> metaflow.plugins.cards.card_client.CardContainer:
     """
     Get cards related to a `Task`.
     
     Note that `get_cards` resolves the cards contained by the task, but it doesn't actually
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/cli.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/cli.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.539827                                        #
+# Generated on 2024-05-13T17:42:14.244457                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/client/__init__.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/client/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.537353                                        #
+# Generated on 2024-05-13T17:42:14.242055                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
+    import datetime
     import metaflow.events
+    import typing
     import metaflow.client.core
-    import datetime
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/client/core.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/client/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.523510                                        #
+# Generated on 2024-05-13T17:42:14.224613                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import tarfile
-    import metaflow.events
     import typing
     import datetime
-    import metaflow.metaflow_current
     import metaflow.client.core
-    import metaflow
     import metaflow.exception
+    import metaflow.metaflow_current
+    import tarfile
+    import metaflow.events
+    import metaflow
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/client/filecache.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/client/filecache.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.541225                                        #
+# Generated on 2024-05-13T17:42:14.245301                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.datastore.content_addressed_store
     import metaflow.exception
+    import metaflow.datastore.content_addressed_store
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/clone_util.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/clone_util.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.537913                                        #
+# Generated on 2024-05-13T17:42:14.242614                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaDatum(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/events.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/events.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.525430                                        #
+# Generated on 2024-05-13T17:42:14.226538                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.events
     import metaflow
+    import metaflow.events
 
 TYPE_CHECKING: bool
 
 class MetaflowEvent(tuple, metaclass=type):
     @staticmethod
     def __new__(_cls, name, id, timestamp, type):
         """
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/exception.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/exception.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.515944                                        #
+# Generated on 2024-05-13T17:42:14.217208                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/flowspec.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/flowspec.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.524840                                        #
+# Generated on 2024-05-13T17:42:14.225957                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import typing
     import metaflow.parameters
+    import metaflow.exception
     import metaflow.unbounded_foreach
-    import typing
     import metaflow.datastore.inputs
-    import metaflow.exception
 
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/includefile.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/includefile.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.533005                                        #
+# Generated on 2024-05-13T17:42:14.235704                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import io
-    import metaflow.parameters
     import typing
-    import metaflow.plugins.datatools.s3.s3
     import metaflow._vendor.click.types
+    import metaflow.parameters
+    import metaflow.plugins.datatools.s3.s3
+    import io
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/metadata/metadata.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/metadata/metadata.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.560835                                        #
+# Generated on 2024-05-13T17:42:14.269008                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metadata.metadata
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/metadata/util.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/metadata/util.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.591964                                        #
+# Generated on 2024-05-13T17:42:14.302766                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def copy_tree(src, dst, update = False):
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/metaflow_config.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/metaflow_config.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.516926                                        #
+# Generated on 2024-05-13T17:42:14.218222                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/metaflow_current.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/metaflow_current.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.604865                                        #
+# Generated on 2024-05-13T17:42:14.313497                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.events
     import typing
     import metaflow.metaflow_current
+    import metaflow.events
     import metaflow
     import metaflow.plugins.cards.component_serializer
 
 TYPE_CHECKING: bool
 
 TEMPDIR: str
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/mflog/mflog.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/mflog/mflog.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.561153                                        #
+# Generated on 2024-05-13T17:42:14.269524                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import datetime
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/multicore_utils.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/multicore_utils.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.517352                                        #
+# Generated on 2024-05-13T17:42:14.218650                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/parameters.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/parameters.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.518499                                        #
+# Generated on 2024-05-13T17:42:14.219723                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow._vendor.click.types
     import typing
-    import metaflow.parameters
+    import metaflow._vendor.click.types
     import metaflow.exception
+    import metaflow.parameters
 
 class ParameterFieldFailed(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, name, field):
         ...
     ...
 
 class ParameterFieldTypeMismatch(metaflow.exception.MetaflowException, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/__init__.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.526990                                        #
+# Generated on 2024-05-13T17:42:14.227985                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.unbounded_foreach
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.unbounded_foreach
 
 CLIS_DESC: list
 
 class InternalTestUnboundedForeachInput(metaflow.unbounded_foreach.UnboundedForeachInput, metaclass=type):
     def __init__(self, iterable):
         ...
     def __iter__(self):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/airflow.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.567714                                        #
+# Generated on 2024-05-13T17:42:14.274027                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow._vendor.click.types
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/airflow_cli.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_cli.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.568741                                        #
+# Generated on 2024-05-13T17:42:14.274985                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/airflow_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_decorator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.565833                                        #
+# Generated on 2024-05-13T17:42:14.271784                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/airflow_utils.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_utils.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.565463                                        #
+# Generated on 2024-05-13T17:42:14.271185                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 TASK_ID_XCOM_KEY: str
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/exception.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.566054                                        #
+# Generated on 2024-05-13T17:42:14.215904                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -13,15 +13,23 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
-    def __init__(self, msg):
-        ...
+CLIENT_REFRESH_INTERVAL_SECONDS: int
+
+class KubernetesClientException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class NotSupportedException(metaflow.exception.MetaflowException, metaclass=type):
+class KubernetesClient(object, metaclass=type):
+    def __init__(self):
+        ...
+    def get(self):
+        ...
+    def job(self, **kwargs):
+        ...
+    def jobset(self, **kwargs):
+        ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/sensors/__init__.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/__init__.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.566328                                        #
+# Generated on 2024-05-13T17:42:14.272470                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.airflow.sensors.base_sensor
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.601152                                        #
+# Generated on 2024-05-13T17:42:14.301186                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.601529                                        #
+# Generated on 2024-05-13T17:42:14.301928                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.decorators
     import metaflow.exception
+    import metaflow.plugins.airflow.sensors.base_sensor
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
@@ -39,16 +39,12 @@
     ...
 
 class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, msg):
         ...
     ...
 
-AIRFLOW_STATES: dict
-
-class ExternalTaskSensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
-    def serialize_operator_args(self):
-        ...
+class S3KeySensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
     def validate(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.601868                                        #
+# Generated on 2024-05-13T17:42:14.301561                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.decorators
     import metaflow.exception
+    import metaflow.plugins.airflow.sensors.base_sensor
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
@@ -39,12 +39,16 @@
     ...
 
 class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, msg):
         ...
     ...
 
-class S3KeySensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
+AIRFLOW_STATES: dict
+
+class ExternalTaskSensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
+    def serialize_operator_args(self):
+        ...
     def validate(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/argo_client.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.580874                                        #
+# Generated on 2024-05-13T17:42:14.290237                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/argo_events.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_events.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.579550                                        #
+# Generated on 2024-05-13T17:42:14.288894                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/argo_workflows.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.584923                                        #
+# Generated on 2024-05-13T17:42:14.294233                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.parameters
-    import metaflow.metaflow_current
     import metaflow._vendor.click.types
     import metaflow.exception
+    import metaflow.parameters
+    import metaflow.metaflow_current
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.586501                                        #
+# Generated on 2024-05-13T17:42:14.295734                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.parameters
     import metaflow.decorators
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.parameters
+    import metaflow.metaflow_current
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.580318                                        #
+# Generated on 2024-05-13T17:42:14.289672                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
+    import metaflow
     import metaflow.events
     import metaflow.metaflow_current
-    import metaflow
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/aws_client.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/aws_client.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.537654                                        #
+# Generated on 2024-05-13T17:42:14.242361                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 cached_aws_sandbox_creds: None
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/aws_utils.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/aws_utils.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.564155                                        #
+# Generated on 2024-05-13T17:42:14.287372                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/batch/batch.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.599024                                        #
+# Generated on 2024-05-13T17:42:14.309380                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/batch/batch_cli.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_cli.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.600292                                        #
+# Generated on 2024-05-13T17:42:14.310651                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/batch/batch_client.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.597996                                        #
+# Generated on 2024-05-13T17:42:14.308424                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.599730                                        #
+# Generated on 2024-05-13T17:42:14.310095                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
 def get_run_time_limit_for_task(step_decos):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.600683                                        #
+# Generated on 2024-05-13T17:42:14.311041                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.exception
     import abc
     import metaflow.plugins.secrets
-    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.592180                                        #
+# Generated on 2024-05-13T17:42:14.302975                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 SFN_DYNAMO_DB_TABLE: None
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.593226                                        #
+# Generated on 2024-05-13T17:42:14.303777                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class EventBridgeClient(object, metaclass=type):
     def __init__(self, name):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/production_token.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/resources_decorator.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.592956                                        #
+# Generated on 2024-05-13T17:42:14.247343                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow.decorators
 
-def new_token(token_prefix, prev_token = None):
-    ...
-
-def load_token(token_prefix):
-    ...
-
-def store_token(token_prefix, token):
+class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/retry_decorator.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.592723                                        #
+# Generated on 2024-05-13T17:42:14.247224                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class ScheduleDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
+
+MAX_ATTEMPTS: int
+
+class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+        ...
+    def step_task_retry_count(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.595412                                        #
+# Generated on 2024-05-13T17:42:14.305943                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.596842                                        #
+# Generated on 2024-05-13T17:42:14.307221                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.parameters
     import metaflow.decorators
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.parameters
+    import metaflow.metaflow_current
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.593530                                        #
+# Generated on 2024-05-13T17:42:14.304082                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 AWS_SANDBOX_ENABLED: bool
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.592558                                        #
+# Generated on 2024-05-13T17:42:14.303350                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/azure_credential.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_credential.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.589009                                        #
+# Generated on 2024-05-13T17:42:14.298031                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class AzureDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/azure_exceptions.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_exceptions.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.589233                                        #
+# Generated on 2024-05-13T17:42:14.298249                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/azure_utils.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.589637                                        #
+# Generated on 2024-05-13T17:42:14.298715                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.589961                                        #
+# Generated on 2024-05-13T17:42:14.299033                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/azure/includefile_support.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/includefile_support.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.555764                                        #
+# Generated on 2024-05-13T17:42:14.260437                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -16,39 +16,39 @@
     def __str__(self):
         ...
     ...
 
 class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class Azure(object, metaclass=type):
+class GS(object, metaclass=type):
     @classmethod
     def get_root_from_config(cls, echo, create_on_absent = True):
         ...
     def __init__(self):
         ...
     def __enter__(self):
         ...
     def __exit__(self, *args):
         ...
     def get(self, key = None, return_missing = False):
         """
-        Key MUST be a fully qualified path with uri scheme.  azure://<container_name>/b/l/o/b/n/a/m/e
+        Key MUST be a fully qualified path.  gs://<bucket_name>/b/l/o/b/n/a/m/e
         """
         ...
     def put(self, key, obj, overwrite = True):
         """
-        Key MUST be a fully qualified path.  <container_name>/b/l/o/b/n/a/m/e
+        Key MUST be a fully qualified path.  gs://<bucket_name>/b/l/o/b/n/a/m/e
         """
         ...
     def info(self, key = None, return_missing = False):
         ...
     ...
 
-class AzureObject(object, metaclass=type):
+class GSObject(object, metaclass=type):
     def __init__(self, url, path, exists, size):
         ...
     @property
     def path(self):
         ...
     @property
     def url(self):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_cli.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.577890                                        #
+# Generated on 2024-05-13T17:42:14.282141                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.parameters
-    import datetime
     import typing
+    import datetime
+    import metaflow.parameters
     import metaflow.client.core
     import metaflow.exception
 
 class Task(metaflow.client.core.MetaflowObject, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     @property
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_client.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.557296                                        #
+# Generated on 2024-05-13T17:42:14.262380                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_client
-    import metaflow.exception
     import metaflow
+    import metaflow.exception
 
 TYPE_CHECKING: bool
 
 CARD_SUFFIX: str
 
 def resolve_paths_from_task(flow_datastore, pathspec = None, type = None, hash = None, card_id = None):
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_creator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_creator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.573630                                        #
+# Generated on 2024-05-13T17:42:14.278031                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_datastore.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_datastore.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.575198                                        #
+# Generated on 2024-05-13T17:42:14.279448                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.574382                                        #
+# Generated on 2024-05-13T17:42:14.278729                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/__init__.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.571475                                        #
+# Generated on 2024-05-13T17:42:14.275827                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/basic.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/basic.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.551850                                        #
+# Generated on 2024-05-13T17:42:14.253401                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.card
-    import metaflow.plugins.cards.card_modules.basic
     import metaflow
+    import metaflow.plugins.cards.card_modules.basic
 
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/card.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/card.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.557698                                        #
+# Generated on 2024-05-13T17:42:14.263118                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.602242                                        #
+# Generated on 2024-05-13T17:42:14.302265                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def main(template, data = None, **kwargs):
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.603759                                        #
+# Generated on 2024-05-13T17:42:14.312477                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def render(template = "", data = {}, partials_path = ".", partials_ext = "mustache", partials_dict = {}, padding = "", def_ldel = "{{", def_rdel = "}}", scopes = None, warn = False, keep = False):
     """
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.603379                                        #
+# Generated on 2024-05-13T17:42:14.312084                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 linesep: str
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.603003                                        #
+# Generated on 2024-05-13T17:42:14.311721                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class ChevronError(SyntaxError, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/components.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/components.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.559651                                        #
+# Generated on 2024-05-13T17:42:14.266901                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
-    import metaflow.plugins.cards.card_modules.components
-    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.components
 
 class LogComponent(metaflow.plugins.cards.card_modules.basic.DefaultComponent, metaclass=type):
     def __init__(self, data = None):
         ...
     def render(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.591489                                        #
+# Generated on 2024-05-13T17:42:14.300481                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class TypeResolvedObject(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.591679                                        #
+# Generated on 2024-05-13T17:42:14.300668                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.basic
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.552999                                        #
+# Generated on 2024-05-13T17:42:14.255078                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.card
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/card_resolver.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_resolver.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.575788                                        #
+# Generated on 2024-05-13T17:42:14.279935                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class CardDatastore(object, metaclass=type):
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/component_serializer.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/component_serializer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.573373                                        #
+# Generated on 2024-05-13T17:42:14.277778                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
-    import metaflow.plugins.cards.card_modules.components
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.exception
     import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.components
 
 class MetaflowCardComponent(object, metaclass=type):
     @property
     def component_id(self):
         ...
     @component_id.setter
     def component_id(self, value):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/cards/exception.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/exception.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.572037                                        #
+# Generated on 2024-05-13T17:42:14.276383                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/catch_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/catch_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.544428                                        #
+# Generated on 2024-05-13T17:42:14.246863                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/__init__.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.547411                                        #
+# Generated on 2024-05-13T17:42:14.249747                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.datatools.s3.s3
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/local.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/local.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.555292                                        #
+# Generated on 2024-05-13T17:42:14.258805                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/s3/__init__.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.588755                                        #
+# Generated on 2024-05-13T17:42:14.297784                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.datatools.s3.s3
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/s3/s3.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.530232                                        #
+# Generated on 2024-05-13T17:42:14.231039                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import io
     import typing
     import metaflow.plugins.datatools.s3.s3
+    import metaflow.exception
     import metaflow.metaflow_current
     import metaflow.datastore.inputs
-    import metaflow.exception
+    import io
 
 TYPE_CHECKING: bool
 
 class FlowSpec(object, metaclass=type):
     def __init__(self, use_cli = True):
         """
         Construct a FlowSpec
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/s3/s3tail.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3tail.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.602653                                        #
+# Generated on 2024-05-13T17:42:14.311397                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def aws_retry(f):
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/datatools/s3/s3util.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3util.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.554762                                        #
+# Generated on 2024-05-13T17:42:14.257860                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/debug_logger.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/debug_logger.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.548971                                        #
+# Generated on 2024-05-13T17:42:14.251264                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.event_logger
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/debug_monitor.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/debug_monitor.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.549199                                        #
+# Generated on 2024-05-13T17:42:14.251487                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.monitor
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/environment_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/environment_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.543506                                        #
+# Generated on 2024-05-13T17:42:14.248225                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/events_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/events_decorator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.547771                                        #
+# Generated on 2024-05-13T17:42:14.250113                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/frameworks/pytorch.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/frameworks/pytorch.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.578337                                        #
+# Generated on 2024-05-13T17:42:14.275367                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
-    import metaflow.metaflow_current
     import metaflow.plugins.parallel_decorator
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class ParallelDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
     def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.591132                                        #
+# Generated on 2024-05-13T17:42:14.300134                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.exception
     import abc
     import metaflow.plugins.secrets
-    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/gs_exceptions.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/utils.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.590419                                        #
+# Generated on 2024-05-13T17:42:14.283246                                        #
 ##################################################################################
 
 from __future__ import annotations
 
-import typing
-if typing.TYPE_CHECKING:
-    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
+def conda_platform():
+    ...
+
+def wheel_tags(wheel):
+    ...
+
+def pip_tags(python_version, mamba_platform):
+    ...
+
+def parse_filename_from_url(url):
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.590234                                        #
+# Generated on 2024-05-13T17:42:14.299264                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class GcpDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/gs_utils.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_utils.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.590711                                        #
+# Generated on 2024-05-13T17:42:14.299721                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/gcp/includefile_support.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/includefile_support.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.556222                                        #
+# Generated on 2024-05-13T17:42:14.259603                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -16,39 +16,39 @@
     def __str__(self):
         ...
     ...
 
 class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class GS(object, metaclass=type):
+class Azure(object, metaclass=type):
     @classmethod
     def get_root_from_config(cls, echo, create_on_absent = True):
         ...
     def __init__(self):
         ...
     def __enter__(self):
         ...
     def __exit__(self, *args):
         ...
     def get(self, key = None, return_missing = False):
         """
-        Key MUST be a fully qualified path.  gs://<bucket_name>/b/l/o/b/n/a/m/e
+        Key MUST be a fully qualified path with uri scheme.  azure://<container_name>/b/l/o/b/n/a/m/e
         """
         ...
     def put(self, key, obj, overwrite = True):
         """
-        Key MUST be a fully qualified path.  gs://<bucket_name>/b/l/o/b/n/a/m/e
+        Key MUST be a fully qualified path.  <container_name>/b/l/o/b/n/a/m/e
         """
         ...
     def info(self, key = None, return_missing = False):
         ...
     ...
 
-class GSObject(object, metaclass=type):
+class AzureObject(object, metaclass=type):
     def __init__(self, url, path, exists, size):
         ...
     @property
     def path(self):
         ...
     @property
     def url(self):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/kubernetes/kubernetes.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.562081                                        #
+# Generated on 2024-05-13T17:42:14.285266                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.563814                                        #
+# Generated on 2024-05-13T17:42:14.287040                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow._vendor.click.types
     import metaflow.decorators
+    import metaflow._vendor.click.types
     import metaflow.exception
 
 class JSONTypeClass(metaflow._vendor.click.types.ParamType, metaclass=type):
     def convert(self, value, param, ctx):
         ...
     def __str__(self):
         ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/project_decorator.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.514695                                        #
+# Generated on 2024-05-13T17:42:14.250433                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
+    import metaflow.decorators
+    import metaflow.metaflow_current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-CLIENT_REFRESH_INTERVAL_SECONDS: int
+current: metaflow.metaflow_current.Current
 
-class KubernetesClientException(metaflow.exception.MetaflowException, metaclass=type):
-    ...
+VALID_NAME_RE: str
 
-class KubernetesClient(object, metaclass=type):
-    def __init__(self):
-        ...
-    def get(self):
-        ...
-    def job(self, **kwargs):
+VALID_NAME_LEN: int
+
+class ProjectDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
-    def jobset(self, **kwargs):
+    def get_top_level_options(self):
         ...
     ...
 
+def format_name(flow_name, project_name, deploy_prod, given_branch, user_name):
+    ...
+
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.563036                                        #
+# Generated on 2024-05-13T17:42:14.286261                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/parallel_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/parallel_decorator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.545631                                        #
+# Generated on 2024-05-13T17:42:14.246383                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/perimeters.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/pylint_wrapper.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.515000                                        #
+# Generated on 2024-05-13T17:42:14.243384                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
+if typing.TYPE_CHECKING:
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-CURRENT_PERIMETER_KEY: str
-
-CURRENT_PERIMETER_URL: str
+class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
+    ...
 
-def get_perimeter_config_url_if_set_in_ob_config() -> typing.Optional[str]:
+class PyLint(object, metaclass=type):
+    def __init__(self, fname):
+        ...
+    def has_pylint(self):
+        ...
+    def run(self, logger = None, warnings = False, pylint_config = []):
+        ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/__init__.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/perimeters.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.545162                                        #
+# Generated on 2024-05-13T17:42:14.216208                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-MAGIC_FILE: str
+CURRENT_PERIMETER_KEY: str
+
+CURRENT_PERIMETER_URL: str
+
+def get_perimeter_config_url_if_set_in_ob_config() -> typing.Optional[str]:
+    ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/conda_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/conda_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.569511                                        #
+# Generated on 2024-05-13T17:42:14.282952                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/conda_environment.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/conda_environment.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.570602                                        #
+# Generated on 2024-05-13T17:42:14.284005                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_environment
-    import abc
     import io
     import metaflow.exception
+    import abc
+    import metaflow.metaflow_environment
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/pypi_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/pypi_decorator.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.568982                                        #
+# Generated on 2024-05-13T17:42:14.282426                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/pypi_environment.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/pypi_environment.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.571024                                        #
+# Generated on 2024-05-13T17:42:14.284388                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_environment
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/pypi/utils.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_exceptions.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.569805                                        #
+# Generated on 2024-05-13T17:42:14.299442                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-def conda_platform():
-    ...
-
-def wheel_tags(wheel):
-    ...
-
-def pip_tags(python_version, mamba_platform):
-    ...
-
-def parse_filename_from_url(url):
+class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/secrets/__init__.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/__init__.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.546087                                        #
+# Generated on 2024-05-13T17:42:14.248440                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.579174                                        #
+# Generated on 2024-05-13T17:42:14.288523                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/secrets/secrets_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/secrets_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.578932                                        #
+# Generated on 2024-05-13T17:42:14.288293                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/storage_executor.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/storage_executor.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.548573                                        #
+# Generated on 2024-05-13T17:42:14.250891                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/tag_cli.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/tag_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.554191                                        #
+# Generated on 2024-05-13T17:42:14.256916                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.events
     import datetime
-    import metaflow.metaflow_current
     import metaflow.client.core
     import metaflow.exception
+    import metaflow.metaflow_current
+    import metaflow.events
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.541963                                        #
+# Generated on 2024-05-13T17:42:14.245825                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/plugins/timeout_decorator.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/timeout_decorator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.542599                                        #
+# Generated on 2024-05-13T17:42:14.247986                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/procpoll.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/procpoll.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.538369                                        #
+# Generated on 2024-05-13T17:42:14.243019                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.procpoll
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/profilers/__init__.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/profilers/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.515240                                        #
+# Generated on 2024-05-13T17:42:14.216446                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class gpu_profile(object, metaclass=type):
     def __init__(self, include_artifacts = True, artifact_prefix = "gpu_profile_", interval = 1):
```

### Comparing `ob-metaflow-stubs-3.2/metaflow-stubs/tagging_util.pyi` & `ob-metaflow-stubs-3.3/metaflow-stubs/tagging_util.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
 # MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-07T00:05:40.518825                                        #
+# Generated on 2024-05-13T17:42:14.220030                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.2/ob_metaflow_stubs.egg-info/PKG-INFO` & `ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.2
+Version: 3.3
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.2/ob_metaflow_stubs.egg-info/SOURCES.txt` & `ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ob-metaflow-stubs-3.2/setup.py` & `ob-metaflow-stubs-3.3/setup.py`

 * *Files identical despite different names*

