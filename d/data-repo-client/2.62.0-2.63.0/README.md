# Comparing `tmp/data-repo-client-2.62.0.tar.gz` & `tmp/data-repo-client-2.63.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-fs7tqq0i/data-repo-client-2.62.0.tar", last modified: Wed May  8 18:17:17 2024, max compression
+gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-tkb2emxl/data-repo-client-2.63.0.tar", last modified: Mon May 13 15:48:23 2024, max compression
```

## Comparing `data-repo-client-2.62.0.tar` & `data-repo-client-2.63.0.tar`

### file list

```diff
@@ -1,388 +1,388 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    43869 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client/
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/configs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41290 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   225812 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22542 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/duos_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/journal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47273 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/register_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   470937 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/repository_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47274 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31737 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/snapshot_access_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   188090 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/add_auth_domain_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_double_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_int_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/enumerate_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/query_column_statistics_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/query_data_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_concepts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_response_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_criteria_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_feature_value_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_parent_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/sql_sort_direction_asc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/sql_sort_direction_desc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/tag_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/unlock_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_add_auth_domain_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_double_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_int_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_text_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_configs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_duos_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_enumerate_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_journal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_query_column_statistics_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_query_data_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_register_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_repository_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_access_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_access_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_concepts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_count_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_count_response_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_criteria_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_dataset_concept_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_domain_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_domain_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_domain_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_domain_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_feature_value_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_get_concept_hierarchy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_parent_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_sql_sort_direction_asc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_sql_sort_direction_desc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_tag_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_unlock_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_workspace_policy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    43869 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/data_repo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/data_repo_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41290 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/data_repository_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   225812 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22542 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/duos_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/journal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47273 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/profiles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/register_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   470937 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/repository_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47274 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31737 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/snapshot_access_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   188090 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/unauthenticated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api/upgrade_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/data_repo_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/access_info_big_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/access_info_big_query_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/access_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/access_info_parquet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/access_info_parquet_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/add_auth_domain_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/asset_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/billing_profile_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/billing_profile_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/bulk_load_array_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/bulk_load_array_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/bulk_load_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/bulk_load_file_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/bulk_load_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/bulk_load_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/bulk_load_history_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/bulk_load_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/bulk_load_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/column_statistics_double_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/column_statistics_double_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/column_statistics_int_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/column_statistics_int_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/column_statistics_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/column_statistics_text_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/column_statistics_text_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/config_enable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/config_fault_counted_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/config_fault_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/config_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/config_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/config_parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/data_deletion_gcs_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/data_deletion_json_array_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/data_deletion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/data_deletion_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/dataset_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/dataset_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/dataset_request_access_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/dataset_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/dataset_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/dataset_schema_column_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/dataset_schema_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/dataset_schema_update_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/dataset_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/dataset_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/date_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/delete_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/directory_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/drs_access_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/drs_access_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/drs_alias_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/drs_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/drs_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/drs_contents_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/drs_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/drs_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/drs_passport_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/drs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/duos_firecloud_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/duos_firecloud_groups_sync_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/enumerate_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/enumerate_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/enumerate_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/enumerate_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/enumerate_sort_by_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/file_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/file_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/file_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/iam_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/inaccessible_workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/ingest_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/ingest_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/int_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/journal_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/policy_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/query_column_statistics_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/query_data_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/relationship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/relationship_term_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/repository_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/repository_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/repository_status_model_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/resource_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/resource_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/sam_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_access_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_concepts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_count_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_count_response_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_criteria_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_domain_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_domain_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_feature_value_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_parent_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_list_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_range_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_ids_and_roles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_link_duos_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_preview_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_request_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_request_contents_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_request_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_request_row_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_request_row_id_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_retrieve_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/snapshot_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/sql_sort_direction_asc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/sql_sort_direction_desc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/storage_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/table_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/tag_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/tag_count_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/tag_update_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/transaction_close_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/transaction_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/transaction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/unlock_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/upgrade_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/upgrade_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/user_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/models/workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/data_repo_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/data_repo_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/data_repo_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/data_repo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/data_repo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/data_repo_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/data_repo_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:48:23.000000 data-repo-client-2.63.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_access_info_big_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_access_info_big_query_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_access_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_access_info_parquet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_access_info_parquet_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_add_auth_domain_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_asset_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_billing_profile_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_billing_profile_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_bulk_load_array_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_bulk_load_array_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_bulk_load_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_bulk_load_file_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_bulk_load_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_bulk_load_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_bulk_load_history_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_bulk_load_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_bulk_load_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_column_statistics_double_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_column_statistics_double_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_column_statistics_int_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_column_statistics_int_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_column_statistics_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_column_statistics_text_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_column_statistics_text_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_config_enable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_config_fault_counted_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_config_fault_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_config_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_config_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_config_parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_data_deletion_gcs_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_data_deletion_json_array_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_data_deletion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_data_deletion_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_data_repository_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_dataset_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_dataset_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_dataset_request_access_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_dataset_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_dataset_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_dataset_schema_column_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_dataset_schema_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_dataset_schema_update_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_dataset_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_dataset_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_date_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_delete_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_directory_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_drs_access_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_drs_access_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_drs_alias_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_drs_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_drs_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_drs_contents_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_drs_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_drs_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_drs_passport_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_drs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_duos_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_duos_firecloud_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_duos_firecloud_groups_sync_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_enumerate_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_enumerate_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_enumerate_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_enumerate_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_enumerate_sort_by_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_file_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_file_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_file_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_iam_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_inaccessible_workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_ingest_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_ingest_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_int_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_journal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_journal_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_policy_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_profiles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_query_column_statistics_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_query_data_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_register_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_relationship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_relationship_term_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_repository_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_repository_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_repository_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_repository_status_model_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_resource_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_resource_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_sam_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_access_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-13 15:48:16.000000 data-repo-client-2.63.0/test/test_snapshot_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_access_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_concepts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_count_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_count_response_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_criteria_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_dataset_concept_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_domain_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_domain_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_domain_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_domain_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_feature_value_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_get_concept_hierarchy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_parent_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_program_data_list_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_program_data_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_program_data_list_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_program_data_list_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_program_data_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_program_data_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_program_data_range_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_program_data_range_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_program_data_range_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_builder_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_export_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_export_response_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_export_response_model_format_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_export_response_model_format_parquet_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_export_response_model_format_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_ids_and_roles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_link_duos_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_preview_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_request_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_request_contents_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_request_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_request_row_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_request_row_id_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_retrieve_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshot_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_sql_sort_direction_asc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_sql_sort_direction_desc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_storage_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_table_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_tag_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_tag_count_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_tag_update_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_transaction_close_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_transaction_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_transaction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_unauthenticated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_unlock_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_upgrade_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_upgrade_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_upgrade_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_user_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-13 15:48:17.000000 data-repo-client-2.63.0/test/test_workspace_policy_model.py
```

### Comparing `data-repo-client-2.62.0/PKG-INFO` & `data-repo-client-2.63.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-repo-client
-Version: 2.62.0
+Version: 2.63.0
 Summary: Data Repository API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
```

### Comparing `data-repo-client-2.62.0/README.md` & `data-repo-client-2.63.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 2.62.0
+- Package version: 2.63.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `data-repo-client-2.62.0/data_repo_client/__init__.py` & `data-repo-client-2.63.0/data_repo_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.62.0"
+__version__ = "2.63.0"
 
 # import apis into sdk package
 from data_repo_client.api.data_repository_service_api import DataRepositoryServiceApi
 from data_repo_client.api.snapshot_access_request_api import SnapshotAccessRequestApi
 from data_repo_client.api.admin_api import AdminApi
 from data_repo_client.api.configs_api import ConfigsApi
 from data_repo_client.api.datasets_api import DatasetsApi
```

