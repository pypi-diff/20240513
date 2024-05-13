# Comparing `tmp/wds-client-0.2.99.tar.gz` & `tmp/wds_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wds-client-0.2.99.tar", last modified: Tue Sep 19 15:29:25 2023, max compression
+gzip compressed data, was "wds_client-0.3.0.tar", last modified: Mon May 13 14:06:37 2024, max compression
```

## Comparing `wds-client-0.2.99.tar` & `wds_client-0.3.0.tar`

### file list

```diff
@@ -1,108 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.746235 wds-client-0.2.99/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-09-19 15:29:25.746235 wds-client-0.2.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2023-09-19 15:27:23.000000 wds-client-0.2.99/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-09-19 15:29:25.750235 wds-client-0.2.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-09-19 15:27:23.000000 wds-client-0.2.99/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.738235 wds-client-0.2.99/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_backup_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_backup_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_backup_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_backup_restore_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_clone_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_clone_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_clone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_db_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_db_validationcomponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_db_validationcomponent_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_disk_space_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_disk_space_component_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_inline_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_instances_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_record_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_records_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_search_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_search_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_version_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.742235 wds-client-0.2.99/wds_client/
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.742235 wds-client-0.2.99/wds_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17088 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9761 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17329 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/instances_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    61562 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/records_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19354 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26210 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12787 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.746235 wds-client-0.2.99/wds_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/backup_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/backup_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/backup_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/backup_restore_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/clone_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/clone_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/clone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/db_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/db_validationcomponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/db_validationcomponent_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/disk_space_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/disk_space_component_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/record_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/search_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/search_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12309 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.742235 wds-client-0.2.99/wds_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-09-19 15:29:25.000000 wds-client-0.2.99/wds_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2023-09-19 15:29:25.000000 wds-client-0.2.99/wds_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 15:29:25.000000 wds-client-0.2.99/wds_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-19 15:29:25.000000 wds-client-0.2.99/wds_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-19 15:29:25.000000 wds-client-0.2.99/wds_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.030501 wds_client-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 14:06:37.030501 wds_client-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-13 14:04:40.000000 wds_client-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 14:06:37.030501 wds_client-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-13 14:04:40.000000 wds_client-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.018501 wds_client-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_attribute_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_attribute_schema_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_backup_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_backup_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_backup_restore_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-13 14:04:39.000000 wds_client-0.3.0/test/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_capabilities_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_clone_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_clone_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_clone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_db_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_db_validationcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_db_validationcomponent_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_disk_space_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_disk_space_component_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_generic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_generic_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_import_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_job_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_job_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_record_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-13 14:04:40.000000 wds_client-0.3.0/test/test_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.022501 wds_client-0.3.0/wds_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.022501 wds_client-0.3.0/wds_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/capabilities_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17329 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/job_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61562 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34758 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26209 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.030501 wds_client-0.3.0/wds_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/attribute_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/attribute_schema_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/backup_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/backup_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/backup_restore_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-13 14:04:39.000000 wds_client-0.3.0/wds_client/models/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/clone_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/clone_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/clone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/db_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/db_validationcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/db_validationcomponent_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/disk_space_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/disk_space_component_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/generic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/generic_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/import_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/job_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/record_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/models/version_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-05-13 14:04:40.000000 wds_client-0.3.0/wds_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:37.030501 wds_client-0.3.0/wds_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 14:06:36.000000 wds_client-0.3.0/wds_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-13 14:06:37.000000 wds_client-0.3.0/wds_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:06:36.000000 wds_client-0.3.0/wds_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 14:06:36.000000 wds_client-0.3.0/wds_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 14:06:36.000000 wds_client-0.3.0/wds_client.egg-info/top_level.txt
```

### Comparing `wds-client-0.2.99/README.md` & `wds_client-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This page lists current APIs.
 As of v0.2, all APIs are subject to change without notice.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v0.2
-- Package version: 0.2.99
+- Package version: 0.3.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -56,105 +56,104 @@
 
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = wds_client.Configuration(
     host = "http://localhost"
 )
 
-# The client must configure the authentication and authorization parameters
-# in accordance with the API server security policy.
-# Examples for each auth method are provided below, use the example that
-# satisfies your auth use case.
-
-# Configure Bearer authorization: bearerAuth
-configuration = wds_client.Configuration(
-    access_token = 'YOUR_BEARER_TOKEN'
-)
 
 
 # Enter a context with an instance of the API client
 with wds_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = wds_client.CloningApi(api_client)
-    v = 'v0.2' # str | API version (default to 'v0.2')
-backup_restore_request = wds_client.BackupRestoreRequest() # BackupRestoreRequest | A backup request
-
+    api_instance = wds_client.CapabilitiesApi(api_client)
+    
     try:
-        # Create a backup of all WDS data
-        api_response = api_instance.create_backup(v, backup_restore_request)
+        # Describes the capabilities of this WDS version.
+        api_response = api_instance.capabilities()
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling CloningApi->create_backup: %s\n" % e)
+        print("Exception when calling CapabilitiesApi->capabilities: %s\n" % e)
     
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*CapabilitiesApi* | [**capabilities**](docs/CapabilitiesApi.md#capabilities) | **GET** /capabilities/v1 | Describes the capabilities of this WDS version.
 *CloningApi* | [**create_backup**](docs/CloningApi.md#create_backup) | **POST** /backup/{v} | Create a backup of all WDS data
 *CloningApi* | [**get_backup_status**](docs/CloningApi.md#get_backup_status) | **GET** /backup/{v}/{trackingId} | Check status of a WDS data backup
 *CloningApi* | [**get_clone_status**](docs/CloningApi.md#get_clone_status) | **GET** /clone/{v} | Check status of a WDS data clone
 *GeneralWDSInformationApi* | [**status_get**](docs/GeneralWDSInformationApi.md#status_get) | **GET** /status | Gets health status for WDS -- generated via Spring Boot Actuator (see https://docs.spring.io/spring-boot/docs/current/actuator-api/htmlsingle/#health for details)
 *GeneralWDSInformationApi* | [**version_get**](docs/GeneralWDSInformationApi.md#version_get) | **GET** /version | Gets related git and build version info for WDS -- generated via Spring Boot Actuator (see https://docs.spring.io/spring-boot/docs/current/actuator-api/htmlsingle/#info for details)
+*ImportApi* | [**import_v1**](docs/ImportApi.md#import_v1) | **POST** /{instanceUuid}/import/v1 | Import from a file
 *InstancesApi* | [**create_wds_instance**](docs/InstancesApi.md#create_wds_instance) | **POST** /instances/{v}/{instanceid} | Create an instance
 *InstancesApi* | [**delete_wds_instance**](docs/InstancesApi.md#delete_wds_instance) | **DELETE** /instances/{v}/{instanceid} | Delete an instance
 *InstancesApi* | [**list_wds_instances**](docs/InstancesApi.md#list_wds_instances) | **GET** /instances/{v} | List instances
+*JobApi* | [**job_status_v1**](docs/JobApi.md#job_status_v1) | **GET** /job/v1/{jobId} | Get status of a long-running job.
+*JobApi* | [**jobs_in_instance_v1**](docs/JobApi.md#jobs_in_instance_v1) | **GET** /job/v1/instance/{instanceUuid} | Get all jobs with a certain status under a particular instance.
 *RecordsApi* | [**batch_write_records**](docs/RecordsApi.md#batch_write_records) | **POST** /{instanceid}/batch/{v}/{type} | Batch write records
 *RecordsApi* | [**create_or_replace_record**](docs/RecordsApi.md#create_or_replace_record) | **PUT** /{instanceid}/records/{v}/{type}/{id} | Create or replace record
 *RecordsApi* | [**delete_record**](docs/RecordsApi.md#delete_record) | **DELETE** /{instanceid}/records/{v}/{type}/{id} | Delete record
 *RecordsApi* | [**get_record**](docs/RecordsApi.md#get_record) | **GET** /{instanceid}/records/{v}/{type}/{id} | Get record
 *RecordsApi* | [**get_records_as_tsv**](docs/RecordsApi.md#get_records_as_tsv) | **GET** /{instanceid}/tsv/{v}/{type} | Retrieve all records in record type as tsv.
 *RecordsApi* | [**query_records**](docs/RecordsApi.md#query_records) | **POST** /{instanceid}/search/{v}/{type} | Query records
 *RecordsApi* | [**update_record**](docs/RecordsApi.md#update_record) | **PATCH** /{instanceid}/records/{v}/{type}/{id} | Update record
 *RecordsApi* | [**upload_tsv**](docs/RecordsApi.md#upload_tsv) | **POST** /{instanceid}/tsv/{v}/{type} | Import records to a record type from a tsv file
+*SchemaApi* | [**delete_attribute**](docs/SchemaApi.md#delete_attribute) | **DELETE** /{instanceid}/types/{v}/{type}/{attribute} | Delete attribute from record type
 *SchemaApi* | [**delete_record_type**](docs/SchemaApi.md#delete_record_type) | **DELETE** /{instanceid}/types/{v}/{type} | Delete record type
 *SchemaApi* | [**describe_all_record_types**](docs/SchemaApi.md#describe_all_record_types) | **GET** /{instanceid}/types/{v} | Describe all record types
 *SchemaApi* | [**describe_record_type**](docs/SchemaApi.md#describe_record_type) | **GET** /{instanceid}/types/{v}/{type} | Describe record type
-*SnapshotsApi* | [**import_snapshot**](docs/SnapshotsApi.md#import_snapshot) | **POST** /{instanceid}/snapshots/{v}/{snapshotid} | Import a snapshot from Terra Data Repo
+*SchemaApi* | [**update_attribute**](docs/SchemaApi.md#update_attribute) | **PATCH** /{instanceid}/types/{v}/{type}/{attribute} | Update an attribute
 
 
 ## Documentation For Models
 
  - [App](docs/App.md)
+ - [AttributeDataType](docs/AttributeDataType.md)
  - [AttributeSchema](docs/AttributeSchema.md)
+ - [AttributeSchemaUpdate](docs/AttributeSchemaUpdate.md)
  - [BackupJob](docs/BackupJob.md)
  - [BackupJobAllOf](docs/BackupJobAllOf.md)
  - [BackupResponse](docs/BackupResponse.md)
  - [BackupRestoreRequest](docs/BackupRestoreRequest.md)
  - [BatchOperation](docs/BatchOperation.md)
  - [BatchRecordRequest](docs/BatchRecordRequest.md)
  - [BatchResponse](docs/BatchResponse.md)
  - [Build](docs/Build.md)
+ - [Capabilities](docs/Capabilities.md)
  - [CloneJob](docs/CloneJob.md)
  - [CloneJobAllOf](docs/CloneJobAllOf.md)
  - [CloneResponse](docs/CloneResponse.md)
  - [Commit](docs/Commit.md)
  - [Component](docs/Component.md)
  - [Components](docs/Components.md)
  - [DbComponent](docs/DbComponent.md)
  - [DbValidationcomponent](docs/DbValidationcomponent.md)
  - [DbValidationcomponentDetails](docs/DbValidationcomponentDetails.md)
  - [DiskSpaceComponent](docs/DiskSpaceComponent.md)
  - [DiskSpaceComponentDetails](docs/DiskSpaceComponentDetails.md)
  - [ErrorResponse](docs/ErrorResponse.md)
+ - [GenericJob](docs/GenericJob.md)
+ - [GenericJobAllOf](docs/GenericJobAllOf.md)
  - [Git](docs/Git.md)
+ - [ImportRequest](docs/ImportRequest.md)
  - [InlineObject](docs/InlineObject.md)
  - [Job](docs/Job.md)
+ - [JobV1](docs/JobV1.md)
  - [RecordQueryResponse](docs/RecordQueryResponse.md)
  - [RecordRequest](docs/RecordRequest.md)
  - [RecordResponse](docs/RecordResponse.md)
  - [RecordTypeSchema](docs/RecordTypeSchema.md)
- - [RequestBodySearch](docs/RequestBodySearch.md)
- - [SearchOperator](docs/SearchOperator.md)
+ - [SearchFilter](docs/SearchFilter.md)
  - [SearchRequest](docs/SearchRequest.md)
  - [SearchSortDirection](docs/SearchSortDirection.md)
- - [StackTraceElement](docs/StackTraceElement.md)
  - [StatusResponse](docs/StatusResponse.md)
  - [TsvUploadResponse](docs/TsvUploadResponse.md)
  - [VersionResponse](docs/VersionResponse.md)
 
 
 ## Documentation For Authorization
```

### Comparing `wds-client-0.2.99/setup.py` & `wds_client-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "wds-client"
-VERSION = "0.2.99"
+VERSION = "0.3.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `wds-client-0.2.99/test/test_app.py` & `wds_client-0.3.0/test/test_app.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_attribute_schema.py` & `wds_client-0.3.0/test/test_attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_backup_job.py` & `wds_client-0.3.0/test/test_backup_job.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,19 +33,20 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = wds_client.models.backup_job.BackupJob()  # noqa: E501
         if include_optional :
             return BackupJob(
                 job_id = '0', 
+                job_type = '0', 
                 status = 'QUEUED', 
                 created = '0', 
                 updated = '0', 
                 error_message = '0', 
-                exception = '0', 
+                input = None, 
                 result = wds_client.models.backup_response.BackupResponse(
                     filename = '0', 
                     requester = '0', 
                     description = '0', )
             )
         else :
             return BackupJob(
```

### Comparing `wds-client-0.2.99/test/test_backup_job_all_of.py` & `wds_client-0.3.0/test/test_backup_job_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         """Test BackupJobAllOf
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = wds_client.models.backup_job_all_of.BackupJobAllOf()  # noqa: E501
         if include_optional :
             return BackupJobAllOf(
+                input = None, 
                 result = wds_client.models.backup_response.BackupResponse(
                     filename = '0', 
                     requester = '0', 
                     description = '0', )
             )
         else :
             return BackupJobAllOf(
```

### Comparing `wds-client-0.2.99/test/test_backup_response.py` & `wds_client-0.3.0/test/test_backup_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_backup_restore_request.py` & `wds_client-0.3.0/test/test_backup_restore_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_batch_operation.py` & `wds_client-0.3.0/test/test_batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_batch_record_request.py` & `wds_client-0.3.0/test/test_batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_batch_response.py` & `wds_client-0.3.0/test/test_batch_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_build.py` & `wds_client-0.3.0/test/test_build.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_clone_job.py` & `wds_client-0.3.0/test/test_clone_job.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,19 +33,20 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = wds_client.models.clone_job.CloneJob()  # noqa: E501
         if include_optional :
             return CloneJob(
                 job_id = '0', 
+                job_type = '0', 
                 status = 'QUEUED', 
                 created = '0', 
                 updated = '0', 
                 error_message = '0', 
-                exception = '0', 
+                input = None, 
                 result = wds_client.models.clone_response.CloneResponse(
                     sourceworkspaceid = '0', 
                     clonestatus = '0', )
             )
         else :
             return CloneJob(
                 job_id = '0',
```

### Comparing `wds-client-0.2.99/test/test_clone_job_all_of.py` & `wds_client-0.3.0/test/test_clone_job_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         """Test CloneJobAllOf
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = wds_client.models.clone_job_all_of.CloneJobAllOf()  # noqa: E501
         if include_optional :
             return CloneJobAllOf(
+                input = None, 
                 result = wds_client.models.clone_response.CloneResponse(
                     sourceworkspaceid = '0', 
                     clonestatus = '0', )
             )
         else :
             return CloneJobAllOf(
         )
```

### Comparing `wds-client-0.2.99/test/test_clone_response.py` & `wds_client-0.3.0/test/test_clone_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_cloning_api.py` & `wds_client-0.3.0/test/test_cloning_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_commit.py` & `wds_client-0.3.0/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_component.py` & `wds_client-0.3.0/test/test_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_components.py` & `wds_client-0.3.0/test/test_components.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_db_component.py` & `wds_client-0.3.0/test/test_db_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_db_validationcomponent.py` & `wds_client-0.3.0/test/test_db_validationcomponent.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_db_validationcomponent_details.py` & `wds_client-0.3.0/test/test_db_validationcomponent_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_disk_space_component.py` & `wds_client-0.3.0/test/test_disk_space_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_disk_space_component_details.py` & `wds_client-0.3.0/test/test_disk_space_component_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_error_response.py` & `wds_client-0.3.0/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_general_wds_information_api.py` & `wds_client-0.3.0/test/test_general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_git.py` & `wds_client-0.3.0/test/test_git.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_inline_object.py` & `wds_client-0.3.0/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_instances_api.py` & `wds_client-0.3.0/test/test_instances_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_job.py` & `wds_client-0.3.0/test/test_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = wds_client.models.job.Job()  # noqa: E501
         if include_optional :
             return Job(
                 job_id = '0', 
+                job_type = '0', 
                 status = 'QUEUED', 
                 created = '0', 
                 updated = '0', 
-                error_message = '0', 
-                exception = '0'
+                error_message = '0'
             )
         else :
             return Job(
                 job_id = '0',
                 status = 'QUEUED',
                 created = '0',
                 updated = '0',
```

### Comparing `wds-client-0.2.99/test/test_record_query_response.py` & `wds_client-0.3.0/test/test_record_query_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,19 @@
         # model = wds_client.models.record_query_response.RecordQueryResponse()  # noqa: E501
         if include_optional :
             return RecordQueryResponse(
                 search_request = wds_client.models.search_request.SearchRequest(
                     offset = 0, 
                     limit = 0, 
                     sort = 'ASC', 
-                    sort_attribute = '0', ), 
+                    sort_attribute = '0', 
+                    filter = wds_client.models.search_filter.SearchFilter(
+                        ids = [
+                            '0'
+                            ], ), ), 
                 total_records = 56, 
                 records = [
                     wds_client.models.record_response.RecordResponse(
                         id = '0', 
                         type = '0', 
                         attributes = {
   "stringAttr": "string",
@@ -65,15 +69,19 @@
             )
         else :
             return RecordQueryResponse(
                 search_request = wds_client.models.search_request.SearchRequest(
                     offset = 0, 
                     limit = 0, 
                     sort = 'ASC', 
-                    sort_attribute = '0', ),
+                    sort_attribute = '0', 
+                    filter = wds_client.models.search_filter.SearchFilter(
+                        ids = [
+                            '0'
+                            ], ), ),
                 total_records = 56,
                 records = [
                     wds_client.models.record_response.RecordResponse(
                         id = '0', 
                         type = '0', 
                         attributes = {
   "stringAttr": "string",
```

### Comparing `wds-client-0.2.99/test/test_record_request.py` & `wds_client-0.3.0/test/test_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_record_response.py` & `wds_client-0.3.0/test/test_record_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_record_type_schema.py` & `wds_client-0.3.0/test/test_record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_records_api.py` & `wds_client-0.3.0/test/test_records_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_request_body_search.py` & `wds_client-0.3.0/test/test_import_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,43 +12,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.request_body_search import RequestBodySearch  # noqa: E501
+from wds_client.models.import_request import ImportRequest  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestRequestBodySearch(unittest.TestCase):
-    """RequestBodySearch unit test stubs"""
+class TestImportRequest(unittest.TestCase):
+    """ImportRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test RequestBodySearch
+        """Test ImportRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.request_body_search.RequestBodySearch()  # noqa: E501
+        # model = wds_client.models.import_request.ImportRequest()  # noqa: E501
         if include_optional :
-            return RequestBodySearch(
-                terms = '0', 
-                operator = 'and'
+            return ImportRequest(
+                type = 'PFB', 
+                url = '0', 
+                options = { }
             )
         else :
-            return RequestBodySearch(
-                terms = '0',
+            return ImportRequest(
+                type = 'PFB',
+                url = '0',
         )
 
-    def testRequestBodySearch(self):
-        """Test RequestBodySearch"""
+    def testImportRequest(self):
+        """Test ImportRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.99/test/test_schema_api.py` & `wds_client-0.3.0/test/test_schema_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 
     def setUp(self):
         self.api = wds_client.api.schema_api.SchemaApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
+    def test_delete_attribute(self):
+        """Test case for delete_attribute
+
+        Delete attribute from record type  # noqa: E501
+        """
+        pass
+
     def test_delete_record_type(self):
         """Test case for delete_record_type
 
         Delete record type  # noqa: E501
         """
         pass
 
@@ -45,10 +52,17 @@
     def test_describe_record_type(self):
         """Test case for describe_record_type
 
         Describe record type  # noqa: E501
         """
         pass
 
+    def test_update_attribute(self):
+        """Test case for update_attribute
+
+        Update an attribute  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.99/test/test_search_operator.py` & `wds_client-0.3.0/test/test_search_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,40 +12,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.search_operator import SearchOperator  # noqa: E501
+from wds_client.models.search_filter import SearchFilter  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestSearchOperator(unittest.TestCase):
-    """SearchOperator unit test stubs"""
+class TestSearchFilter(unittest.TestCase):
+    """SearchFilter unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SearchOperator
+        """Test SearchFilter
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.search_operator.SearchOperator()  # noqa: E501
+        # model = wds_client.models.search_filter.SearchFilter()  # noqa: E501
         if include_optional :
-            return SearchOperator(
+            return SearchFilter(
+                ids = [
+                    '0'
+                    ]
             )
         else :
-            return SearchOperator(
+            return SearchFilter(
         )
 
-    def testSearchOperator(self):
-        """Test SearchOperator"""
+    def testSearchFilter(self):
+        """Test SearchFilter"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.99/test/test_search_request.py` & `wds_client-0.3.0/test/test_search_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,19 @@
             optional params are included """
         # model = wds_client.models.search_request.SearchRequest()  # noqa: E501
         if include_optional :
             return SearchRequest(
                 offset = 0, 
                 limit = 0, 
                 sort = 'ASC', 
-                sort_attribute = '0'
+                sort_attribute = '0', 
+                filter = wds_client.models.search_filter.SearchFilter(
+                    ids = [
+                        '0'
+                        ], )
             )
         else :
             return SearchRequest(
         )
 
     def testSearchRequest(self):
         """Test SearchRequest"""
```

### Comparing `wds-client-0.2.99/test/test_search_sort_direction.py` & `wds_client-0.3.0/test/test_search_sort_direction.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_snapshots_api.py` & `wds_client-0.3.0/test/test_import_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import wds_client
-from wds_client.api.snapshots_api import SnapshotsApi  # noqa: E501
+from wds_client.api.import_api import ImportApi  # noqa: E501
 from wds_client.rest import ApiException
 
 
-class TestSnapshotsApi(unittest.TestCase):
-    """SnapshotsApi unit test stubs"""
+class TestImportApi(unittest.TestCase):
+    """ImportApi unit test stubs"""
 
     def setUp(self):
-        self.api = wds_client.api.snapshots_api.SnapshotsApi()  # noqa: E501
+        self.api = wds_client.api.import_api.ImportApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_import_snapshot(self):
-        """Test case for import_snapshot
+    def test_import_v1(self):
+        """Test case for import_v1
 
-        Import a snapshot from Terra Data Repo  # noqa: E501
+        Import from a file  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.99/test/test_stack_trace_element.py` & `wds_client-0.3.0/test/test_generic_job_all_of.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,48 +12,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.stack_trace_element import StackTraceElement  # noqa: E501
+from wds_client.models.generic_job_all_of import GenericJobAllOf  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestStackTraceElement(unittest.TestCase):
-    """StackTraceElement unit test stubs"""
+class TestGenericJobAllOf(unittest.TestCase):
+    """GenericJobAllOf unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test StackTraceElement
+        """Test GenericJobAllOf
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.stack_trace_element.StackTraceElement()  # noqa: E501
+        # model = wds_client.models.generic_job_all_of.GenericJobAllOf()  # noqa: E501
         if include_optional :
-            return StackTraceElement(
-                class_name = '0', 
-                method_name = '0', 
-                file_name = '0', 
-                line_number = 56
+            return GenericJobAllOf(
+                input = None, 
+                result = None
             )
         else :
-            return StackTraceElement(
-                class_name = '0',
-                method_name = '0',
-                file_name = '0',
-                line_number = 56,
+            return GenericJobAllOf(
         )
 
-    def testStackTraceElement(self):
-        """Test StackTraceElement"""
+    def testGenericJobAllOf(self):
+        """Test GenericJobAllOf"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.99/test/test_status_response.py` & `wds_client-0.3.0/test/test_status_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_tsv_upload_response.py` & `wds_client-0.3.0/test/test_tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/test/test_version_response.py` & `wds_client-0.3.0/test/test_version_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/__init__.py` & `wds_client-0.3.0/wds_client/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,58 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Workspace Data Service
 
     This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.2.99"
-
-# import apis into sdk package
-from wds_client.api.cloning_api import CloningApi
-from wds_client.api.general_wds_information_api import GeneralWDSInformationApi
-from wds_client.api.instances_api import InstancesApi
-from wds_client.api.records_api import RecordsApi
-from wds_client.api.schema_api import SchemaApi
-from wds_client.api.snapshots_api import SnapshotsApi
-
-# import ApiClient
-from wds_client.api_client import ApiClient
-from wds_client.configuration import Configuration
-from wds_client.exceptions import OpenApiException
-from wds_client.exceptions import ApiTypeError
-from wds_client.exceptions import ApiValueError
-from wds_client.exceptions import ApiKeyError
-from wds_client.exceptions import ApiException
-# import models into sdk package
+# import models into model package
 from wds_client.models.app import App
+from wds_client.models.attribute_data_type import AttributeDataType
 from wds_client.models.attribute_schema import AttributeSchema
+from wds_client.models.attribute_schema_update import AttributeSchemaUpdate
 from wds_client.models.backup_job import BackupJob
 from wds_client.models.backup_job_all_of import BackupJobAllOf
 from wds_client.models.backup_response import BackupResponse
 from wds_client.models.backup_restore_request import BackupRestoreRequest
 from wds_client.models.batch_operation import BatchOperation
 from wds_client.models.batch_record_request import BatchRecordRequest
 from wds_client.models.batch_response import BatchResponse
 from wds_client.models.build import Build
+from wds_client.models.capabilities import Capabilities
 from wds_client.models.clone_job import CloneJob
 from wds_client.models.clone_job_all_of import CloneJobAllOf
 from wds_client.models.clone_response import CloneResponse
 from wds_client.models.commit import Commit
 from wds_client.models.component import Component
 from wds_client.models.components import Components
 from wds_client.models.db_component import DbComponent
 from wds_client.models.db_validationcomponent import DbValidationcomponent
 from wds_client.models.db_validationcomponent_details import DbValidationcomponentDetails
 from wds_client.models.disk_space_component import DiskSpaceComponent
 from wds_client.models.disk_space_component_details import DiskSpaceComponentDetails
 from wds_client.models.error_response import ErrorResponse
+from wds_client.models.generic_job import GenericJob
+from wds_client.models.generic_job_all_of import GenericJobAllOf
 from wds_client.models.git import Git
+from wds_client.models.import_request import ImportRequest
 from wds_client.models.inline_object import InlineObject
 from wds_client.models.job import Job
+from wds_client.models.job_v1 import JobV1
 from wds_client.models.record_query_response import RecordQueryResponse
 from wds_client.models.record_request import RecordRequest
 from wds_client.models.record_response import RecordResponse
 from wds_client.models.record_type_schema import RecordTypeSchema
-from wds_client.models.request_body_search import RequestBodySearch
-from wds_client.models.search_operator import SearchOperator
+from wds_client.models.search_filter import SearchFilter
 from wds_client.models.search_request import SearchRequest
 from wds_client.models.search_sort_direction import SearchSortDirection
-from wds_client.models.stack_trace_element import StackTraceElement
 from wds_client.models.status_response import StatusResponse
 from wds_client.models.tsv_upload_response import TsvUploadResponse
 from wds_client.models.version_response import VersionResponse
-
```

### Comparing `wds-client-0.2.99/wds_client/api/cloning_api.py` & `wds_client-0.3.0/wds_client/api/cloning_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/api/general_wds_information_api.py` & `wds_client-0.3.0/wds_client/api/general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/api/instances_api.py` & `wds_client-0.3.0/wds_client/api/instances_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/api/records_api.py` & `wds_client-0.3.0/wds_client/api/records_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/api_client.py` & `wds_client-0.3.0/wds_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'wds-client/0.2.99/python'
+        self.user_agent = 'wds-client/0.3.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `wds-client-0.2.99/wds_client/configuration.py` & `wds_client-0.3.0/wds_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v0.2\n"\
-               "SDK Package Version: 0.2.99".\
+               "SDK Package Version: 0.3.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `wds-client-0.2.99/wds_client/exceptions.py` & `wds_client-0.3.0/wds_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/__init__.py` & `wds_client-0.3.0/wds_client/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,80 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     Workspace Data Service
 
     This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-# import models into model package
+__version__ = "0.3.0"
+
+# import apis into sdk package
+from wds_client.api.capabilities_api import CapabilitiesApi
+from wds_client.api.cloning_api import CloningApi
+from wds_client.api.general_wds_information_api import GeneralWDSInformationApi
+from wds_client.api.import_api import ImportApi
+from wds_client.api.instances_api import InstancesApi
+from wds_client.api.job_api import JobApi
+from wds_client.api.records_api import RecordsApi
+from wds_client.api.schema_api import SchemaApi
+
+# import ApiClient
+from wds_client.api_client import ApiClient
+from wds_client.configuration import Configuration
+from wds_client.exceptions import OpenApiException
+from wds_client.exceptions import ApiTypeError
+from wds_client.exceptions import ApiValueError
+from wds_client.exceptions import ApiKeyError
+from wds_client.exceptions import ApiException
+# import models into sdk package
 from wds_client.models.app import App
+from wds_client.models.attribute_data_type import AttributeDataType
 from wds_client.models.attribute_schema import AttributeSchema
+from wds_client.models.attribute_schema_update import AttributeSchemaUpdate
 from wds_client.models.backup_job import BackupJob
 from wds_client.models.backup_job_all_of import BackupJobAllOf
 from wds_client.models.backup_response import BackupResponse
 from wds_client.models.backup_restore_request import BackupRestoreRequest
 from wds_client.models.batch_operation import BatchOperation
 from wds_client.models.batch_record_request import BatchRecordRequest
 from wds_client.models.batch_response import BatchResponse
 from wds_client.models.build import Build
+from wds_client.models.capabilities import Capabilities
 from wds_client.models.clone_job import CloneJob
 from wds_client.models.clone_job_all_of import CloneJobAllOf
 from wds_client.models.clone_response import CloneResponse
 from wds_client.models.commit import Commit
 from wds_client.models.component import Component
 from wds_client.models.components import Components
 from wds_client.models.db_component import DbComponent
 from wds_client.models.db_validationcomponent import DbValidationcomponent
 from wds_client.models.db_validationcomponent_details import DbValidationcomponentDetails
 from wds_client.models.disk_space_component import DiskSpaceComponent
 from wds_client.models.disk_space_component_details import DiskSpaceComponentDetails
 from wds_client.models.error_response import ErrorResponse
+from wds_client.models.generic_job import GenericJob
+from wds_client.models.generic_job_all_of import GenericJobAllOf
 from wds_client.models.git import Git
+from wds_client.models.import_request import ImportRequest
 from wds_client.models.inline_object import InlineObject
 from wds_client.models.job import Job
+from wds_client.models.job_v1 import JobV1
 from wds_client.models.record_query_response import RecordQueryResponse
 from wds_client.models.record_request import RecordRequest
 from wds_client.models.record_response import RecordResponse
 from wds_client.models.record_type_schema import RecordTypeSchema
-from wds_client.models.request_body_search import RequestBodySearch
-from wds_client.models.search_operator import SearchOperator
+from wds_client.models.search_filter import SearchFilter
 from wds_client.models.search_request import SearchRequest
 from wds_client.models.search_sort_direction import SearchSortDirection
-from wds_client.models.stack_trace_element import StackTraceElement
 from wds_client.models.status_response import StatusResponse
 from wds_client.models.tsv_upload_response import TsvUploadResponse
 from wds_client.models.version_response import VersionResponse
+
```

### Comparing `wds-client-0.2.99/wds_client/models/app.py` & `wds_client-0.3.0/wds_client/models/app.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/attribute_schema.py` & `wds_client-0.3.0/wds_client/models/attribute_schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'name': 'str',
-        'datatype': 'str',
+        'datatype': 'AttributeDataType',
         'relates_to': 'str'
     }
 
     attribute_map = {
         'name': 'name',
         'datatype': 'datatype',
         'relates_to': 'relatesTo'
@@ -85,38 +85,30 @@
 
         self._name = name
 
     @property
     def datatype(self):
         """Gets the datatype of this AttributeSchema.  # noqa: E501
 
-        Datatype of this attribute. The enum of datatypes is in flux and will change. Please comment at https://docs.google.com/document/d/1d352ZoN5kEYWPjy0NqqWGxdf7HEu5VEdrLmiAv7dMmQ/edit#heading=h.naxag0augkgf.   # noqa: E501
 
         :return: The datatype of this AttributeSchema.  # noqa: E501
-        :rtype: str
+        :rtype: AttributeDataType
         """
         return self._datatype
 
     @datatype.setter
     def datatype(self, datatype):
         """Sets the datatype of this AttributeSchema.
 
-        Datatype of this attribute. The enum of datatypes is in flux and will change. Please comment at https://docs.google.com/document/d/1d352ZoN5kEYWPjy0NqqWGxdf7HEu5VEdrLmiAv7dMmQ/edit#heading=h.naxag0augkgf.   # noqa: E501
 
         :param datatype: The datatype of this AttributeSchema.  # noqa: E501
-        :type: str
+        :type: AttributeDataType
         """
         if self.local_vars_configuration.client_side_validation and datatype is None:  # noqa: E501
             raise ValueError("Invalid value for `datatype`, must not be `None`")  # noqa: E501
-        allowed_values = ["BOOLEAN", "NUMBER", "DATE", "DATE_TIME", "STRING", "JSON", "RELATION", "FILE", "ARRAY_OF_BOOLEAN", "ARRAY_OF_STRING", "ARRAY_OF_NUMBER", "ARRAY_OF_DATE", "ARRAY_OF_DATE_TIME", "ARRAY_OF_RELATION", "ARRAY_OF_FILE"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and datatype not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `datatype` ({0}), must be one of {1}"  # noqa: E501
-                .format(datatype, allowed_values)
-            )
 
         self._datatype = datatype
 
     @property
     def relates_to(self):
         """Gets the relates_to of this AttributeSchema.  # noqa: E501
```

### Comparing `wds-client-0.2.99/wds_client/models/backup_job.py` & `wds_client-0.3.0/wds_client/models/backup_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,55 +30,60 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'job_id': 'str',
+        'job_type': 'str',
         'status': 'str',
         'created': 'str',
         'updated': 'str',
         'error_message': 'str',
-        'exception': 'str',
+        'input': 'object',
         'result': 'BackupResponse'
     }
 
     attribute_map = {
         'job_id': 'jobId',
+        'job_type': 'jobType',
         'status': 'status',
         'created': 'created',
         'updated': 'updated',
         'error_message': 'errorMessage',
-        'exception': 'exception',
+        'input': 'input',
         'result': 'result'
     }
 
-    def __init__(self, job_id=None, status=None, created=None, updated=None, error_message=None, exception=None, result=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, job_id=None, job_type=None, status=None, created=None, updated=None, error_message=None, input=None, result=None, local_vars_configuration=None):  # noqa: E501
         """BackupJob - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._job_id = None
+        self._job_type = None
         self._status = None
         self._created = None
         self._updated = None
         self._error_message = None
-        self._exception = None
+        self._input = None
         self._result = None
         self.discriminator = None
 
         self.job_id = job_id
+        if job_type is not None:
+            self.job_type = job_type
         self.status = status
         self.created = created
         self.updated = updated
         if error_message is not None:
             self.error_message = error_message
-        if exception is not None:
-            self.exception = exception
+        if input is not None:
+            self.input = input
         if result is not None:
             self.result = result
 
     @property
     def job_id(self):
         """Gets the job_id of this BackupJob.  # noqa: E501
 
@@ -98,14 +103,35 @@
         """
         if self.local_vars_configuration.client_side_validation and job_id is None:  # noqa: E501
             raise ValueError("Invalid value for `job_id`, must not be `None`")  # noqa: E501
 
         self._job_id = job_id
 
     @property
+    def job_type(self):
+        """Gets the job_type of this BackupJob.  # noqa: E501
+
+
+        :return: The job_type of this BackupJob.  # noqa: E501
+        :rtype: str
+        """
+        return self._job_type
+
+    @job_type.setter
+    def job_type(self, job_type):
+        """Sets the job_type of this BackupJob.
+
+
+        :param job_type: The job_type of this BackupJob.  # noqa: E501
+        :type: str
+        """
+
+        self._job_type = job_type
+
+    @property
     def status(self):
         """Gets the status of this BackupJob.  # noqa: E501
 
 
         :return: The status of this BackupJob.  # noqa: E501
         :rtype: str
         """
@@ -194,33 +220,35 @@
         :param error_message: The error_message of this BackupJob.  # noqa: E501
         :type: str
         """
 
         self._error_message = error_message
 
     @property
-    def exception(self):
-        """Gets the exception of this BackupJob.  # noqa: E501
+    def input(self):
+        """Gets the input of this BackupJob.  # noqa: E501
 
+        Input arguments; expected to be empty.  # noqa: E501
 
-        :return: The exception of this BackupJob.  # noqa: E501
-        :rtype: str
+        :return: The input of this BackupJob.  # noqa: E501
+        :rtype: object
         """
-        return self._exception
+        return self._input
 
-    @exception.setter
-    def exception(self, exception):
-        """Sets the exception of this BackupJob.
+    @input.setter
+    def input(self, input):
+        """Sets the input of this BackupJob.
 
+        Input arguments; expected to be empty.  # noqa: E501
 
-        :param exception: The exception of this BackupJob.  # noqa: E501
-        :type: str
+        :param input: The input of this BackupJob.  # noqa: E501
+        :type: object
         """
 
-        self._exception = exception
+        self._input = input
 
     @property
     def result(self):
         """Gets the result of this BackupJob.  # noqa: E501
 
 
         :return: The result of this BackupJob.  # noqa: E501
```

### Comparing `wds-client-0.2.99/wds_client/models/backup_job_all_of.py` & `wds_client-0.3.0/wds_client/models/capabilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,68 +14,68 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class BackupJobAllOf(object):
+class Capabilities(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'result': 'BackupResponse'
+        'capabilities': 'bool'
     }
 
     attribute_map = {
-        'result': 'result'
+        'capabilities': 'capabilities'
     }
 
-    def __init__(self, result=None, local_vars_configuration=None):  # noqa: E501
-        """BackupJobAllOf - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, capabilities=None, local_vars_configuration=None):  # noqa: E501
+        """Capabilities - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._result = None
+        self._capabilities = None
         self.discriminator = None
 
-        if result is not None:
-            self.result = result
+        if capabilities is not None:
+            self.capabilities = capabilities
 
     @property
-    def result(self):
-        """Gets the result of this BackupJobAllOf.  # noqa: E501
+    def capabilities(self):
+        """Gets the capabilities of this Capabilities.  # noqa: E501
 
 
-        :return: The result of this BackupJobAllOf.  # noqa: E501
-        :rtype: BackupResponse
+        :return: The capabilities of this Capabilities.  # noqa: E501
+        :rtype: bool
         """
-        return self._result
+        return self._capabilities
 
-    @result.setter
-    def result(self, result):
-        """Sets the result of this BackupJobAllOf.
+    @capabilities.setter
+    def capabilities(self, capabilities):
+        """Sets the capabilities of this Capabilities.
 
 
-        :param result: The result of this BackupJobAllOf.  # noqa: E501
-        :type: BackupResponse
+        :param capabilities: The capabilities of this Capabilities.  # noqa: E501
+        :type: bool
         """
 
-        self._result = result
+        self._capabilities = capabilities
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -103,18 +103,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BackupJobAllOf):
+        if not isinstance(other, Capabilities):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, BackupJobAllOf):
+        if not isinstance(other, Capabilities):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds-client-0.2.99/wds_client/models/backup_response.py` & `wds_client-0.3.0/wds_client/models/backup_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/backup_restore_request.py` & `wds_client-0.3.0/wds_client/models/backup_restore_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/batch_operation.py` & `wds_client-0.3.0/wds_client/models/batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/batch_record_request.py` & `wds_client-0.3.0/wds_client/models/batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/batch_response.py` & `wds_client-0.3.0/wds_client/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/build.py` & `wds_client-0.3.0/wds_client/models/build.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/clone_job.py` & `wds_client-0.3.0/wds_client/models/clone_job.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,55 +30,60 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'job_id': 'str',
+        'job_type': 'str',
         'status': 'str',
         'created': 'str',
         'updated': 'str',
         'error_message': 'str',
-        'exception': 'str',
+        'input': 'object',
         'result': 'CloneResponse'
     }
 
     attribute_map = {
         'job_id': 'jobId',
+        'job_type': 'jobType',
         'status': 'status',
         'created': 'created',
         'updated': 'updated',
         'error_message': 'errorMessage',
-        'exception': 'exception',
+        'input': 'input',
         'result': 'result'
     }
 
-    def __init__(self, job_id=None, status=None, created=None, updated=None, error_message=None, exception=None, result=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, job_id=None, job_type=None, status=None, created=None, updated=None, error_message=None, input=None, result=None, local_vars_configuration=None):  # noqa: E501
         """CloneJob - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._job_id = None
+        self._job_type = None
         self._status = None
         self._created = None
         self._updated = None
         self._error_message = None
-        self._exception = None
+        self._input = None
         self._result = None
         self.discriminator = None
 
         self.job_id = job_id
+        if job_type is not None:
+            self.job_type = job_type
         self.status = status
         self.created = created
         self.updated = updated
         if error_message is not None:
             self.error_message = error_message
-        if exception is not None:
-            self.exception = exception
+        if input is not None:
+            self.input = input
         if result is not None:
             self.result = result
 
     @property
     def job_id(self):
         """Gets the job_id of this CloneJob.  # noqa: E501
 
@@ -98,14 +103,35 @@
         """
         if self.local_vars_configuration.client_side_validation and job_id is None:  # noqa: E501
             raise ValueError("Invalid value for `job_id`, must not be `None`")  # noqa: E501
 
         self._job_id = job_id
 
     @property
+    def job_type(self):
+        """Gets the job_type of this CloneJob.  # noqa: E501
+
+
+        :return: The job_type of this CloneJob.  # noqa: E501
+        :rtype: str
+        """
+        return self._job_type
+
+    @job_type.setter
+    def job_type(self, job_type):
+        """Sets the job_type of this CloneJob.
+
+
+        :param job_type: The job_type of this CloneJob.  # noqa: E501
+        :type: str
+        """
+
+        self._job_type = job_type
+
+    @property
     def status(self):
         """Gets the status of this CloneJob.  # noqa: E501
 
 
         :return: The status of this CloneJob.  # noqa: E501
         :rtype: str
         """
@@ -194,33 +220,35 @@
         :param error_message: The error_message of this CloneJob.  # noqa: E501
         :type: str
         """
 
         self._error_message = error_message
 
     @property
-    def exception(self):
-        """Gets the exception of this CloneJob.  # noqa: E501
+    def input(self):
+        """Gets the input of this CloneJob.  # noqa: E501
 
+        Input arguments; expected to be empty.  # noqa: E501
 
-        :return: The exception of this CloneJob.  # noqa: E501
-        :rtype: str
+        :return: The input of this CloneJob.  # noqa: E501
+        :rtype: object
         """
-        return self._exception
+        return self._input
 
-    @exception.setter
-    def exception(self, exception):
-        """Sets the exception of this CloneJob.
+    @input.setter
+    def input(self, input):
+        """Sets the input of this CloneJob.
 
+        Input arguments; expected to be empty.  # noqa: E501
 
-        :param exception: The exception of this CloneJob.  # noqa: E501
-        :type: str
+        :param input: The input of this CloneJob.  # noqa: E501
+        :type: object
         """
 
-        self._exception = exception
+        self._input = input
 
     @property
     def result(self):
         """Gets the result of this CloneJob.  # noqa: E501
 
 
         :return: The result of this CloneJob.  # noqa: E501
```

### Comparing `wds-client-0.2.99/wds_client/models/clone_job_all_of.py` & `wds_client-0.3.0/wds_client/models/inline_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,68 +14,71 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class CloneJobAllOf(object):
+class InlineObject(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'result': 'CloneResponse'
+        'records': 'file'
     }
 
     attribute_map = {
-        'result': 'result'
+        'records': 'records'
     }
 
-    def __init__(self, result=None, local_vars_configuration=None):  # noqa: E501
-        """CloneJobAllOf - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, records=None, local_vars_configuration=None):  # noqa: E501
+        """InlineObject - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._result = None
+        self._records = None
         self.discriminator = None
 
-        if result is not None:
-            self.result = result
+        self.records = records
 
     @property
-    def result(self):
-        """Gets the result of this CloneJobAllOf.  # noqa: E501
+    def records(self):
+        """Gets the records of this InlineObject.  # noqa: E501
 
+        A valid TSV import file  # noqa: E501
 
-        :return: The result of this CloneJobAllOf.  # noqa: E501
-        :rtype: CloneResponse
+        :return: The records of this InlineObject.  # noqa: E501
+        :rtype: file
         """
-        return self._result
+        return self._records
 
-    @result.setter
-    def result(self, result):
-        """Sets the result of this CloneJobAllOf.
+    @records.setter
+    def records(self, records):
+        """Sets the records of this InlineObject.
 
+        A valid TSV import file  # noqa: E501
 
-        :param result: The result of this CloneJobAllOf.  # noqa: E501
-        :type: CloneResponse
+        :param records: The records of this InlineObject.  # noqa: E501
+        :type: file
         """
+        if self.local_vars_configuration.client_side_validation and records is None:  # noqa: E501
+            raise ValueError("Invalid value for `records`, must not be `None`")  # noqa: E501
 
-        self._result = result
+        self._records = records
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -103,18 +106,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CloneJobAllOf):
+        if not isinstance(other, InlineObject):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CloneJobAllOf):
+        if not isinstance(other, InlineObject):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds-client-0.2.99/wds_client/models/clone_response.py` & `wds_client-0.3.0/wds_client/models/clone_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/commit.py` & `wds_client-0.3.0/wds_client/models/commit.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/component.py` & `wds_client-0.3.0/wds_client/models/component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/components.py` & `wds_client-0.3.0/wds_client/models/components.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/db_component.py` & `wds_client-0.3.0/wds_client/models/db_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/db_validationcomponent.py` & `wds_client-0.3.0/wds_client/models/db_validationcomponent.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/db_validationcomponent_details.py` & `wds_client-0.3.0/wds_client/models/db_validationcomponent_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/disk_space_component.py` & `wds_client-0.3.0/wds_client/models/disk_space_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/disk_space_component_details.py` & `wds_client-0.3.0/wds_client/models/disk_space_component_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/error_response.py` & `wds_client-0.3.0/wds_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/git.py` & `wds_client-0.3.0/wds_client/models/git.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/inline_object.py` & `wds_client-0.3.0/wds_client/models/search_filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,71 +14,70 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class InlineObject(object):
+class SearchFilter(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'records': 'file'
+        'ids': 'list[str]'
     }
 
     attribute_map = {
-        'records': 'records'
+        'ids': 'ids'
     }
 
-    def __init__(self, records=None, local_vars_configuration=None):  # noqa: E501
-        """InlineObject - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, ids=None, local_vars_configuration=None):  # noqa: E501
+        """SearchFilter - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._records = None
+        self._ids = None
         self.discriminator = None
 
-        self.records = records
+        if ids is not None:
+            self.ids = ids
 
     @property
-    def records(self):
-        """Gets the records of this InlineObject.  # noqa: E501
+    def ids(self):
+        """Gets the ids of this SearchFilter.  # noqa: E501
 
-        A valid TSV import file  # noqa: E501
+        Record ids by which to filter the query  # noqa: E501
 
-        :return: The records of this InlineObject.  # noqa: E501
-        :rtype: file
+        :return: The ids of this SearchFilter.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._records
+        return self._ids
 
-    @records.setter
-    def records(self, records):
-        """Sets the records of this InlineObject.
+    @ids.setter
+    def ids(self, ids):
+        """Sets the ids of this SearchFilter.
 
-        A valid TSV import file  # noqa: E501
+        Record ids by which to filter the query  # noqa: E501
 
-        :param records: The records of this InlineObject.  # noqa: E501
-        :type: file
+        :param ids: The ids of this SearchFilter.  # noqa: E501
+        :type: list[str]
         """
-        if self.local_vars_configuration.client_side_validation and records is None:  # noqa: E501
-            raise ValueError("Invalid value for `records`, must not be `None`")  # noqa: E501
 
-        self._records = records
+        self._ids = ids
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -106,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InlineObject):
+        if not isinstance(other, SearchFilter):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, InlineObject):
+        if not isinstance(other, SearchFilter):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds-client-0.2.99/wds_client/models/job.py` & `wds_client-0.3.0/wds_client/models/job_v1.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class Job(object):
+class JobV1(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,193 +30,227 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'job_id': 'str',
+        'job_type': 'str',
+        'instance_id': 'str',
         'status': 'str',
-        'created': 'str',
-        'updated': 'str',
-        'error_message': 'str',
-        'exception': 'str'
+        'created': 'datetime',
+        'updated': 'datetime',
+        'error_message': 'str'
     }
 
     attribute_map = {
         'job_id': 'jobId',
+        'job_type': 'jobType',
+        'instance_id': 'instanceId',
         'status': 'status',
         'created': 'created',
         'updated': 'updated',
-        'error_message': 'errorMessage',
-        'exception': 'exception'
+        'error_message': 'errorMessage'
     }
 
-    def __init__(self, job_id=None, status=None, created=None, updated=None, error_message=None, exception=None, local_vars_configuration=None):  # noqa: E501
-        """Job - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, job_id=None, job_type=None, instance_id=None, status=None, created=None, updated=None, error_message=None, local_vars_configuration=None):  # noqa: E501
+        """JobV1 - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._job_id = None
+        self._job_type = None
+        self._instance_id = None
         self._status = None
         self._created = None
         self._updated = None
         self._error_message = None
-        self._exception = None
         self.discriminator = None
 
         self.job_id = job_id
+        self.job_type = job_type
+        self.instance_id = instance_id
         self.status = status
         self.created = created
         self.updated = updated
         if error_message is not None:
             self.error_message = error_message
-        if exception is not None:
-            self.exception = exception
 
     @property
     def job_id(self):
-        """Gets the job_id of this Job.  # noqa: E501
+        """Gets the job_id of this JobV1.  # noqa: E501
 
 
-        :return: The job_id of this Job.  # noqa: E501
+        :return: The job_id of this JobV1.  # noqa: E501
         :rtype: str
         """
         return self._job_id
 
     @job_id.setter
     def job_id(self, job_id):
-        """Sets the job_id of this Job.
+        """Sets the job_id of this JobV1.
 
 
-        :param job_id: The job_id of this Job.  # noqa: E501
+        :param job_id: The job_id of this JobV1.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and job_id is None:  # noqa: E501
             raise ValueError("Invalid value for `job_id`, must not be `None`")  # noqa: E501
 
         self._job_id = job_id
 
     @property
+    def job_type(self):
+        """Gets the job_type of this JobV1.  # noqa: E501
+
+
+        :return: The job_type of this JobV1.  # noqa: E501
+        :rtype: str
+        """
+        return self._job_type
+
+    @job_type.setter
+    def job_type(self, job_type):
+        """Sets the job_type of this JobV1.
+
+
+        :param job_type: The job_type of this JobV1.  # noqa: E501
+        :type: str
+        """
+        if self.local_vars_configuration.client_side_validation and job_type is None:  # noqa: E501
+            raise ValueError("Invalid value for `job_type`, must not be `None`")  # noqa: E501
+        allowed_values = ["DATA_IMPORT", "UNKNOWN"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and job_type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `job_type` ({0}), must be one of {1}"  # noqa: E501
+                .format(job_type, allowed_values)
+            )
+
+        self._job_type = job_type
+
+    @property
+    def instance_id(self):
+        """Gets the instance_id of this JobV1.  # noqa: E501
+
+
+        :return: The instance_id of this JobV1.  # noqa: E501
+        :rtype: str
+        """
+        return self._instance_id
+
+    @instance_id.setter
+    def instance_id(self, instance_id):
+        """Sets the instance_id of this JobV1.
+
+
+        :param instance_id: The instance_id of this JobV1.  # noqa: E501
+        :type: str
+        """
+        if self.local_vars_configuration.client_side_validation and instance_id is None:  # noqa: E501
+            raise ValueError("Invalid value for `instance_id`, must not be `None`")  # noqa: E501
+
+        self._instance_id = instance_id
+
+    @property
     def status(self):
-        """Gets the status of this Job.  # noqa: E501
+        """Gets the status of this JobV1.  # noqa: E501
 
 
-        :return: The status of this Job.  # noqa: E501
+        :return: The status of this JobV1.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this Job.
+        """Sets the status of this JobV1.
 
 
-        :param status: The status of this Job.  # noqa: E501
+        :param status: The status of this JobV1.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
             raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
-        allowed_values = ["QUEUED", "RUNNING", "SUCCEEDED", "ERROR", "CANCELLED", "UNKNOWN"]  # noqa: E501
+        allowed_values = ["CREATED", "QUEUED", "RUNNING", "SUCCEEDED", "ERROR", "CANCELLED", "UNKNOWN"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and status not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `status` ({0}), must be one of {1}"  # noqa: E501
                 .format(status, allowed_values)
             )
 
         self._status = status
 
     @property
     def created(self):
-        """Gets the created of this Job.  # noqa: E501
+        """Gets the created of this JobV1.  # noqa: E501
 
 
-        :return: The created of this Job.  # noqa: E501
-        :rtype: str
+        :return: The created of this JobV1.  # noqa: E501
+        :rtype: datetime
         """
         return self._created
 
     @created.setter
     def created(self, created):
-        """Sets the created of this Job.
+        """Sets the created of this JobV1.
 
 
-        :param created: The created of this Job.  # noqa: E501
-        :type: str
+        :param created: The created of this JobV1.  # noqa: E501
+        :type: datetime
         """
         if self.local_vars_configuration.client_side_validation and created is None:  # noqa: E501
             raise ValueError("Invalid value for `created`, must not be `None`")  # noqa: E501
 
         self._created = created
 
     @property
     def updated(self):
-        """Gets the updated of this Job.  # noqa: E501
+        """Gets the updated of this JobV1.  # noqa: E501
 
 
-        :return: The updated of this Job.  # noqa: E501
-        :rtype: str
+        :return: The updated of this JobV1.  # noqa: E501
+        :rtype: datetime
         """
         return self._updated
 
     @updated.setter
     def updated(self, updated):
-        """Sets the updated of this Job.
+        """Sets the updated of this JobV1.
 
 
-        :param updated: The updated of this Job.  # noqa: E501
-        :type: str
+        :param updated: The updated of this JobV1.  # noqa: E501
+        :type: datetime
         """
         if self.local_vars_configuration.client_side_validation and updated is None:  # noqa: E501
             raise ValueError("Invalid value for `updated`, must not be `None`")  # noqa: E501
 
         self._updated = updated
 
     @property
     def error_message(self):
-        """Gets the error_message of this Job.  # noqa: E501
+        """Gets the error_message of this JobV1.  # noqa: E501
 
 
-        :return: The error_message of this Job.  # noqa: E501
+        :return: The error_message of this JobV1.  # noqa: E501
         :rtype: str
         """
         return self._error_message
 
     @error_message.setter
     def error_message(self, error_message):
-        """Sets the error_message of this Job.
+        """Sets the error_message of this JobV1.
 
 
-        :param error_message: The error_message of this Job.  # noqa: E501
+        :param error_message: The error_message of this JobV1.  # noqa: E501
         :type: str
         """
 
         self._error_message = error_message
 
-    @property
-    def exception(self):
-        """Gets the exception of this Job.  # noqa: E501
-
-
-        :return: The exception of this Job.  # noqa: E501
-        :rtype: str
-        """
-        return self._exception
-
-    @exception.setter
-    def exception(self, exception):
-        """Sets the exception of this Job.
-
-
-        :param exception: The exception of this Job.  # noqa: E501
-        :type: str
-        """
-
-        self._exception = exception
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -243,18 +277,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Job):
+        if not isinstance(other, JobV1):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Job):
+        if not isinstance(other, JobV1):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds-client-0.2.99/wds_client/models/record_query_response.py` & `wds_client-0.3.0/wds_client/models/record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/record_request.py` & `wds_client-0.3.0/wds_client/models/record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/record_response.py` & `wds_client-0.3.0/wds_client/models/record_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/record_type_schema.py` & `wds_client-0.3.0/wds_client/models/record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/request_body_search.py` & `wds_client-0.3.0/wds_client/models/backup_job_all_of.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,97 +14,96 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class RequestBodySearch(object):
+class BackupJobAllOf(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'terms': 'str',
-        'operator': 'SearchOperator'
+        'input': 'object',
+        'result': 'BackupResponse'
     }
 
     attribute_map = {
-        'terms': 'terms',
-        'operator': 'operator'
+        'input': 'input',
+        'result': 'result'
     }
 
-    def __init__(self, terms=None, operator=None, local_vars_configuration=None):  # noqa: E501
-        """RequestBodySearch - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, input=None, result=None, local_vars_configuration=None):  # noqa: E501
+        """BackupJobAllOf - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._terms = None
-        self._operator = None
+        self._input = None
+        self._result = None
         self.discriminator = None
 
-        self.terms = terms
-        if operator is not None:
-            self.operator = operator
+        if input is not None:
+            self.input = input
+        if result is not None:
+            self.result = result
 
     @property
-    def terms(self):
-        """Gets the terms of this RequestBodySearch.  # noqa: E501
+    def input(self):
+        """Gets the input of this BackupJobAllOf.  # noqa: E501
 
-        Space-delimited list of terms on which to search  # noqa: E501
+        Input arguments; expected to be empty.  # noqa: E501
 
-        :return: The terms of this RequestBodySearch.  # noqa: E501
-        :rtype: str
+        :return: The input of this BackupJobAllOf.  # noqa: E501
+        :rtype: object
         """
-        return self._terms
+        return self._input
 
-    @terms.setter
-    def terms(self, terms):
-        """Sets the terms of this RequestBodySearch.
+    @input.setter
+    def input(self, input):
+        """Sets the input of this BackupJobAllOf.
 
-        Space-delimited list of terms on which to search  # noqa: E501
+        Input arguments; expected to be empty.  # noqa: E501
 
-        :param terms: The terms of this RequestBodySearch.  # noqa: E501
-        :type: str
+        :param input: The input of this BackupJobAllOf.  # noqa: E501
+        :type: object
         """
-        if self.local_vars_configuration.client_side_validation and terms is None:  # noqa: E501
-            raise ValueError("Invalid value for `terms`, must not be `None`")  # noqa: E501
 
-        self._terms = terms
+        self._input = input
 
     @property
-    def operator(self):
-        """Gets the operator of this RequestBodySearch.  # noqa: E501
+    def result(self):
+        """Gets the result of this BackupJobAllOf.  # noqa: E501
 
 
-        :return: The operator of this RequestBodySearch.  # noqa: E501
-        :rtype: SearchOperator
+        :return: The result of this BackupJobAllOf.  # noqa: E501
+        :rtype: BackupResponse
         """
-        return self._operator
+        return self._result
 
-    @operator.setter
-    def operator(self, operator):
-        """Sets the operator of this RequestBodySearch.
+    @result.setter
+    def result(self, result):
+        """Sets the result of this BackupJobAllOf.
 
 
-        :param operator: The operator of this RequestBodySearch.  # noqa: E501
-        :type: SearchOperator
+        :param result: The result of this BackupJobAllOf.  # noqa: E501
+        :type: BackupResponse
         """
 
-        self._operator = operator
+        self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -132,18 +131,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RequestBodySearch):
+        if not isinstance(other, BackupJobAllOf):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, RequestBodySearch):
+        if not isinstance(other, BackupJobAllOf):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds-client-0.2.99/wds_client/models/search_operator.py` & `wds_client-0.3.0/wds_client/models/search_sort_direction.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 import re  # noqa: F401
 
 import six
 
 from wds_client.configuration import Configuration
 
 
-class SearchOperator(object):
+class SearchSortDirection(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    AND = "and"
-    OR = "or"
+    ASC = "ASC"
+    DESC = "DESC"
 
-    allowable_values = [AND, OR]  # noqa: E501
+    allowable_values = [ASC, DESC]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -43,15 +43,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """SearchOperator - a model defined in OpenAPI"""  # noqa: E501
+        """SearchSortDirection - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -83,18 +83,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SearchOperator):
+        if not isinstance(other, SearchSortDirection):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SearchOperator):
+        if not isinstance(other, SearchSortDirection):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `wds-client-0.2.99/wds_client/models/search_request.py` & `wds_client-0.3.0/wds_client/models/search_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,44 +32,49 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'offset': 'int',
         'limit': 'int',
         'sort': 'SearchSortDirection',
-        'sort_attribute': 'str'
+        'sort_attribute': 'str',
+        'filter': 'SearchFilter'
     }
 
     attribute_map = {
         'offset': 'offset',
         'limit': 'limit',
         'sort': 'sort',
-        'sort_attribute': 'sortAttribute'
+        'sort_attribute': 'sortAttribute',
+        'filter': 'filter'
     }
 
-    def __init__(self, offset=0, limit=10, sort=None, sort_attribute=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, offset=0, limit=10, sort=None, sort_attribute=None, filter=None, local_vars_configuration=None):  # noqa: E501
         """SearchRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._offset = None
         self._limit = None
         self._sort = None
         self._sort_attribute = None
+        self._filter = None
         self.discriminator = None
 
         if offset is not None:
             self.offset = offset
         if limit is not None:
             self.limit = limit
         if sort is not None:
             self.sort = sort
         if sort_attribute is not None:
             self.sort_attribute = sort_attribute
+        if filter is not None:
+            self.filter = filter
 
     @property
     def offset(self):
         """Gets the offset of this SearchRequest.  # noqa: E501
 
         Pagination offset  # noqa: E501
 
@@ -160,14 +165,35 @@
 
         :param sort_attribute: The sort_attribute of this SearchRequest.  # noqa: E501
         :type: str
         """
 
         self._sort_attribute = sort_attribute
 
+    @property
+    def filter(self):
+        """Gets the filter of this SearchRequest.  # noqa: E501
+
+
+        :return: The filter of this SearchRequest.  # noqa: E501
+        :rtype: SearchFilter
+        """
+        return self._filter
+
+    @filter.setter
+    def filter(self, filter):
+        """Sets the filter of this SearchRequest.
+
+
+        :param filter: The filter of this SearchRequest.  # noqa: E501
+        :type: SearchFilter
+        """
+
+        self._filter = filter
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `wds-client-0.2.99/wds_client/models/status_response.py` & `wds_client-0.3.0/wds_client/models/status_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/tsv_upload_response.py` & `wds_client-0.3.0/wds_client/models/tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/models/version_response.py` & `wds_client-0.3.0/wds_client/models/version_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client/rest.py` & `wds_client-0.3.0/wds_client/rest.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.99/wds_client.egg-info/SOURCES.txt` & `wds_client-0.3.0/wds_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,101 +1,115 @@
 README.md
 setup.cfg
 setup.py
 test/test_app.py
+test/test_attribute_data_type.py
 test/test_attribute_schema.py
+test/test_attribute_schema_update.py
 test/test_backup_job.py
 test/test_backup_job_all_of.py
 test/test_backup_response.py
 test/test_backup_restore_request.py
 test/test_batch_operation.py
 test/test_batch_record_request.py
 test/test_batch_response.py
 test/test_build.py
+test/test_capabilities.py
+test/test_capabilities_api.py
 test/test_clone_job.py
 test/test_clone_job_all_of.py
 test/test_clone_response.py
 test/test_cloning_api.py
 test/test_commit.py
 test/test_component.py
 test/test_components.py
 test/test_db_component.py
 test/test_db_validationcomponent.py
 test/test_db_validationcomponent_details.py
 test/test_disk_space_component.py
 test/test_disk_space_component_details.py
 test/test_error_response.py
 test/test_general_wds_information_api.py
+test/test_generic_job.py
+test/test_generic_job_all_of.py
 test/test_git.py
+test/test_import_api.py
+test/test_import_request.py
 test/test_inline_object.py
 test/test_instances_api.py
 test/test_job.py
+test/test_job_api.py
+test/test_job_v1.py
 test/test_record_query_response.py
 test/test_record_request.py
 test/test_record_response.py
 test/test_record_type_schema.py
 test/test_records_api.py
-test/test_request_body_search.py
 test/test_schema_api.py
-test/test_search_operator.py
+test/test_search_filter.py
 test/test_search_request.py
 test/test_search_sort_direction.py
-test/test_snapshots_api.py
-test/test_stack_trace_element.py
 test/test_status_response.py
 test/test_tsv_upload_response.py
 test/test_version_response.py
 wds_client/__init__.py
 wds_client/api_client.py
 wds_client/configuration.py
 wds_client/exceptions.py
 wds_client/rest.py
 wds_client.egg-info/PKG-INFO
 wds_client.egg-info/SOURCES.txt
 wds_client.egg-info/dependency_links.txt
 wds_client.egg-info/requires.txt
 wds_client.egg-info/top_level.txt
 wds_client/api/__init__.py
+wds_client/api/capabilities_api.py
 wds_client/api/cloning_api.py
 wds_client/api/general_wds_information_api.py
+wds_client/api/import_api.py
 wds_client/api/instances_api.py
+wds_client/api/job_api.py
 wds_client/api/records_api.py
 wds_client/api/schema_api.py
-wds_client/api/snapshots_api.py
 wds_client/models/__init__.py
 wds_client/models/app.py
+wds_client/models/attribute_data_type.py
 wds_client/models/attribute_schema.py
+wds_client/models/attribute_schema_update.py
 wds_client/models/backup_job.py
 wds_client/models/backup_job_all_of.py
 wds_client/models/backup_response.py
 wds_client/models/backup_restore_request.py
 wds_client/models/batch_operation.py
 wds_client/models/batch_record_request.py
 wds_client/models/batch_response.py
 wds_client/models/build.py
+wds_client/models/capabilities.py
 wds_client/models/clone_job.py
 wds_client/models/clone_job_all_of.py
 wds_client/models/clone_response.py
 wds_client/models/commit.py
 wds_client/models/component.py
 wds_client/models/components.py
 wds_client/models/db_component.py
 wds_client/models/db_validationcomponent.py
 wds_client/models/db_validationcomponent_details.py
 wds_client/models/disk_space_component.py
 wds_client/models/disk_space_component_details.py
 wds_client/models/error_response.py
+wds_client/models/generic_job.py
+wds_client/models/generic_job_all_of.py
 wds_client/models/git.py
+wds_client/models/import_request.py
 wds_client/models/inline_object.py
 wds_client/models/job.py
+wds_client/models/job_v1.py
 wds_client/models/record_query_response.py
 wds_client/models/record_request.py
 wds_client/models/record_response.py
 wds_client/models/record_type_schema.py
-wds_client/models/request_body_search.py
-wds_client/models/search_operator.py
+wds_client/models/search_filter.py
 wds_client/models/search_request.py
 wds_client/models/search_sort_direction.py
-wds_client/models/stack_trace_element.py
 wds_client/models/status_response.py
 wds_client/models/tsv_upload_response.py
 wds_client/models/version_response.py
```