### Comparing `data-repo-client-2.62.0/data_repo_client/api/__init__.py` & `data-repo-client-2.63.0/data_repo_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/admin_api.py` & `data-repo-client-2.63.0/data_repo_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/configs_api.py` & `data-repo-client-2.63.0/data_repo_client/api/configs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/data_repository_service_api.py` & `data-repo-client-2.63.0/data_repo_client/api/data_repository_service_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/datasets_api.py` & `data-repo-client-2.63.0/data_repo_client/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/duos_api.py` & `data-repo-client-2.63.0/data_repo_client/api/duos_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/jobs_api.py` & `data-repo-client-2.63.0/data_repo_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/journal_api.py` & `data-repo-client-2.63.0/data_repo_client/api/journal_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/profiles_api.py` & `data-repo-client-2.63.0/data_repo_client/api/profiles_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/register_api.py` & `data-repo-client-2.63.0/data_repo_client/api/register_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/repository_api.py` & `data-repo-client-2.63.0/data_repo_client/api/repository_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/resources_api.py` & `data-repo-client-2.63.0/data_repo_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/search_api.py` & `data-repo-client-2.63.0/data_repo_client/api/search_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/snapshot_access_request_api.py` & `data-repo-client-2.63.0/data_repo_client/api/snapshot_access_request_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/snapshots_api.py` & `data-repo-client-2.63.0/data_repo_client/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/unauthenticated_api.py` & `data-repo-client-2.63.0/data_repo_client/api/unauthenticated_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api/upgrade_api.py` & `data-repo-client-2.63.0/data_repo_client/api/upgrade_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/api_client.py` & `data-repo-client-2.63.0/data_repo_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.62.0/python'
+        self.user_agent = 'OpenAPI-Generator/2.63.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `data-repo-client-2.62.0/data_repo_client/configuration.py` & `data-repo-client-2.63.0/data_repo_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 2.62.0".\
+               "SDK Package Version: 2.63.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `data-repo-client-2.62.0/data_repo_client/exceptions.py` & `data-repo-client-2.63.0/data_repo_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/__init__.py` & `data-repo-client-2.63.0/data_repo_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/access_info_big_query_model.py` & `data-repo-client-2.63.0/data_repo_client/models/access_info_big_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/access_info_big_query_model_table.py` & `data-repo-client-2.63.0/data_repo_client/models/access_info_big_query_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/access_info_model.py` & `data-repo-client-2.63.0/data_repo_client/models/access_info_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/access_info_parquet_model.py` & `data-repo-client-2.63.0/data_repo_client/models/access_info_parquet_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/access_info_parquet_model_table.py` & `data-repo-client-2.63.0/data_repo_client/models/access_info_parquet_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/add_auth_domain_response_model.py` & `data-repo-client-2.63.0/data_repo_client/models/add_auth_domain_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/asset_model.py` & `data-repo-client-2.63.0/data_repo_client/models/asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/asset_table_model.py` & `data-repo-client-2.63.0/data_repo_client/models/asset_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/billing_profile_model.py` & `data-repo-client-2.63.0/data_repo_client/models/billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/billing_profile_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/billing_profile_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/billing_profile_update_model.py` & `data-repo-client-2.63.0/data_repo_client/models/billing_profile_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/bulk_load_array_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/bulk_load_array_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/bulk_load_array_result_model.py` & `data-repo-client-2.63.0/data_repo_client/models/bulk_load_array_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_model.py` & `data-repo-client-2.63.0/data_repo_client/models/bulk_load_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_result_model.py` & `data-repo-client-2.63.0/data_repo_client/models/bulk_load_file_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_state.py` & `data-repo-client-2.63.0/data_repo_client/models/bulk_load_file_state.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/bulk_load_history_model.py` & `data-repo-client-2.63.0/data_repo_client/models/bulk_load_history_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/bulk_load_history_model_list.py` & `data-repo-client-2.63.0/data_repo_client/models/bulk_load_history_model_list.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/bulk_load_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/bulk_load_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/bulk_load_result_model.py` & `data-repo-client-2.63.0/data_repo_client/models/bulk_load_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/cloud_platform.py` & `data-repo-client-2.63.0/data_repo_client/models/cloud_platform.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/column_model.py` & `data-repo-client-2.63.0/data_repo_client/models/column_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/column_statistics_double_model.py` & `data-repo-client-2.63.0/data_repo_client/models/column_statistics_double_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/column_statistics_double_model_all_of.py` & `data-repo-client-2.63.0/data_repo_client/models/column_statistics_double_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/column_statistics_int_model.py` & `data-repo-client-2.63.0/data_repo_client/models/column_statistics_int_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/column_statistics_int_model_all_of.py` & `data-repo-client-2.63.0/data_repo_client/models/column_statistics_int_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/column_statistics_model.py` & `data-repo-client-2.63.0/data_repo_client/models/column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_model.py` & `data-repo-client-2.63.0/data_repo_client/models/column_statistics_text_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_model_all_of.py` & `data-repo-client-2.63.0/data_repo_client/models/column_statistics_text_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_value.py` & `data-repo-client-2.63.0/data_repo_client/models/column_statistics_text_value.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/config_enable_model.py` & `data-repo-client-2.63.0/data_repo_client/models/config_enable_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/config_fault_counted_model.py` & `data-repo-client-2.63.0/data_repo_client/models/config_fault_counted_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/config_fault_model.py` & `data-repo-client-2.63.0/data_repo_client/models/config_fault_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/config_group_model.py` & `data-repo-client-2.63.0/data_repo_client/models/config_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/config_list_model.py` & `data-repo-client-2.63.0/data_repo_client/models/config_list_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/config_model.py` & `data-repo-client-2.63.0/data_repo_client/models/config_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/config_parameter_model.py` & `data-repo-client-2.63.0/data_repo_client/models/config_parameter_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/data_deletion_gcs_file_model.py` & `data-repo-client-2.63.0/data_repo_client/models/data_deletion_gcs_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/data_deletion_json_array_model.py` & `data-repo-client-2.63.0/data_repo_client/models/data_deletion_json_array_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/data_deletion_request.py` & `data-repo-client-2.63.0/data_repo_client/models/data_deletion_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/data_deletion_table_model.py` & `data-repo-client-2.63.0/data_repo_client/models/data_deletion_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/dataset_data_model.py` & `data-repo-client-2.63.0/data_repo_client/models/dataset_data_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/dataset_model.py` & `data-repo-client-2.63.0/data_repo_client/models/dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/dataset_patch_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/dataset_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/dataset_request_access_include_model.py` & `data-repo-client-2.63.0/data_repo_client/models/dataset_request_access_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/dataset_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/dataset_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/dataset_request_model_policies.py` & `data-repo-client-2.63.0/data_repo_client/models/dataset_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/dataset_schema_column_update_model.py` & `data-repo-client-2.63.0/data_repo_client/models/dataset_schema_column_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/dataset_schema_update_model.py` & `data-repo-client-2.63.0/data_repo_client/models/dataset_schema_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/dataset_schema_update_model_changes.py` & `data-repo-client-2.63.0/data_repo_client/models/dataset_schema_update_model_changes.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/dataset_specification_model.py` & `data-repo-client-2.63.0/data_repo_client/models/dataset_specification_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/dataset_summary_model.py` & `data-repo-client-2.63.0/data_repo_client/models/dataset_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/date_partition_options_model.py` & `data-repo-client-2.63.0/data_repo_client/models/date_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/delete_response_model.py` & `data-repo-client-2.63.0/data_repo_client/models/delete_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/directory_detail_model.py` & `data-repo-client-2.63.0/data_repo_client/models/directory_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/drs_access_method.py` & `data-repo-client-2.63.0/data_repo_client/models/drs_access_method.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/drs_access_url.py` & `data-repo-client-2.63.0/data_repo_client/models/drs_access_url.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/drs_alias_model.py` & `data-repo-client-2.63.0/data_repo_client/models/drs_alias_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/drs_authorizations.py` & `data-repo-client-2.63.0/data_repo_client/models/drs_authorizations.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/drs_checksum.py` & `data-repo-client-2.63.0/data_repo_client/models/drs_checksum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/drs_contents_object.py` & `data-repo-client-2.63.0/data_repo_client/models/drs_contents_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/drs_error.py` & `data-repo-client-2.63.0/data_repo_client/models/drs_error.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/drs_object.py` & `data-repo-client-2.63.0/data_repo_client/models/drs_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/drs_passport_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/drs_passport_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/drs_service_info.py` & `data-repo-client-2.63.0/data_repo_client/models/drs_service_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/duos_firecloud_group_model.py` & `data-repo-client-2.63.0/data_repo_client/models/duos_firecloud_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/duos_firecloud_groups_sync_response.py` & `data-repo-client-2.63.0/data_repo_client/models/duos_firecloud_groups_sync_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/enumerate_billing_profile_model.py` & `data-repo-client-2.63.0/data_repo_client/models/enumerate_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/enumerate_dataset_model.py` & `data-repo-client-2.63.0/data_repo_client/models/enumerate_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/enumerate_snapshot_access_request.py` & `data-repo-client-2.63.0/data_repo_client/models/enumerate_snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/enumerate_snapshot_model.py` & `data-repo-client-2.63.0/data_repo_client/models/enumerate_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/enumerate_sort_by_param.py` & `data-repo-client-2.63.0/data_repo_client/models/enumerate_sort_by_param.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/error_model.py` & `data-repo-client-2.63.0/data_repo_client/models/error_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/file_detail_model.py` & `data-repo-client-2.63.0/data_repo_client/models/file_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/file_load_model.py` & `data-repo-client-2.63.0/data_repo_client/models/file_load_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/file_model.py` & `data-repo-client-2.63.0/data_repo_client/models/file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/file_model_type.py` & `data-repo-client-2.63.0/data_repo_client/models/file_model_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/iam_resource_type_enum.py` & `data-repo-client-2.63.0/data_repo_client/models/iam_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/inaccessible_workspace_policy_model.py` & `data-repo-client-2.63.0/data_repo_client/models/inaccessible_workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/ingest_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/ingest_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/ingest_response_model.py` & `data-repo-client-2.63.0/data_repo_client/models/ingest_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/int_partition_options_model.py` & `data-repo-client-2.63.0/data_repo_client/models/int_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/job_model.py` & `data-repo-client-2.63.0/data_repo_client/models/job_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/journal_entry_model.py` & `data-repo-client-2.63.0/data_repo_client/models/journal_entry_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/policy_member_request.py` & `data-repo-client-2.63.0/data_repo_client/models/policy_member_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/policy_model.py` & `data-repo-client-2.63.0/data_repo_client/models/policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/policy_response.py` & `data-repo-client-2.63.0/data_repo_client/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/query_column_statistics_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/query_column_statistics_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/query_data_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/query_data_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/relationship_model.py` & `data-repo-client-2.63.0/data_repo_client/models/relationship_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/relationship_term_model.py` & `data-repo-client-2.63.0/data_repo_client/models/relationship_term_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/repository_configuration_model.py` & `data-repo-client-2.63.0/data_repo_client/models/repository_configuration_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/repository_status_model.py` & `data-repo-client-2.63.0/data_repo_client/models/repository_status_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/repository_status_model_systems.py` & `data-repo-client-2.63.0/data_repo_client/models/repository_status_model_systems.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/resource_locks.py` & `data-repo-client-2.63.0/data_repo_client/models/resource_locks.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/resource_policy_model.py` & `data-repo-client-2.63.0/data_repo_client/models/resource_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/sam_policy_model.py` & `data-repo-client-2.63.0/data_repo_client/models/sam_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request_response.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_access_request_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request_status.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_access_request_status.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_cohort.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_cohort.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,16 +50,15 @@
 
         self._name = None
         self._criteria_groups = None
         self.discriminator = None
 
         if name is not None:
             self.name = name
-        if criteria_groups is not None:
-            self.criteria_groups = criteria_groups
+        self.criteria_groups = criteria_groups
 
     @property
     def name(self):
         """Gets the name of this SnapshotBuilderCohort.  # noqa: E501
 
 
         :return: The name of this SnapshotBuilderCohort.  # noqa: E501
@@ -92,14 +91,16 @@
     def criteria_groups(self, criteria_groups):
         """Sets the criteria_groups of this SnapshotBuilderCohort.
 
 
         :param criteria_groups: The criteria_groups of this SnapshotBuilderCohort.  # noqa: E501
         :type: list[SnapshotBuilderCriteriaGroup]
         """
+        if self.local_vars_configuration.client_side_validation and criteria_groups is None:  # noqa: E501
+            raise ValueError("Invalid value for `criteria_groups`, must not be `None`")  # noqa: E501
 
         self._criteria_groups = criteria_groups
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_concept.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_concepts_response.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_concepts_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_request.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_count_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_response.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_count_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_response_result.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_count_response_result.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_criteria.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_criteria_group.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_criteria_group.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,49 +32,41 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'name': 'str',
         'criteria': 'list[SnapshotBuilderCriteria]',
         'must_meet': 'bool',
-        'meet_all': 'bool',
-        'count': 'float'
+        'meet_all': 'bool'
     }
 
     attribute_map = {
         'name': 'name',
         'criteria': 'criteria',
         'must_meet': 'mustMeet',
-        'meet_all': 'meetAll',
-        'count': 'count'
+        'meet_all': 'meetAll'
     }
 
-    def __init__(self, name=None, criteria=None, must_meet=None, meet_all=None, count=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, criteria=None, must_meet=None, meet_all=None, local_vars_configuration=None):  # noqa: E501
         """SnapshotBuilderCriteriaGroup - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._criteria = None
         self._must_meet = None
         self._meet_all = None
-        self._count = None
         self.discriminator = None
 
         if name is not None:
             self.name = name
-        if criteria is not None:
-            self.criteria = criteria
-        if must_meet is not None:
-            self.must_meet = must_meet
-        if meet_all is not None:
-            self.meet_all = meet_all
-        if count is not None:
-            self.count = count
+        self.criteria = criteria
+        self.must_meet = must_meet
+        self.meet_all = meet_all
 
     @property
     def name(self):
         """Gets the name of this SnapshotBuilderCriteriaGroup.  # noqa: E501
 
 
         :return: The name of this SnapshotBuilderCriteriaGroup.  # noqa: E501
@@ -107,14 +99,16 @@
     def criteria(self, criteria):
         """Sets the criteria of this SnapshotBuilderCriteriaGroup.
 
 
         :param criteria: The criteria of this SnapshotBuilderCriteriaGroup.  # noqa: E501
         :type: list[SnapshotBuilderCriteria]
         """
+        if self.local_vars_configuration.client_side_validation and criteria is None:  # noqa: E501
+            raise ValueError("Invalid value for `criteria`, must not be `None`")  # noqa: E501
 
         self._criteria = criteria
 
     @property
     def must_meet(self):
         """Gets the must_meet of this SnapshotBuilderCriteriaGroup.  # noqa: E501
 
@@ -128,14 +122,16 @@
     def must_meet(self, must_meet):
         """Sets the must_meet of this SnapshotBuilderCriteriaGroup.
 
 
         :param must_meet: The must_meet of this SnapshotBuilderCriteriaGroup.  # noqa: E501
         :type: bool
         """
+        if self.local_vars_configuration.client_side_validation and must_meet is None:  # noqa: E501
+            raise ValueError("Invalid value for `must_meet`, must not be `None`")  # noqa: E501
 
         self._must_meet = must_meet
 
     @property
     def meet_all(self):
         """Gets the meet_all of this SnapshotBuilderCriteriaGroup.  # noqa: E501
 
@@ -149,38 +145,19 @@
     def meet_all(self, meet_all):
         """Sets the meet_all of this SnapshotBuilderCriteriaGroup.
 
 
         :param meet_all: The meet_all of this SnapshotBuilderCriteriaGroup.  # noqa: E501
         :type: bool
         """
+        if self.local_vars_configuration.client_side_validation and meet_all is None:  # noqa: E501
+            raise ValueError("Invalid value for `meet_all`, must not be `None`")  # noqa: E501
 
         self._meet_all = meet_all
 
-    @property
-    def count(self):
-        """Gets the count of this SnapshotBuilderCriteriaGroup.  # noqa: E501
-
-
-        :return: The count of this SnapshotBuilderCriteriaGroup.  # noqa: E501
-        :rtype: float
-        """
-        return self._count
-
-    @count.setter
-    def count(self, count):
-        """Sets the count of this SnapshotBuilderCriteriaGroup.
-
-
-        :param count: The count of this SnapshotBuilderCriteriaGroup.  # noqa: E501
-        :type: float
-        """
-
-        self._count = count
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_criteria.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_domain_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_option.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_domain_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_feature_value_group.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_feature_value_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_option.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_parent_concept.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_parent_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_item.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_list_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_option.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_list_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_option.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_option.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_range_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_request.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_settings.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_builder_settings.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model_format.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_ids_and_roles_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_ids_and_roles_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_link_duos_dataset_response.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_link_duos_dataset_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_patch_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_preview_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_preview_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_asset_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_request_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_contents_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_request_contents_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_model_policies.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_query_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_request_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_row_id_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_request_row_id_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_row_id_table_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_request_row_id_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_retrieve_include_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_retrieve_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_source_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_source_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/snapshot_summary_model.py` & `data-repo-client-2.63.0/data_repo_client/models/snapshot_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/sql_sort_direction_asc_default.py` & `data-repo-client-2.63.0/data_repo_client/models/sql_sort_direction_asc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/sql_sort_direction_desc_default.py` & `data-repo-client-2.63.0/data_repo_client/models/sql_sort_direction_desc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/storage_resource_model.py` & `data-repo-client-2.63.0/data_repo_client/models/storage_resource_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/table_data_type.py` & `data-repo-client-2.63.0/data_repo_client/models/table_data_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/table_model.py` & `data-repo-client-2.63.0/data_repo_client/models/table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/tag_count.py` & `data-repo-client-2.63.0/data_repo_client/models/tag_count.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/tag_count_result_model.py` & `data-repo-client-2.63.0/data_repo_client/models/tag_count_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/tag_update_request_model.py` & `data-repo-client-2.63.0/data_repo_client/models/tag_update_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/transaction_close_model.py` & `data-repo-client-2.63.0/data_repo_client/models/transaction_close_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/transaction_create_model.py` & `data-repo-client-2.63.0/data_repo_client/models/transaction_create_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/transaction_model.py` & `data-repo-client-2.63.0/data_repo_client/models/transaction_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/unlock_resource_request.py` & `data-repo-client-2.63.0/data_repo_client/models/unlock_resource_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/upgrade_model.py` & `data-repo-client-2.63.0/data_repo_client/models/upgrade_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/upgrade_response_model.py` & `data-repo-client-2.63.0/data_repo_client/models/upgrade_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/user_status_info.py` & `data-repo-client-2.63.0/data_repo_client/models/user_status_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/models/workspace_policy_model.py` & `data-repo-client-2.63.0/data_repo_client/models/workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client/rest.py` & `data-repo-client-2.63.0/data_repo_client/rest.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/data_repo_client.egg-info/PKG-INFO` & `data-repo-client-2.63.0/data_repo_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-repo-client
-Version: 2.62.0
+Version: 2.63.0
 Summary: Data Repository API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
```

### Comparing `data-repo-client-2.62.0/data_repo_client.egg-info/SOURCES.txt` & `data-repo-client-2.63.0/data_repo_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/setup.py` & `data-repo-client-2.63.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "data-repo-client"
-VERSION = "2.62.0"
+VERSION = "2.63.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `data-repo-client-2.62.0/test/test_access_info_big_query_model.py` & `data-repo-client-2.63.0/test/test_access_info_big_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_access_info_big_query_model_table.py` & `data-repo-client-2.63.0/test/test_access_info_big_query_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_access_info_model.py` & `data-repo-client-2.63.0/test/test_access_info_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_access_info_parquet_model.py` & `data-repo-client-2.63.0/test/test_access_info_parquet_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_access_info_parquet_model_table.py` & `data-repo-client-2.63.0/test/test_access_info_parquet_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_add_auth_domain_response_model.py` & `data-repo-client-2.63.0/test/test_add_auth_domain_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_admin_api.py` & `data-repo-client-2.63.0/test/test_admin_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_asset_model.py` & `data-repo-client-2.63.0/test/test_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_asset_table_model.py` & `data-repo-client-2.63.0/test/test_asset_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_billing_profile_model.py` & `data-repo-client-2.63.0/test/test_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_billing_profile_request_model.py` & `data-repo-client-2.63.0/test/test_billing_profile_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_billing_profile_update_model.py` & `data-repo-client-2.63.0/test/test_billing_profile_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_bulk_load_array_request_model.py` & `data-repo-client-2.63.0/test/test_bulk_load_array_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_bulk_load_array_result_model.py` & `data-repo-client-2.63.0/test/test_bulk_load_array_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_bulk_load_file_model.py` & `data-repo-client-2.63.0/test/test_bulk_load_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_bulk_load_file_result_model.py` & `data-repo-client-2.63.0/test/test_bulk_load_file_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_bulk_load_file_state.py` & `data-repo-client-2.63.0/test/test_bulk_load_file_state.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_bulk_load_history_model.py` & `data-repo-client-2.63.0/test/test_bulk_load_history_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_bulk_load_history_model_list.py` & `data-repo-client-2.63.0/test/test_bulk_load_history_model_list.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_bulk_load_request_model.py` & `data-repo-client-2.63.0/test/test_bulk_load_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_bulk_load_result_model.py` & `data-repo-client-2.63.0/test/test_bulk_load_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_cloud_platform.py` & `data-repo-client-2.63.0/test/test_cloud_platform.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_column_model.py` & `data-repo-client-2.63.0/test/test_column_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_column_statistics_double_model.py` & `data-repo-client-2.63.0/test/test_column_statistics_double_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_column_statistics_double_model_all_of.py` & `data-repo-client-2.63.0/test/test_column_statistics_double_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_column_statistics_int_model.py` & `data-repo-client-2.63.0/test/test_column_statistics_int_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_column_statistics_int_model_all_of.py` & `data-repo-client-2.63.0/test/test_column_statistics_int_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_column_statistics_model.py` & `data-repo-client-2.63.0/test/test_column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_column_statistics_text_model.py` & `data-repo-client-2.63.0/test/test_column_statistics_text_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_column_statistics_text_model_all_of.py` & `data-repo-client-2.63.0/test/test_column_statistics_text_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_column_statistics_text_value.py` & `data-repo-client-2.63.0/test/test_column_statistics_text_value.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_config_enable_model.py` & `data-repo-client-2.63.0/test/test_config_enable_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_config_fault_counted_model.py` & `data-repo-client-2.63.0/test/test_config_fault_counted_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_config_fault_model.py` & `data-repo-client-2.63.0/test/test_config_fault_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_config_group_model.py` & `data-repo-client-2.63.0/test/test_config_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_config_list_model.py` & `data-repo-client-2.63.0/test/test_config_list_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_config_model.py` & `data-repo-client-2.63.0/test/test_config_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_config_parameter_model.py` & `data-repo-client-2.63.0/test/test_config_parameter_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_configs_api.py` & `data-repo-client-2.63.0/test/test_configs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_data_deletion_gcs_file_model.py` & `data-repo-client-2.63.0/test/test_data_deletion_gcs_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_data_deletion_json_array_model.py` & `data-repo-client-2.63.0/test/test_data_deletion_json_array_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_data_deletion_request.py` & `data-repo-client-2.63.0/test/test_data_deletion_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_data_deletion_table_model.py` & `data-repo-client-2.63.0/test/test_data_deletion_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_data_repository_service_api.py` & `data-repo-client-2.63.0/test/test_data_repository_service_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_dataset_data_model.py` & `data-repo-client-2.63.0/test/test_dataset_data_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_dataset_model.py` & `data-repo-client-2.63.0/test/test_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_dataset_patch_request_model.py` & `data-repo-client-2.63.0/test/test_dataset_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_dataset_request_access_include_model.py` & `data-repo-client-2.63.0/test/test_dataset_request_access_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_dataset_request_model.py` & `data-repo-client-2.63.0/test/test_dataset_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_dataset_request_model_policies.py` & `data-repo-client-2.63.0/test/test_dataset_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_dataset_schema_column_update_model.py` & `data-repo-client-2.63.0/test/test_dataset_schema_column_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_dataset_schema_update_model.py` & `data-repo-client-2.63.0/test/test_dataset_schema_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_dataset_schema_update_model_changes.py` & `data-repo-client-2.63.0/test/test_dataset_schema_update_model_changes.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_dataset_specification_model.py` & `data-repo-client-2.63.0/test/test_dataset_specification_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_dataset_summary_model.py` & `data-repo-client-2.63.0/test/test_dataset_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_datasets_api.py` & `data-repo-client-2.63.0/test/test_datasets_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_date_partition_options_model.py` & `data-repo-client-2.63.0/test/test_date_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_delete_response_model.py` & `data-repo-client-2.63.0/test/test_delete_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_directory_detail_model.py` & `data-repo-client-2.63.0/test/test_directory_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_drs_access_method.py` & `data-repo-client-2.63.0/test/test_drs_access_method.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_drs_access_url.py` & `data-repo-client-2.63.0/test/test_drs_access_url.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_drs_alias_model.py` & `data-repo-client-2.63.0/test/test_drs_alias_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_drs_authorizations.py` & `data-repo-client-2.63.0/test/test_drs_authorizations.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_drs_checksum.py` & `data-repo-client-2.63.0/test/test_drs_checksum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_drs_contents_object.py` & `data-repo-client-2.63.0/test/test_drs_contents_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_drs_error.py` & `data-repo-client-2.63.0/test/test_drs_error.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_drs_object.py` & `data-repo-client-2.63.0/test/test_drs_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_drs_passport_request_model.py` & `data-repo-client-2.63.0/test/test_drs_passport_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_drs_service_info.py` & `data-repo-client-2.63.0/test/test_drs_service_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_duos_api.py` & `data-repo-client-2.63.0/test/test_duos_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_duos_firecloud_group_model.py` & `data-repo-client-2.63.0/test/test_duos_firecloud_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_duos_firecloud_groups_sync_response.py` & `data-repo-client-2.63.0/test/test_duos_firecloud_groups_sync_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_enumerate_billing_profile_model.py` & `data-repo-client-2.63.0/test/test_enumerate_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_enumerate_dataset_model.py` & `data-repo-client-2.63.0/test/test_enumerate_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_enumerate_snapshot_access_request.py` & `data-repo-client-2.63.0/test/test_enumerate_snapshot_access_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,15 @@
                                             name = '0', 
                                             criteria = [
                                                 data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
                                                     kind = 'list', 
                                                     id = 56, )
                                                 ], 
                                             must_meet = True, 
-                                            meet_all = True, 
-                                            count = 1.337, )
+                                            meet_all = True, )
                                         ], )
                                 ], 
                             concept_sets = [
                                 data_repo_client.models.snapshot_builder_dataset_concept_set.SnapshotBuilderDatasetConceptSet(
                                     name = '0', 
                                     feature_value_group_name = '0', 
                                     concept = data_repo_client.models.snapshot_builder_concept.SnapshotBuilderConcept(
```

### Comparing `data-repo-client-2.62.0/test/test_enumerate_snapshot_model.py` & `data-repo-client-2.63.0/test/test_enumerate_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_enumerate_sort_by_param.py` & `data-repo-client-2.63.0/test/test_enumerate_sort_by_param.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_error_model.py` & `data-repo-client-2.63.0/test/test_error_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_file_detail_model.py` & `data-repo-client-2.63.0/test/test_file_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_file_load_model.py` & `data-repo-client-2.63.0/test/test_file_load_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_file_model.py` & `data-repo-client-2.63.0/test/test_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_file_model_type.py` & `data-repo-client-2.63.0/test/test_file_model_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_iam_resource_type_enum.py` & `data-repo-client-2.63.0/test/test_iam_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_inaccessible_workspace_policy_model.py` & `data-repo-client-2.63.0/test/test_inaccessible_workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_ingest_request_model.py` & `data-repo-client-2.63.0/test/test_ingest_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_ingest_response_model.py` & `data-repo-client-2.63.0/test/test_ingest_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_int_partition_options_model.py` & `data-repo-client-2.63.0/test/test_int_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_job_model.py` & `data-repo-client-2.63.0/test/test_job_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_jobs_api.py` & `data-repo-client-2.63.0/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_journal_api.py` & `data-repo-client-2.63.0/test/test_journal_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_journal_entry_model.py` & `data-repo-client-2.63.0/test/test_journal_entry_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_policy_member_request.py` & `data-repo-client-2.63.0/test/test_policy_member_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_policy_model.py` & `data-repo-client-2.63.0/test/test_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_policy_response.py` & `data-repo-client-2.63.0/test/test_policy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_profiles_api.py` & `data-repo-client-2.63.0/test/test_profiles_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_query_column_statistics_request_model.py` & `data-repo-client-2.63.0/test/test_query_column_statistics_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_query_data_request_model.py` & `data-repo-client-2.63.0/test/test_query_data_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_register_api.py` & `data-repo-client-2.63.0/test/test_register_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_relationship_model.py` & `data-repo-client-2.63.0/test/test_relationship_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_relationship_term_model.py` & `data-repo-client-2.63.0/test/test_relationship_term_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_repository_api.py` & `data-repo-client-2.63.0/test/test_repository_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_repository_configuration_model.py` & `data-repo-client-2.63.0/test/test_repository_configuration_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_repository_status_model.py` & `data-repo-client-2.63.0/test/test_repository_status_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_repository_status_model_systems.py` & `data-repo-client-2.63.0/test/test_repository_status_model_systems.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_resource_locks.py` & `data-repo-client-2.63.0/test/test_resource_locks.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_resource_policy_model.py` & `data-repo-client-2.63.0/test/test_resource_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_resources_api.py` & `data-repo-client-2.63.0/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_sam_policy_model.py` & `data-repo-client-2.63.0/test/test_sam_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_search_api.py` & `data-repo-client-2.63.0/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_access_request.py` & `data-repo-client-2.63.0/test/test_snapshot_access_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,15 @@
                                     name = '0', 
                                     criteria = [
                                         data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
                                             kind = 'list', 
                                             id = 56, )
                                         ], 
                                     must_meet = True, 
-                                    meet_all = True, 
-                                    count = 1.337, )
+                                    meet_all = True, )
                                 ], )
                         ], 
                     concept_sets = [
                         data_repo_client.models.snapshot_builder_dataset_concept_set.SnapshotBuilderDatasetConceptSet(
                             name = '0', 
                             feature_value_group_name = '0', 
                             concept = data_repo_client.models.snapshot_builder_concept.SnapshotBuilderConcept(
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_access_request_api.py` & `data-repo-client-2.63.0/test/test_snapshot_access_request_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_access_request_response.py` & `data-repo-client-2.63.0/test/test_snapshot_access_request_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,15 @@
                                     name = '0', 
                                     criteria = [
                                         data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
                                             kind = 'list', 
                                             id = 56, )
                                         ], 
                                     must_meet = True, 
-                                    meet_all = True, 
-                                    count = 1.337, )
+                                    meet_all = True, )
                                 ], )
                         ], 
                     concept_sets = [
                         data_repo_client.models.snapshot_builder_dataset_concept_set.SnapshotBuilderDatasetConceptSet(
                             name = '0', 
                             feature_value_group_name = '0', 
                             concept = data_repo_client.models.snapshot_builder_concept.SnapshotBuilderConcept(
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_access_request_status.py` & `data-repo-client-2.63.0/test/test_snapshot_access_request_status.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_cohort.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_count_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,53 +12,55 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_builder_cohort import SnapshotBuilderCohort  # noqa: E501
+from data_repo_client.models.snapshot_builder_count_request import SnapshotBuilderCountRequest  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotBuilderCohort(unittest.TestCase):
-    """SnapshotBuilderCohort unit test stubs"""
+class TestSnapshotBuilderCountRequest(unittest.TestCase):
+    """SnapshotBuilderCountRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotBuilderCohort
+        """Test SnapshotBuilderCountRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_builder_cohort.SnapshotBuilderCohort()  # noqa: E501
+        # model = data_repo_client.models.snapshot_builder_count_request.SnapshotBuilderCountRequest()  # noqa: E501
         if include_optional :
-            return SnapshotBuilderCohort(
-                name = '0', 
-                criteria_groups = [
-                    data_repo_client.models.snapshot_builder_criteria_group.SnapshotBuilderCriteriaGroup(
+            return SnapshotBuilderCountRequest(
+                cohorts = [
+                    data_repo_client.models.snapshot_builder_cohort.SnapshotBuilderCohort(
                         name = '0', 
-                        criteria = [
-                            data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
-                                kind = 'list', 
-                                id = 56, )
-                            ], 
-                        must_meet = True, 
-                        meet_all = True, 
-                        count = 1.337, )
+                        criteria_groups = [
+                            data_repo_client.models.snapshot_builder_criteria_group.SnapshotBuilderCriteriaGroup(
+                                name = '0', 
+                                criteria = [
+                                    data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
+                                        kind = 'list', 
+                                        id = 56, )
+                                    ], 
+                                must_meet = True, 
+                                meet_all = True, )
+                            ], )
                     ]
             )
         else :
-            return SnapshotBuilderCohort(
+            return SnapshotBuilderCountRequest(
         )
 
-    def testSnapshotBuilderCohort(self):
-        """Test SnapshotBuilderCohort"""
+    def testSnapshotBuilderCountRequest(self):
+        """Test SnapshotBuilderCountRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_concept.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_concepts_response.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_concepts_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_count_request.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_cohort.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,56 +12,63 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_builder_count_request import SnapshotBuilderCountRequest  # noqa: E501
+from data_repo_client.models.snapshot_builder_cohort import SnapshotBuilderCohort  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotBuilderCountRequest(unittest.TestCase):
-    """SnapshotBuilderCountRequest unit test stubs"""
+class TestSnapshotBuilderCohort(unittest.TestCase):
+    """SnapshotBuilderCohort unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotBuilderCountRequest
+        """Test SnapshotBuilderCohort
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_builder_count_request.SnapshotBuilderCountRequest()  # noqa: E501
+        # model = data_repo_client.models.snapshot_builder_cohort.SnapshotBuilderCohort()  # noqa: E501
         if include_optional :
-            return SnapshotBuilderCountRequest(
-                cohorts = [
-                    data_repo_client.models.snapshot_builder_cohort.SnapshotBuilderCohort(
+            return SnapshotBuilderCohort(
+                name = '0', 
+                criteria_groups = [
+                    data_repo_client.models.snapshot_builder_criteria_group.SnapshotBuilderCriteriaGroup(
                         name = '0', 
-                        criteria_groups = [
-                            data_repo_client.models.snapshot_builder_criteria_group.SnapshotBuilderCriteriaGroup(
-                                name = '0', 
-                                criteria = [
-                                    data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
-                                        kind = 'list', 
-                                        id = 56, )
-                                    ], 
-                                must_meet = True, 
-                                meet_all = True, 
-                                count = 1.337, )
-                            ], )
+                        criteria = [
+                            data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
+                                kind = 'list', 
+                                id = 56, )
+                            ], 
+                        must_meet = True, 
+                        meet_all = True, )
                     ]
             )
         else :
-            return SnapshotBuilderCountRequest(
+            return SnapshotBuilderCohort(
+                criteria_groups = [
+                    data_repo_client.models.snapshot_builder_criteria_group.SnapshotBuilderCriteriaGroup(
+                        name = '0', 
+                        criteria = [
+                            data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
+                                kind = 'list', 
+                                id = 56, )
+                            ], 
+                        must_meet = True, 
+                        meet_all = True, )
+                    ],
         )
 
-    def testSnapshotBuilderCountRequest(self):
-        """Test SnapshotBuilderCountRequest"""
+    def testSnapshotBuilderCohort(self):
+        """Test SnapshotBuilderCohort"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_count_response.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_count_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_count_response_result.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_count_response_result.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_criteria.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_criteria_group.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_domain_criteria.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,49 +12,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_builder_criteria_group import SnapshotBuilderCriteriaGroup  # noqa: E501
+from data_repo_client.models.snapshot_builder_domain_criteria import SnapshotBuilderDomainCriteria  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotBuilderCriteriaGroup(unittest.TestCase):
-    """SnapshotBuilderCriteriaGroup unit test stubs"""
+class TestSnapshotBuilderDomainCriteria(unittest.TestCase):
+    """SnapshotBuilderDomainCriteria unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotBuilderCriteriaGroup
+        """Test SnapshotBuilderDomainCriteria
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_builder_criteria_group.SnapshotBuilderCriteriaGroup()  # noqa: E501
+        # model = data_repo_client.models.snapshot_builder_domain_criteria.SnapshotBuilderDomainCriteria()  # noqa: E501
         if include_optional :
-            return SnapshotBuilderCriteriaGroup(
-                name = '0', 
-                criteria = [
-                    data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
-                        kind = 'list', 
-                        id = 56, )
-                    ], 
-                must_meet = True, 
-                meet_all = True, 
-                count = 1.337
+            return SnapshotBuilderDomainCriteria(
+                concept_id = 56
             )
         else :
-            return SnapshotBuilderCriteriaGroup(
+            return SnapshotBuilderDomainCriteria(
+                concept_id = 56,
         )
 
-    def testSnapshotBuilderCriteriaGroup(self):
-        """Test SnapshotBuilderCriteriaGroup"""
+    def testSnapshotBuilderDomainCriteria(self):
+        """Test SnapshotBuilderDomainCriteria"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_dataset_concept_set.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_dataset_concept_set.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_domain_criteria.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_domain_criteria_all_of.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,42 +12,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_builder_domain_criteria import SnapshotBuilderDomainCriteria  # noqa: E501
+from data_repo_client.models.snapshot_builder_domain_criteria_all_of import SnapshotBuilderDomainCriteriaAllOf  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotBuilderDomainCriteria(unittest.TestCase):
-    """SnapshotBuilderDomainCriteria unit test stubs"""
+class TestSnapshotBuilderDomainCriteriaAllOf(unittest.TestCase):
+    """SnapshotBuilderDomainCriteriaAllOf unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotBuilderDomainCriteria
+        """Test SnapshotBuilderDomainCriteriaAllOf
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_builder_domain_criteria.SnapshotBuilderDomainCriteria()  # noqa: E501
+        # model = data_repo_client.models.snapshot_builder_domain_criteria_all_of.SnapshotBuilderDomainCriteriaAllOf()  # noqa: E501
         if include_optional :
-            return SnapshotBuilderDomainCriteria(
+            return SnapshotBuilderDomainCriteriaAllOf(
                 concept_id = 56
             )
         else :
-            return SnapshotBuilderDomainCriteria(
+            return SnapshotBuilderDomainCriteriaAllOf(
                 concept_id = 56,
         )
 
-    def testSnapshotBuilderDomainCriteria(self):
-        """Test SnapshotBuilderDomainCriteria"""
+    def testSnapshotBuilderDomainCriteriaAllOf(self):
+        """Test SnapshotBuilderDomainCriteriaAllOf"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_domain_criteria_all_of.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_get_concept_hierarchy_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,42 +12,52 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_builder_domain_criteria_all_of import SnapshotBuilderDomainCriteriaAllOf  # noqa: E501
+from data_repo_client.models.snapshot_builder_get_concept_hierarchy_response import SnapshotBuilderGetConceptHierarchyResponse  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotBuilderDomainCriteriaAllOf(unittest.TestCase):
-    """SnapshotBuilderDomainCriteriaAllOf unit test stubs"""
+class TestSnapshotBuilderGetConceptHierarchyResponse(unittest.TestCase):
+    """SnapshotBuilderGetConceptHierarchyResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotBuilderDomainCriteriaAllOf
+        """Test SnapshotBuilderGetConceptHierarchyResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_builder_domain_criteria_all_of.SnapshotBuilderDomainCriteriaAllOf()  # noqa: E501
+        # model = data_repo_client.models.snapshot_builder_get_concept_hierarchy_response.SnapshotBuilderGetConceptHierarchyResponse()  # noqa: E501
         if include_optional :
-            return SnapshotBuilderDomainCriteriaAllOf(
-                concept_id = 56
+            return SnapshotBuilderGetConceptHierarchyResponse(
+                result = [
+                    data_repo_client.models.snapshot_builder_parent_concept.SnapshotBuilderParentConcept(
+                        parent_id = 56, 
+                        children = [
+                            data_repo_client.models.snapshot_builder_concept.SnapshotBuilderConcept(
+                                id = 56, 
+                                code = '0', 
+                                name = '0', 
+                                count = 56, 
+                                has_children = True, )
+                            ], )
+                    ]
             )
         else :
-            return SnapshotBuilderDomainCriteriaAllOf(
-                concept_id = 56,
+            return SnapshotBuilderGetConceptHierarchyResponse(
         )
 
-    def testSnapshotBuilderDomainCriteriaAllOf(self):
-        """Test SnapshotBuilderDomainCriteriaAllOf"""
+    def testSnapshotBuilderGetConceptHierarchyResponse(self):
+        """Test SnapshotBuilderGetConceptHierarchyResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_domain_option.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_domain_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_domain_option_all_of.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_domain_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_feature_value_group.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_feature_value_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_get_concept_hierarchy_response.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_parent_concept.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,52 +12,49 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_builder_get_concept_hierarchy_response import SnapshotBuilderGetConceptHierarchyResponse  # noqa: E501
+from data_repo_client.models.snapshot_builder_parent_concept import SnapshotBuilderParentConcept  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotBuilderGetConceptHierarchyResponse(unittest.TestCase):
-    """SnapshotBuilderGetConceptHierarchyResponse unit test stubs"""
+class TestSnapshotBuilderParentConcept(unittest.TestCase):
+    """SnapshotBuilderParentConcept unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotBuilderGetConceptHierarchyResponse
+        """Test SnapshotBuilderParentConcept
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_builder_get_concept_hierarchy_response.SnapshotBuilderGetConceptHierarchyResponse()  # noqa: E501
+        # model = data_repo_client.models.snapshot_builder_parent_concept.SnapshotBuilderParentConcept()  # noqa: E501
         if include_optional :
-            return SnapshotBuilderGetConceptHierarchyResponse(
-                result = [
-                    data_repo_client.models.snapshot_builder_parent_concept.SnapshotBuilderParentConcept(
-                        parent_id = 56, 
-                        children = [
-                            data_repo_client.models.snapshot_builder_concept.SnapshotBuilderConcept(
-                                id = 56, 
-                                code = '0', 
-                                name = '0', 
-                                count = 56, 
-                                has_children = True, )
-                            ], )
+            return SnapshotBuilderParentConcept(
+                parent_id = 56, 
+                children = [
+                    data_repo_client.models.snapshot_builder_concept.SnapshotBuilderConcept(
+                        id = 56, 
+                        code = '0', 
+                        name = '0', 
+                        count = 56, 
+                        has_children = True, )
                     ]
             )
         else :
-            return SnapshotBuilderGetConceptHierarchyResponse(
+            return SnapshotBuilderParentConcept(
         )
 
-    def testSnapshotBuilderGetConceptHierarchyResponse(self):
-        """Test SnapshotBuilderGetConceptHierarchyResponse"""
+    def testSnapshotBuilderParentConcept(self):
+        """Test SnapshotBuilderParentConcept"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_option.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_parent_concept.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_program_data_option.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,49 +12,41 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_builder_parent_concept import SnapshotBuilderParentConcept  # noqa: E501
+from data_repo_client.models.snapshot_builder_program_data_option import SnapshotBuilderProgramDataOption  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotBuilderParentConcept(unittest.TestCase):
-    """SnapshotBuilderParentConcept unit test stubs"""
+class TestSnapshotBuilderProgramDataOption(unittest.TestCase):
+    """SnapshotBuilderProgramDataOption unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotBuilderParentConcept
+        """Test SnapshotBuilderProgramDataOption
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_builder_parent_concept.SnapshotBuilderParentConcept()  # noqa: E501
+        # model = data_repo_client.models.snapshot_builder_program_data_option.SnapshotBuilderProgramDataOption()  # noqa: E501
         if include_optional :
-            return SnapshotBuilderParentConcept(
-                parent_id = 56, 
-                children = [
-                    data_repo_client.models.snapshot_builder_concept.SnapshotBuilderConcept(
-                        id = 56, 
-                        code = '0', 
-                        name = '0', 
-                        count = 56, 
-                        has_children = True, )
-                    ]
+            return SnapshotBuilderProgramDataOption(
+                kind = 'list'
             )
         else :
-            return SnapshotBuilderParentConcept(
+            return SnapshotBuilderProgramDataOption(
         )
 
-    def testSnapshotBuilderParentConcept(self):
-        """Test SnapshotBuilderParentConcept"""
+    def testSnapshotBuilderProgramDataOption(self):
+        """Test SnapshotBuilderProgramDataOption"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_criteria.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_program_data_list_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_item.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_program_data_list_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_option.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_program_data_list_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_option_all_of.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_program_data_list_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_option.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_program_data_option_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,41 +12,41 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_builder_program_data_option import SnapshotBuilderProgramDataOption  # noqa: E501
+from data_repo_client.models.snapshot_builder_program_data_option_all_of import SnapshotBuilderProgramDataOptionAllOf  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotBuilderProgramDataOption(unittest.TestCase):
-    """SnapshotBuilderProgramDataOption unit test stubs"""
+class TestSnapshotBuilderProgramDataOptionAllOf(unittest.TestCase):
+    """SnapshotBuilderProgramDataOptionAllOf unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotBuilderProgramDataOption
+        """Test SnapshotBuilderProgramDataOptionAllOf
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_builder_program_data_option.SnapshotBuilderProgramDataOption()  # noqa: E501
+        # model = data_repo_client.models.snapshot_builder_program_data_option_all_of.SnapshotBuilderProgramDataOptionAllOf()  # noqa: E501
         if include_optional :
-            return SnapshotBuilderProgramDataOption(
+            return SnapshotBuilderProgramDataOptionAllOf(
                 kind = 'list'
             )
         else :
-            return SnapshotBuilderProgramDataOption(
+            return SnapshotBuilderProgramDataOptionAllOf(
         )
 
-    def testSnapshotBuilderProgramDataOption(self):
-        """Test SnapshotBuilderProgramDataOption"""
+    def testSnapshotBuilderProgramDataOptionAllOf(self):
+        """Test SnapshotBuilderProgramDataOptionAllOf"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_option_all_of.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_program_data_range_option_all_of.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,41 +12,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_builder_program_data_option_all_of import SnapshotBuilderProgramDataOptionAllOf  # noqa: E501
+from data_repo_client.models.snapshot_builder_program_data_range_option_all_of import SnapshotBuilderProgramDataRangeOptionAllOf  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotBuilderProgramDataOptionAllOf(unittest.TestCase):
-    """SnapshotBuilderProgramDataOptionAllOf unit test stubs"""
+class TestSnapshotBuilderProgramDataRangeOptionAllOf(unittest.TestCase):
+    """SnapshotBuilderProgramDataRangeOptionAllOf unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotBuilderProgramDataOptionAllOf
+        """Test SnapshotBuilderProgramDataRangeOptionAllOf
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_builder_program_data_option_all_of.SnapshotBuilderProgramDataOptionAllOf()  # noqa: E501
+        # model = data_repo_client.models.snapshot_builder_program_data_range_option_all_of.SnapshotBuilderProgramDataRangeOptionAllOf()  # noqa: E501
         if include_optional :
-            return SnapshotBuilderProgramDataOptionAllOf(
-                kind = 'list'
+            return SnapshotBuilderProgramDataRangeOptionAllOf(
+                min = 56, 
+                max = 56
             )
         else :
-            return SnapshotBuilderProgramDataOptionAllOf(
+            return SnapshotBuilderProgramDataRangeOptionAllOf(
         )
 
-    def testSnapshotBuilderProgramDataOptionAllOf(self):
-        """Test SnapshotBuilderProgramDataOptionAllOf"""
+    def testSnapshotBuilderProgramDataRangeOptionAllOf(self):
+        """Test SnapshotBuilderProgramDataRangeOptionAllOf"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_criteria.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_program_data_range_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_option.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_program_data_range_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_option_all_of.py` & `data-repo-client-2.63.0/test/test_snapshot_request_model_policies.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,42 +12,49 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_builder_program_data_range_option_all_of import SnapshotBuilderProgramDataRangeOptionAllOf  # noqa: E501
+from data_repo_client.models.snapshot_request_model_policies import SnapshotRequestModelPolicies  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotBuilderProgramDataRangeOptionAllOf(unittest.TestCase):
-    """SnapshotBuilderProgramDataRangeOptionAllOf unit test stubs"""
+class TestSnapshotRequestModelPolicies(unittest.TestCase):
+    """SnapshotRequestModelPolicies unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotBuilderProgramDataRangeOptionAllOf
+        """Test SnapshotRequestModelPolicies
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_builder_program_data_range_option_all_of.SnapshotBuilderProgramDataRangeOptionAllOf()  # noqa: E501
+        # model = data_repo_client.models.snapshot_request_model_policies.SnapshotRequestModelPolicies()  # noqa: E501
         if include_optional :
-            return SnapshotBuilderProgramDataRangeOptionAllOf(
-                min = 56, 
-                max = 56
+            return SnapshotRequestModelPolicies(
+                stewards = [
+                    '0'
+                    ], 
+                readers = [
+                    '0'
+                    ], 
+                discoverers = [
+                    '0'
+                    ]
             )
         else :
-            return SnapshotBuilderProgramDataRangeOptionAllOf(
+            return SnapshotRequestModelPolicies(
         )
 
-    def testSnapshotBuilderProgramDataRangeOptionAllOf(self):
-        """Test SnapshotBuilderProgramDataRangeOptionAllOf"""
+    def testSnapshotRequestModelPolicies(self):
+        """Test SnapshotRequestModelPolicies"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_request.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,15 @@
                                 name = '0', 
                                 criteria = [
                                     data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
                                         kind = 'list', 
                                         id = 56, )
                                     ], 
                                 must_meet = True, 
-                                meet_all = True, 
-                                count = 1.337, )
+                                meet_all = True, )
                             ], )
                     ], 
                 concept_sets = [
                     data_repo_client.models.snapshot_builder_dataset_concept_set.SnapshotBuilderDatasetConceptSet(
                         name = '0', 
                         feature_value_group_name = '0', 
                         concept = data_repo_client.models.snapshot_builder_concept.SnapshotBuilderConcept(
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_builder_settings.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_settings.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_export_response_model.py` & `data-repo-client-2.63.0/test/test_snapshot_export_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_export_response_model_format.py` & `data-repo-client-2.63.0/test/test_snapshot_export_response_model_format.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet.py` & `data-repo-client-2.63.0/test/test_snapshot_export_response_model_format_parquet.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet_location.py` & `data-repo-client-2.63.0/test/test_snapshot_export_response_model_format_parquet_location.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py` & `data-repo-client-2.63.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_workspace.py` & `data-repo-client-2.63.0/test/test_snapshot_export_response_model_format_workspace.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_ids_and_roles_model.py` & `data-repo-client-2.63.0/test/test_snapshot_ids_and_roles_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_link_duos_dataset_response.py` & `data-repo-client-2.63.0/test/test_snapshot_link_duos_dataset_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_model.py` & `data-repo-client-2.63.0/test/test_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_patch_request_model.py` & `data-repo-client-2.63.0/test/test_snapshot_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_preview_model.py` & `data-repo-client-2.63.0/test/test_snapshot_preview_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_request_asset_model.py` & `data-repo-client-2.63.0/test/test_snapshot_request_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_request_contents_model.py` & `data-repo-client-2.63.0/test/test_snapshot_request_contents_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_request_model.py` & `data-repo-client-2.63.0/test/test_snapshot_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_request_model_policies.py` & `data-repo-client-2.63.0/test/test_snapshot_request_row_id_table_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,49 +12,54 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_request_model_policies import SnapshotRequestModelPolicies  # noqa: E501
+from data_repo_client.models.snapshot_request_row_id_table_model import SnapshotRequestRowIdTableModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotRequestModelPolicies(unittest.TestCase):
-    """SnapshotRequestModelPolicies unit test stubs"""
+class TestSnapshotRequestRowIdTableModel(unittest.TestCase):
+    """SnapshotRequestRowIdTableModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotRequestModelPolicies
+        """Test SnapshotRequestRowIdTableModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_request_model_policies.SnapshotRequestModelPolicies()  # noqa: E501
+        # model = data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel()  # noqa: E501
         if include_optional :
-            return SnapshotRequestModelPolicies(
-                stewards = [
-                    '0'
-                    ], 
-                readers = [
-                    '0'
+            return SnapshotRequestRowIdTableModel(
+                table_name = 'a', 
+                columns = [
+                    'a'
                     ], 
-                discoverers = [
+                row_ids = [
                     '0'
                     ]
             )
         else :
-            return SnapshotRequestModelPolicies(
+            return SnapshotRequestRowIdTableModel(
+                table_name = 'a',
+                columns = [
+                    'a'
+                    ],
+                row_ids = [
+                    '0'
+                    ],
         )
 
-    def testSnapshotRequestModelPolicies(self):
-        """Test SnapshotRequestModelPolicies"""
+    def testSnapshotRequestRowIdTableModel(self):
+        """Test SnapshotRequestRowIdTableModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_request_query_model.py` & `data-repo-client-2.63.0/test/test_snapshot_request_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_request_row_id_model.py` & `data-repo-client-2.63.0/test/test_snapshot_request_row_id_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_request_row_id_table_model.py` & `data-repo-client-2.63.0/test/test_transaction_create_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,54 +12,41 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_request_row_id_table_model import SnapshotRequestRowIdTableModel  # noqa: E501
+from data_repo_client.models.transaction_create_model import TransactionCreateModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotRequestRowIdTableModel(unittest.TestCase):
-    """SnapshotRequestRowIdTableModel unit test stubs"""
+class TestTransactionCreateModel(unittest.TestCase):
+    """TransactionCreateModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotRequestRowIdTableModel
+        """Test TransactionCreateModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel()  # noqa: E501
+        # model = data_repo_client.models.transaction_create_model.TransactionCreateModel()  # noqa: E501
         if include_optional :
-            return SnapshotRequestRowIdTableModel(
-                table_name = 'a', 
-                columns = [
-                    'a'
-                    ], 
-                row_ids = [
-                    '0'
-                    ]
+            return TransactionCreateModel(
+                description = '0'
             )
         else :
-            return SnapshotRequestRowIdTableModel(
-                table_name = 'a',
-                columns = [
-                    'a'
-                    ],
-                row_ids = [
-                    '0'
-                    ],
+            return TransactionCreateModel(
         )
 
-    def testSnapshotRequestRowIdTableModel(self):
-        """Test SnapshotRequestRowIdTableModel"""
+    def testTransactionCreateModel(self):
+        """Test TransactionCreateModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_snapshot_retrieve_include_model.py` & `data-repo-client-2.63.0/test/test_snapshot_retrieve_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_source_model.py` & `data-repo-client-2.63.0/test/test_snapshot_source_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshot_summary_model.py` & `data-repo-client-2.63.0/test/test_snapshot_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_snapshots_api.py` & `data-repo-client-2.63.0/test/test_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_sql_sort_direction_asc_default.py` & `data-repo-client-2.63.0/test/test_sql_sort_direction_asc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_sql_sort_direction_desc_default.py` & `data-repo-client-2.63.0/test/test_sql_sort_direction_desc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_storage_resource_model.py` & `data-repo-client-2.63.0/test/test_storage_resource_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_table_data_type.py` & `data-repo-client-2.63.0/test/test_table_data_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_table_model.py` & `data-repo-client-2.63.0/test/test_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_tag_count.py` & `data-repo-client-2.63.0/test/test_tag_count.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_tag_count_result_model.py` & `data-repo-client-2.63.0/test/test_tag_count_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_tag_update_request_model.py` & `data-repo-client-2.63.0/test/test_tag_update_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_transaction_close_model.py` & `data-repo-client-2.63.0/test/test_transaction_close_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_transaction_create_model.py` & `data-repo-client-2.63.0/test/test_transaction_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,41 +12,51 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.transaction_create_model import TransactionCreateModel  # noqa: E501
+from data_repo_client.models.transaction_model import TransactionModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestTransactionCreateModel(unittest.TestCase):
-    """TransactionCreateModel unit test stubs"""
+class TestTransactionModel(unittest.TestCase):
+    """TransactionModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test TransactionCreateModel
+        """Test TransactionModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.transaction_create_model.TransactionCreateModel()  # noqa: E501
+        # model = data_repo_client.models.transaction_model.TransactionModel()  # noqa: E501
         if include_optional :
-            return TransactionCreateModel(
-                description = '0'
+            return TransactionModel(
+                id = '0', 
+                status = 'active', 
+                lock = '0', 
+                description = '0', 
+                created_at = '0', 
+                created_by = '0', 
+                terminated_at = '0', 
+                terminated_by = '0'
             )
         else :
-            return TransactionCreateModel(
+            return TransactionModel(
+                id = '0',
+                created_at = '0',
+                created_by = '0',
         )
 
-    def testTransactionCreateModel(self):
-        """Test TransactionCreateModel"""
+    def testTransactionModel(self):
+        """Test TransactionModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_transaction_model.py` & `data-repo-client-2.63.0/test/test_user_status_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,51 +12,46 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.transaction_model import TransactionModel  # noqa: E501
+from data_repo_client.models.user_status_info import UserStatusInfo  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestTransactionModel(unittest.TestCase):
-    """TransactionModel unit test stubs"""
+class TestUserStatusInfo(unittest.TestCase):
+    """UserStatusInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test TransactionModel
+        """Test UserStatusInfo
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.transaction_model.TransactionModel()  # noqa: E501
+        # model = data_repo_client.models.user_status_info.UserStatusInfo()  # noqa: E501
         if include_optional :
-            return TransactionModel(
-                id = '0', 
-                status = 'active', 
-                lock = '0', 
-                description = '0', 
-                created_at = '0', 
-                created_by = '0', 
-                terminated_at = '0', 
-                terminated_by = '0'
+            return UserStatusInfo(
+                user_subject_id = '0', 
+                user_email = '0', 
+                enabled = True
             )
         else :
-            return TransactionModel(
-                id = '0',
-                created_at = '0',
-                created_by = '0',
+            return UserStatusInfo(
+                user_subject_id = '0',
+                user_email = '0',
+                enabled = True,
         )
 
-    def testTransactionModel(self):
-        """Test TransactionModel"""
+    def testUserStatusInfo(self):
+        """Test UserStatusInfo"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_unauthenticated_api.py` & `data-repo-client-2.63.0/test/test_unauthenticated_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_unlock_resource_request.py` & `data-repo-client-2.63.0/test/test_unlock_resource_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_upgrade_api.py` & `data-repo-client-2.63.0/test/test_upgrade_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_upgrade_model.py` & `data-repo-client-2.63.0/test/test_upgrade_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_upgrade_response_model.py` & `data-repo-client-2.63.0/test/test_upgrade_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.62.0/test/test_user_status_info.py` & `data-repo-client-2.63.0/test/test_workspace_policy_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,46 +12,51 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.user_status_info import UserStatusInfo  # noqa: E501
+from data_repo_client.models.workspace_policy_model import WorkspacePolicyModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestUserStatusInfo(unittest.TestCase):
-    """UserStatusInfo unit test stubs"""
+class TestWorkspacePolicyModel(unittest.TestCase):
+    """WorkspacePolicyModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test UserStatusInfo
+        """Test WorkspacePolicyModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.user_status_info.UserStatusInfo()  # noqa: E501
+        # model = data_repo_client.models.workspace_policy_model.WorkspacePolicyModel()  # noqa: E501
         if include_optional :
-            return UserStatusInfo(
-                user_subject_id = '0', 
-                user_email = '0', 
-                enabled = True
+            return WorkspacePolicyModel(
+                workspace_id = '0', 
+                workspace_name = '0', 
+                workspace_namespace = '0', 
+                workspace_link = '0', 
+                workspace_policies = [
+                    data_repo_client.models.policy_model.PolicyModel(
+                        name = '0', 
+                        members = [
+                            '0'
+                            ], )
+                    ]
             )
         else :
-            return UserStatusInfo(
-                user_subject_id = '0',
-                user_email = '0',
-                enabled = True,
+            return WorkspacePolicyModel(
         )
 
-    def testUserStatusInfo(self):
-        """Test UserStatusInfo"""
+    def testWorkspacePolicyModel(self):
+        """Test WorkspacePolicyModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.62.0/test/test_workspace_policy_model.py` & `data-repo-client-2.63.0/test/test_snapshot_builder_criteria_group.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,51 +12,55 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.workspace_policy_model import WorkspacePolicyModel  # noqa: E501
+from data_repo_client.models.snapshot_builder_criteria_group import SnapshotBuilderCriteriaGroup  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestWorkspacePolicyModel(unittest.TestCase):
-    """WorkspacePolicyModel unit test stubs"""
+class TestSnapshotBuilderCriteriaGroup(unittest.TestCase):
+    """SnapshotBuilderCriteriaGroup unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test WorkspacePolicyModel
+        """Test SnapshotBuilderCriteriaGroup
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.workspace_policy_model.WorkspacePolicyModel()  # noqa: E501
+        # model = data_repo_client.models.snapshot_builder_criteria_group.SnapshotBuilderCriteriaGroup()  # noqa: E501
         if include_optional :
-            return WorkspacePolicyModel(
-                workspace_id = '0', 
-                workspace_name = '0', 
-                workspace_namespace = '0', 
-                workspace_link = '0', 
-                workspace_policies = [
-                    data_repo_client.models.policy_model.PolicyModel(
-                        name = '0', 
-                        members = [
-                            '0'
-                            ], )
-                    ]
+            return SnapshotBuilderCriteriaGroup(
+                name = '0', 
+                criteria = [
+                    data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
+                        kind = 'list', 
+                        id = 56, )
+                    ], 
+                must_meet = True, 
+                meet_all = True
             )
         else :
-            return WorkspacePolicyModel(
+            return SnapshotBuilderCriteriaGroup(
+                criteria = [
+                    data_repo_client.models.snapshot_builder_criteria.SnapshotBuilderCriteria(
+                        kind = 'list', 
+                        id = 56, )
+                    ],
+                must_meet = True,
+                meet_all = True,
         )
 
-    def testWorkspacePolicyModel(self):
-        """Test WorkspacePolicyModel"""
+    def testSnapshotBuilderCriteriaGroup(self):
+        """Test SnapshotBuilderCriteriaGroup"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

