# Comparing `tmp/kio-0.0.0a3.tar.gz` & `tmp/kio-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kio-0.0.0a3.tar", last modified: Tue Feb 13 09:44:34 2024, max compression
+gzip compressed data, was "kio-0.1.0.tar", last modified: Mon May 13 15:08:35 2024, max compression
```

## Comparing `kio-0.0.0a3.tar` & `kio-0.1.0.tar`

### file list

```diff
@@ -1,1354 +1,1356 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.282151 kio-0.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-13 09:44:25.000000 kio-0.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-13 09:44:25.000000 kio-0.0.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-13 09:44:25.000000 kio-0.0.0a3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-02-13 09:44:34.282151 kio-0.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-02-13 09:44:25.000000 kio-0.0.0a3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-02-13 09:44:25.000000 kio-0.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 09:44:34.282151 kio-0.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.086149 kio-0.0.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.130149 kio-0.0.0a3/src/kio/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.130149 kio-0.0.0a3/src/kio/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.130149 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.130149 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.130149 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.130149 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.130149 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.130149 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.134149 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.134149 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.134149 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.134149 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.134149 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.134149 kio-0.0.0a3/src/kio/schema/allocate_producer_ids/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/allocate_producer_ids/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.134149 kio-0.0.0a3/src/kio/schema/allocate_producer_ids/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/allocate_producer_ids/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/allocate_producer_ids/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/allocate_producer_ids/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.134149 kio-0.0.0a3/src/kio/schema/alter_client_quotas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_client_quotas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.134149 kio-0.0.0a3/src/kio/schema/alter_client_quotas/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_client_quotas/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_client_quotas/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_client_quotas/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.138150 kio-0.0.0a3/src/kio/schema/alter_client_quotas/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_client_quotas/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_client_quotas/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_client_quotas/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.138150 kio-0.0.0a3/src/kio/schema/alter_configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.138150 kio-0.0.0a3/src/kio/schema/alter_configs/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_configs/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_configs/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_configs/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.138150 kio-0.0.0a3/src/kio/schema/alter_configs/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_configs/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_configs/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_configs/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.138150 kio-0.0.0a3/src/kio/schema/alter_configs/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_configs/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_configs/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_configs/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.138150 kio-0.0.0a3/src/kio/schema/alter_partition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.138150 kio-0.0.0a3/src/kio/schema/alter_partition/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.138150 kio-0.0.0a3/src/kio/schema/alter_partition/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.138150 kio-0.0.0a3/src/kio/schema/alter_partition/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.138150 kio-0.0.0a3/src/kio/schema/alter_partition/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.138150 kio-0.0.0a3/src/kio/schema/alter_partition_reassignments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition_reassignments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.142150 kio-0.0.0a3/src/kio/schema/alter_partition_reassignments/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition_reassignments/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition_reassignments/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_partition_reassignments/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.142150 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.142150 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.142150 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.142150 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.142150 kio-0.0.0a3/src/kio/schema/alter_user_scram_credentials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_user_scram_credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.142150 kio-0.0.0a3/src/kio/schema/alter_user_scram_credentials/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_user_scram_credentials/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_user_scram_credentials/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/alter_user_scram_credentials/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.142150 kio-0.0.0a3/src/kio/schema/api_versions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.142150 kio-0.0.0a3/src/kio/schema/api_versions/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.142150 kio-0.0.0a3/src/kio/schema/api_versions/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/api_versions/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/api_versions/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/api_versions/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/begin_quorum_epoch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/begin_quorum_epoch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/begin_quorum_epoch/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/begin_quorum_epoch/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/begin_quorum_epoch/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/begin_quorum_epoch/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/broker_heartbeat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/broker_heartbeat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/broker_heartbeat/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/broker_heartbeat/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/broker_heartbeat/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/broker_heartbeat/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/broker_registration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/broker_registration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/broker_registration/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/broker_registration/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/broker_registration/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/broker_registration/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/broker_registration/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/broker_registration/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/broker_registration/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/broker_registration/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/consumer_group_heartbeat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_group_heartbeat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/consumer_group_heartbeat/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_group_heartbeat/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_group_heartbeat/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_group_heartbeat/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.146150 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v0/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v0/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v1/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v2/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v2/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v3/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v3/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v0/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v0/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v1/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v2/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v2/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v3/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v3/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/controlled_shutdown/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.150150 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.154150 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/controlled_shutdown/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.154150 kio-0.0.0a3/src/kio/schema/create_acls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.154150 kio-0.0.0a3/src/kio/schema/create_acls/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.154150 kio-0.0.0a3/src/kio/schema/create_acls/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.154150 kio-0.0.0a3/src/kio/schema/create_acls/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.154150 kio-0.0.0a3/src/kio/schema/create_acls/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_acls/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.154150 kio-0.0.0a3/src/kio/schema/create_delegation_token/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.154150 kio-0.0.0a3/src/kio/schema/create_delegation_token/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.154150 kio-0.0.0a3/src/kio/schema/create_delegation_token/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.158150 kio-0.0.0a3/src/kio/schema/create_delegation_token/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.158150 kio-0.0.0a3/src/kio/schema/create_delegation_token/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_delegation_token/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.158150 kio-0.0.0a3/src/kio/schema/create_partitions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.158150 kio-0.0.0a3/src/kio/schema/create_partitions/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.158150 kio-0.0.0a3/src/kio/schema/create_partitions/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.158150 kio-0.0.0a3/src/kio/schema/create_partitions/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.158150 kio-0.0.0a3/src/kio/schema/create_partitions/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_partitions/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.158150 kio-0.0.0a3/src/kio/schema/create_topics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.158150 kio-0.0.0a3/src/kio/schema/create_topics/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.158150 kio-0.0.0a3/src/kio/schema/create_topics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.162150 kio-0.0.0a3/src/kio/schema/create_topics/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.162150 kio-0.0.0a3/src/kio/schema/create_topics/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.162150 kio-0.0.0a3/src/kio/schema/create_topics/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.162150 kio-0.0.0a3/src/kio/schema/create_topics/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.162150 kio-0.0.0a3/src/kio/schema/create_topics/v6/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v6/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v6/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.162150 kio-0.0.0a3/src/kio/schema/create_topics/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v7/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/create_topics/v7/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.162150 kio-0.0.0a3/src/kio/schema/default_principal_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/default_principal_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.162150 kio-0.0.0a3/src/kio/schema/default_principal_data/v0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/default_principal_data/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/default_principal_data/v0/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.162150 kio-0.0.0a3/src/kio/schema/delete_acls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.162150 kio-0.0.0a3/src/kio/schema/delete_acls/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.166150 kio-0.0.0a3/src/kio/schema/delete_acls/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.166150 kio-0.0.0a3/src/kio/schema/delete_acls/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.166150 kio-0.0.0a3/src/kio/schema/delete_acls/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_acls/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.166150 kio-0.0.0a3/src/kio/schema/delete_groups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.166150 kio-0.0.0a3/src/kio/schema/delete_groups/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_groups/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_groups/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_groups/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.166150 kio-0.0.0a3/src/kio/schema/delete_groups/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_groups/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_groups/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_groups/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.166150 kio-0.0.0a3/src/kio/schema/delete_groups/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_groups/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_groups/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_groups/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.166150 kio-0.0.0a3/src/kio/schema/delete_records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.166150 kio-0.0.0a3/src/kio/schema/delete_records/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_records/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_records/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_records/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.166150 kio-0.0.0a3/src/kio/schema/delete_records/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_records/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_records/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_records/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.170150 kio-0.0.0a3/src/kio/schema/delete_records/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_records/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_records/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_records/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.170150 kio-0.0.0a3/src/kio/schema/delete_topics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.170150 kio-0.0.0a3/src/kio/schema/delete_topics/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.170150 kio-0.0.0a3/src/kio/schema/delete_topics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.170150 kio-0.0.0a3/src/kio/schema/delete_topics/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.170150 kio-0.0.0a3/src/kio/schema/delete_topics/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.170150 kio-0.0.0a3/src/kio/schema/delete_topics/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.170150 kio-0.0.0a3/src/kio/schema/delete_topics/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.170150 kio-0.0.0a3/src/kio/schema/delete_topics/v6/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v6/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/delete_topics/v6/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.174150 kio-0.0.0a3/src/kio/schema/describe_acls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.174150 kio-0.0.0a3/src/kio/schema/describe_acls/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.174150 kio-0.0.0a3/src/kio/schema/describe_acls/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.174150 kio-0.0.0a3/src/kio/schema/describe_acls/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.174150 kio-0.0.0a3/src/kio/schema/describe_acls/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_acls/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.174150 kio-0.0.0a3/src/kio/schema/describe_client_quotas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_client_quotas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.174150 kio-0.0.0a3/src/kio/schema/describe_client_quotas/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_client_quotas/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_client_quotas/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_client_quotas/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.174150 kio-0.0.0a3/src/kio/schema/describe_client_quotas/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_client_quotas/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_client_quotas/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_client_quotas/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.174150 kio-0.0.0a3/src/kio/schema/describe_cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.174150 kio-0.0.0a3/src/kio/schema/describe_cluster/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_cluster/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_cluster/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_cluster/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.178150 kio-0.0.0a3/src/kio/schema/describe_configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.178150 kio-0.0.0a3/src/kio/schema/describe_configs/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.178150 kio-0.0.0a3/src/kio/schema/describe_configs/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.178150 kio-0.0.0a3/src/kio/schema/describe_configs/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.178150 kio-0.0.0a3/src/kio/schema/describe_configs/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.178150 kio-0.0.0a3/src/kio/schema/describe_configs/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_configs/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.178150 kio-0.0.0a3/src/kio/schema/describe_delegation_token/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.178150 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.178150 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.182150 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.182150 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_delegation_token/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.182150 kio-0.0.0a3/src/kio/schema/describe_groups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.182150 kio-0.0.0a3/src/kio/schema/describe_groups/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.182150 kio-0.0.0a3/src/kio/schema/describe_groups/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.182150 kio-0.0.0a3/src/kio/schema/describe_groups/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.182150 kio-0.0.0a3/src/kio/schema/describe_groups/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.182150 kio-0.0.0a3/src/kio/schema/describe_groups/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.182150 kio-0.0.0a3/src/kio/schema/describe_groups/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_groups/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.182150 kio-0.0.0a3/src/kio/schema/describe_log_dirs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.186150 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.186150 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.186150 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.186150 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.186150 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_log_dirs/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.186150 kio-0.0.0a3/src/kio/schema/describe_producers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_producers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.186150 kio-0.0.0a3/src/kio/schema/describe_producers/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_producers/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_producers/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_producers/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.186150 kio-0.0.0a3/src/kio/schema/describe_quorum/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_quorum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.186150 kio-0.0.0a3/src/kio/schema/describe_quorum/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_quorum/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_quorum/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_quorum/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.186150 kio-0.0.0a3/src/kio/schema/describe_quorum/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_quorum/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_quorum/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_quorum/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.190150 kio-0.0.0a3/src/kio/schema/describe_transactions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_transactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.190150 kio-0.0.0a3/src/kio/schema/describe_transactions/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_transactions/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_transactions/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_transactions/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.190150 kio-0.0.0a3/src/kio/schema/describe_user_scram_credentials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_user_scram_credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.190150 kio-0.0.0a3/src/kio/schema/describe_user_scram_credentials/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_user_scram_credentials/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_user_scram_credentials/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/describe_user_scram_credentials/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.190150 kio-0.0.0a3/src/kio/schema/elect_leaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/elect_leaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.190150 kio-0.0.0a3/src/kio/schema/elect_leaders/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/elect_leaders/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/elect_leaders/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/elect_leaders/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.190150 kio-0.0.0a3/src/kio/schema/elect_leaders/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/elect_leaders/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/elect_leaders/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/elect_leaders/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.190150 kio-0.0.0a3/src/kio/schema/elect_leaders/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/elect_leaders/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/elect_leaders/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/elect_leaders/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.190150 kio-0.0.0a3/src/kio/schema/end_quorum_epoch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_quorum_epoch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.190150 kio-0.0.0a3/src/kio/schema/end_quorum_epoch/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_quorum_epoch/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_quorum_epoch/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_quorum_epoch/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.190150 kio-0.0.0a3/src/kio/schema/end_txn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.194150 kio-0.0.0a3/src/kio/schema/end_txn/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.194150 kio-0.0.0a3/src/kio/schema/end_txn/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.194150 kio-0.0.0a3/src/kio/schema/end_txn/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.194150 kio-0.0.0a3/src/kio/schema/end_txn/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/end_txn/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.194150 kio-0.0.0a3/src/kio/schema/envelope/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/envelope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.194150 kio-0.0.0a3/src/kio/schema/envelope/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/envelope/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/envelope/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/envelope/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.194150 kio-0.0.0a3/src/kio/schema/expire_delegation_token/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/expire_delegation_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.194150 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.194150 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.194150 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/expire_delegation_token/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.194150 kio-0.0.0a3/src/kio/schema/fetch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.198150 kio-0.0.0a3/src/kio/schema/fetch/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.198150 kio-0.0.0a3/src/kio/schema/fetch/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.198150 kio-0.0.0a3/src/kio/schema/fetch/v10/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v10/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v10/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.198150 kio-0.0.0a3/src/kio/schema/fetch/v11/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v11/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v11/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.198150 kio-0.0.0a3/src/kio/schema/fetch/v12/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v12/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v12/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.198150 kio-0.0.0a3/src/kio/schema/fetch/v13/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v13/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v13/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.198150 kio-0.0.0a3/src/kio/schema/fetch/v14/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v14/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v14/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v14/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.198150 kio-0.0.0a3/src/kio/schema/fetch/v15/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v15/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v15/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v15/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.202150 kio-0.0.0a3/src/kio/schema/fetch/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.202150 kio-0.0.0a3/src/kio/schema/fetch/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.202150 kio-0.0.0a3/src/kio/schema/fetch/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.202150 kio-0.0.0a3/src/kio/schema/fetch/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.202150 kio-0.0.0a3/src/kio/schema/fetch/v6/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v6/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v6/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.202150 kio-0.0.0a3/src/kio/schema/fetch/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v7/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v7/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.202150 kio-0.0.0a3/src/kio/schema/fetch/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v8/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v8/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.202150 kio-0.0.0a3/src/kio/schema/fetch/v9/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v9/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch/v9/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.202150 kio-0.0.0a3/src/kio/schema/fetch_snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch_snapshot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.206150 kio-0.0.0a3/src/kio/schema/fetch_snapshot/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch_snapshot/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch_snapshot/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/fetch_snapshot/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.206150 kio-0.0.0a3/src/kio/schema/find_coordinator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.206150 kio-0.0.0a3/src/kio/schema/find_coordinator/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.206150 kio-0.0.0a3/src/kio/schema/find_coordinator/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.206150 kio-0.0.0a3/src/kio/schema/find_coordinator/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.206150 kio-0.0.0a3/src/kio/schema/find_coordinator/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.206150 kio-0.0.0a3/src/kio/schema/find_coordinator/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/find_coordinator/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.206150 kio-0.0.0a3/src/kio/schema/heartbeat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.206150 kio-0.0.0a3/src/kio/schema/heartbeat/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.206150 kio-0.0.0a3/src/kio/schema/heartbeat/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.210150 kio-0.0.0a3/src/kio/schema/heartbeat/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.210150 kio-0.0.0a3/src/kio/schema/heartbeat/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.210150 kio-0.0.0a3/src/kio/schema/heartbeat/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/heartbeat/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.210150 kio-0.0.0a3/src/kio/schema/incremental_alter_configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/incremental_alter_configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.210150 kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.210150 kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.210150 kio-0.0.0a3/src/kio/schema/init_producer_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.210150 kio-0.0.0a3/src/kio/schema/init_producer_id/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.210150 kio-0.0.0a3/src/kio/schema/init_producer_id/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.214150 kio-0.0.0a3/src/kio/schema/init_producer_id/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.214150 kio-0.0.0a3/src/kio/schema/init_producer_id/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.214150 kio-0.0.0a3/src/kio/schema/init_producer_id/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/init_producer_id/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.214150 kio-0.0.0a3/src/kio/schema/join_group/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.214150 kio-0.0.0a3/src/kio/schema/join_group/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.214150 kio-0.0.0a3/src/kio/schema/join_group/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.214150 kio-0.0.0a3/src/kio/schema/join_group/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.214150 kio-0.0.0a3/src/kio/schema/join_group/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.214150 kio-0.0.0a3/src/kio/schema/join_group/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.214150 kio-0.0.0a3/src/kio/schema/join_group/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.218150 kio-0.0.0a3/src/kio/schema/join_group/v6/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v6/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v6/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.218150 kio-0.0.0a3/src/kio/schema/join_group/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v7/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v7/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.218150 kio-0.0.0a3/src/kio/schema/join_group/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v8/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v8/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.218150 kio-0.0.0a3/src/kio/schema/join_group/v9/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v9/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/join_group/v9/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.218150 kio-0.0.0a3/src/kio/schema/leader_and_isr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.218150 kio-0.0.0a3/src/kio/schema/leader_and_isr/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.218150 kio-0.0.0a3/src/kio/schema/leader_and_isr/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.218150 kio-0.0.0a3/src/kio/schema/leader_and_isr/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.218150 kio-0.0.0a3/src/kio/schema/leader_and_isr/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.222150 kio-0.0.0a3/src/kio/schema/leader_and_isr/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.222150 kio-0.0.0a3/src/kio/schema/leader_and_isr/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.222150 kio-0.0.0a3/src/kio/schema/leader_and_isr/v6/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v6/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v6/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.222150 kio-0.0.0a3/src/kio/schema/leader_and_isr/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v7/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_and_isr/v7/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.222150 kio-0.0.0a3/src/kio/schema/leader_change_message/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_change_message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.222150 kio-0.0.0a3/src/kio/schema/leader_change_message/v0/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_change_message/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leader_change_message/v0/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.222150 kio-0.0.0a3/src/kio/schema/leave_group/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.222150 kio-0.0.0a3/src/kio/schema/leave_group/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.222150 kio-0.0.0a3/src/kio/schema/leave_group/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.222150 kio-0.0.0a3/src/kio/schema/leave_group/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.226150 kio-0.0.0a3/src/kio/schema/leave_group/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.226150 kio-0.0.0a3/src/kio/schema/leave_group/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.226150 kio-0.0.0a3/src/kio/schema/leave_group/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/leave_group/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.226150 kio-0.0.0a3/src/kio/schema/list_groups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.226150 kio-0.0.0a3/src/kio/schema/list_groups/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.226150 kio-0.0.0a3/src/kio/schema/list_groups/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.226150 kio-0.0.0a3/src/kio/schema/list_groups/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.226150 kio-0.0.0a3/src/kio/schema/list_groups/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.226150 kio-0.0.0a3/src/kio/schema/list_groups/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_groups/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.226150 kio-0.0.0a3/src/kio/schema/list_offsets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.230151 kio-0.0.0a3/src/kio/schema/list_offsets/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.230151 kio-0.0.0a3/src/kio/schema/list_offsets/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.230151 kio-0.0.0a3/src/kio/schema/list_offsets/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.230151 kio-0.0.0a3/src/kio/schema/list_offsets/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.230151 kio-0.0.0a3/src/kio/schema/list_offsets/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.230151 kio-0.0.0a3/src/kio/schema/list_offsets/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.230151 kio-0.0.0a3/src/kio/schema/list_offsets/v6/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v6/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v6/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.230151 kio-0.0.0a3/src/kio/schema/list_offsets/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v7/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v7/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.234151 kio-0.0.0a3/src/kio/schema/list_offsets/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v8/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_offsets/v8/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.234151 kio-0.0.0a3/src/kio/schema/list_partition_reassignments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_partition_reassignments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.234151 kio-0.0.0a3/src/kio/schema/list_partition_reassignments/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_partition_reassignments/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_partition_reassignments/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_partition_reassignments/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.234151 kio-0.0.0a3/src/kio/schema/list_transactions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_transactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.234151 kio-0.0.0a3/src/kio/schema/list_transactions/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_transactions/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_transactions/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/list_transactions/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.234151 kio-0.0.0a3/src/kio/schema/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.234151 kio-0.0.0a3/src/kio/schema/metadata/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.234151 kio-0.0.0a3/src/kio/schema/metadata/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.234151 kio-0.0.0a3/src/kio/schema/metadata/v10/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v10/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v10/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.234151 kio-0.0.0a3/src/kio/schema/metadata/v11/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v11/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v11/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.234151 kio-0.0.0a3/src/kio/schema/metadata/v12/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v12/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v12/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.238151 kio-0.0.0a3/src/kio/schema/metadata/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.238151 kio-0.0.0a3/src/kio/schema/metadata/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.238151 kio-0.0.0a3/src/kio/schema/metadata/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.238151 kio-0.0.0a3/src/kio/schema/metadata/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.238151 kio-0.0.0a3/src/kio/schema/metadata/v6/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v6/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v6/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.238151 kio-0.0.0a3/src/kio/schema/metadata/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v7/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v7/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.238151 kio-0.0.0a3/src/kio/schema/metadata/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v8/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v8/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.238151 kio-0.0.0a3/src/kio/schema/metadata/v9/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v9/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/metadata/v9/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.242151 kio-0.0.0a3/src/kio/schema/offset_commit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.242151 kio-0.0.0a3/src/kio/schema/offset_commit/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.242151 kio-0.0.0a3/src/kio/schema/offset_commit/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.242151 kio-0.0.0a3/src/kio/schema/offset_commit/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.242151 kio-0.0.0a3/src/kio/schema/offset_commit/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.242151 kio-0.0.0a3/src/kio/schema/offset_commit/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.242151 kio-0.0.0a3/src/kio/schema/offset_commit/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.242151 kio-0.0.0a3/src/kio/schema/offset_commit/v6/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v6/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v6/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.242151 kio-0.0.0a3/src/kio/schema/offset_commit/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v7/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v7/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.242151 kio-0.0.0a3/src/kio/schema/offset_commit/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v8/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v8/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.246151 kio-0.0.0a3/src/kio/schema/offset_commit/v9/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v9/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_commit/v9/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.246151 kio-0.0.0a3/src/kio/schema/offset_delete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_delete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.246151 kio-0.0.0a3/src/kio/schema/offset_delete/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_delete/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_delete/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_delete/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.246151 kio-0.0.0a3/src/kio/schema/offset_fetch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.246151 kio-0.0.0a3/src/kio/schema/offset_fetch/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.246151 kio-0.0.0a3/src/kio/schema/offset_fetch/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.246151 kio-0.0.0a3/src/kio/schema/offset_fetch/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.246151 kio-0.0.0a3/src/kio/schema/offset_fetch/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.246151 kio-0.0.0a3/src/kio/schema/offset_fetch/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.246151 kio-0.0.0a3/src/kio/schema/offset_fetch/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.246151 kio-0.0.0a3/src/kio/schema/offset_fetch/v6/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v6/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v6/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.250151 kio-0.0.0a3/src/kio/schema/offset_fetch/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v7/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v7/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.250151 kio-0.0.0a3/src/kio/schema/offset_fetch/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v8/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_fetch/v8/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.250151 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.250151 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.250151 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.250151 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.250151 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.250151 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.250151 kio-0.0.0a3/src/kio/schema/produce/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.250151 kio-0.0.0a3/src/kio/schema/produce/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.250151 kio-0.0.0a3/src/kio/schema/produce/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.254151 kio-0.0.0a3/src/kio/schema/produce/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.254151 kio-0.0.0a3/src/kio/schema/produce/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.254151 kio-0.0.0a3/src/kio/schema/produce/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.254151 kio-0.0.0a3/src/kio/schema/produce/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.254151 kio-0.0.0a3/src/kio/schema/produce/v6/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v6/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v6/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.254151 kio-0.0.0a3/src/kio/schema/produce/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v7/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v7/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.254151 kio-0.0.0a3/src/kio/schema/produce/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v8/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v8/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.254151 kio-0.0.0a3/src/kio/schema/produce/v9/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v9/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/produce/v9/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.254151 kio-0.0.0a3/src/kio/schema/renew_delegation_token/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/renew_delegation_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.254151 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/renew_delegation_token/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/request_header/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/request_header/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/request_header/v0/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/request_header/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/request_header/v0/header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/request_header/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/request_header/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/request_header/v1/header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/request_header/v2/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/request_header/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/request_header/v2/header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/response_header/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/response_header/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/response_header/v0/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/response_header/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/response_header/v0/header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/response_header/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/response_header/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/response_header/v1/header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/sasl_authenticate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_authenticate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_authenticate/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.258151 kio-0.0.0a3/src/kio/schema/sasl_handshake/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_handshake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.262151 kio-0.0.0a3/src/kio/schema/sasl_handshake/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_handshake/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_handshake/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_handshake/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.262151 kio-0.0.0a3/src/kio/schema/sasl_handshake/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_handshake/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_handshake/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sasl_handshake/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.262151 kio-0.0.0a3/src/kio/schema/snapshot_footer_record/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/snapshot_footer_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.262151 kio-0.0.0a3/src/kio/schema/snapshot_footer_record/v0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/snapshot_footer_record/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/snapshot_footer_record/v0/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.262151 kio-0.0.0a3/src/kio/schema/snapshot_header_record/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/snapshot_header_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.262151 kio-0.0.0a3/src/kio/schema/snapshot_header_record/v0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/snapshot_header_record/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/snapshot_header_record/v0/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.262151 kio-0.0.0a3/src/kio/schema/stop_replica/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.262151 kio-0.0.0a3/src/kio/schema/stop_replica/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.262151 kio-0.0.0a3/src/kio/schema/stop_replica/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.262151 kio-0.0.0a3/src/kio/schema/stop_replica/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.262151 kio-0.0.0a3/src/kio/schema/stop_replica/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.266151 kio-0.0.0a3/src/kio/schema/stop_replica/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/stop_replica/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.266151 kio-0.0.0a3/src/kio/schema/sync_group/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.266151 kio-0.0.0a3/src/kio/schema/sync_group/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.266151 kio-0.0.0a3/src/kio/schema/sync_group/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.266151 kio-0.0.0a3/src/kio/schema/sync_group/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.266151 kio-0.0.0a3/src/kio/schema/sync_group/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.266151 kio-0.0.0a3/src/kio/schema/sync_group/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.266151 kio-0.0.0a3/src/kio/schema/sync_group/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/sync_group/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.266151 kio-0.0.0a3/src/kio/schema/txn_offset_commit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.270151 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.270151 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.270151 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.270151 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/txn_offset_commit/v3/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.270151 kio-0.0.0a3/src/kio/schema/unregister_broker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/unregister_broker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.270151 kio-0.0.0a3/src/kio/schema/unregister_broker/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/unregister_broker/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/unregister_broker/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/unregister_broker/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.270151 kio-0.0.0a3/src/kio/schema/update_features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.270151 kio-0.0.0a3/src/kio/schema/update_features/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_features/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_features/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_features/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.270151 kio-0.0.0a3/src/kio/schema/update_features/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_features/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_features/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_features/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.270151 kio-0.0.0a3/src/kio/schema/update_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.270151 kio-0.0.0a3/src/kio/schema/update_metadata/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.274151 kio-0.0.0a3/src/kio/schema/update_metadata/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.274151 kio-0.0.0a3/src/kio/schema/update_metadata/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v2/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v2/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.274151 kio-0.0.0a3/src/kio/schema/update_metadata/v3/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.274151 kio-0.0.0a3/src/kio/schema/update_metadata/v4/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v4/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v4/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.274151 kio-0.0.0a3/src/kio/schema/update_metadata/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v5/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v5/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.274151 kio-0.0.0a3/src/kio/schema/update_metadata/v6/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v6/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v6/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.274151 kio-0.0.0a3/src/kio/schema/update_metadata/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v7/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v7/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.274151 kio-0.0.0a3/src/kio/schema/update_metadata/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v8/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/update_metadata/v8/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.274151 kio-0.0.0a3/src/kio/schema/vote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/vote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.278151 kio-0.0.0a3/src/kio/schema/vote/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/vote/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/vote/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/vote/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.278151 kio-0.0.0a3/src/kio/schema/write_txn_markers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/write_txn_markers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.278151 kio-0.0.0a3/src/kio/schema/write_txn_markers/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/write_txn_markers/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/write_txn_markers/v0/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/write_txn_markers/v0/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.278151 kio-0.0.0a3/src/kio/schema/write_txn_markers/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/write_txn_markers/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/write_txn_markers/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/schema/write_txn_markers/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.278151 kio-0.0.0a3/src/kio/serial/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/serial/_introspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/serial/_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/serial/_serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/serial/_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/serial/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/serial/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/serial/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.278151 kio-0.0.0a3/src/kio/static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/static/_phantom.py
--rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/static/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/static/primitive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-02-13 09:44:25.000000 kio-0.0.0a3/src/kio/static/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:44:34.278151 kio-0.0.0a3/src/kio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-02-13 09:44:33.000000 kio-0.0.0a3/src/kio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    43053 2024-02-13 09:44:34.000000 kio-0.0.0a3/src/kio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 09:44:33.000000 kio-0.0.0a3/src/kio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-13 09:44:33.000000 kio-0.0.0a3/src/kio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-13 09:44:33.000000 kio-0.0.0a3/src/kio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.014700 kio-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-13 15:08:28.000000 kio-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-13 15:08:28.000000 kio-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 15:08:28.000000 kio-0.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-13 15:08:35.014700 kio-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-13 15:08:28.000000 kio-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-13 15:08:28.000000 kio-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:08:35.014700 kio-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.830698 kio-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.870698 kio-0.1.0/src/kio/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.874698 kio-0.1.0/src/kio/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.874698 kio-0.1.0/src/kio/schema/add_offsets_to_txn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.874698 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.874698 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.874698 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.874698 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_offsets_to_txn/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.874698 kio-0.1.0/src/kio/schema/add_partitions_to_txn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.874698 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.874698 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.874698 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/add_partitions_to_txn/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/allocate_producer_ids/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/allocate_producer_ids/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/allocate_producer_ids/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/allocate_producer_ids/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/allocate_producer_ids/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/allocate_producer_ids/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/alter_client_quotas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_client_quotas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/alter_client_quotas/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_client_quotas/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_client_quotas/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_client_quotas/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/alter_client_quotas/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_client_quotas/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_client_quotas/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_client_quotas/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/alter_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/alter_configs/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_configs/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_configs/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_configs/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/alter_configs/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_configs/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_configs/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_configs/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/alter_configs/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_configs/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_configs/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_configs/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/alter_partition/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.878698 kio-0.1.0/src/kio/schema/alter_partition/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.882699 kio-0.1.0/src/kio/schema/alter_partition/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.882699 kio-0.1.0/src/kio/schema/alter_partition/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.882699 kio-0.1.0/src/kio/schema/alter_partition/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.882699 kio-0.1.0/src/kio/schema/alter_partition_reassignments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition_reassignments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.882699 kio-0.1.0/src/kio/schema/alter_partition_reassignments/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition_reassignments/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition_reassignments/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_partition_reassignments/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.882699 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.882699 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.882699 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.882699 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.882699 kio-0.1.0/src/kio/schema/alter_user_scram_credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_user_scram_credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/alter_user_scram_credentials/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_user_scram_credentials/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_user_scram_credentials/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/alter_user_scram_credentials/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/api_versions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/api_versions/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/api_versions/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/api_versions/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/api_versions/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/api_versions/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/begin_quorum_epoch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/begin_quorum_epoch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/begin_quorum_epoch/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/begin_quorum_epoch/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/begin_quorum_epoch/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/begin_quorum_epoch/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/broker_heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/broker_heartbeat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/broker_heartbeat/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/broker_heartbeat/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/broker_heartbeat/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/broker_heartbeat/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/broker_registration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/broker_registration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.886699 kio-0.1.0/src/kio/schema/broker_registration/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/broker_registration/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/broker_registration/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/broker_registration/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/broker_registration/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/broker_registration/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/broker_registration/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/broker_registration/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/consumer_group_heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_group_heartbeat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/consumer_group_heartbeat/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_group_heartbeat/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_group_heartbeat/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_group_heartbeat/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v0/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v1/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v2/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v3/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v0/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v1/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.890699 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v2/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.894699 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v3/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.894699 kio-0.1.0/src/kio/schema/controlled_shutdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.894699 kio-0.1.0/src/kio/schema/controlled_shutdown/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.894699 kio-0.1.0/src/kio/schema/controlled_shutdown/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.894699 kio-0.1.0/src/kio/schema/controlled_shutdown/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.894699 kio-0.1.0/src/kio/schema/controlled_shutdown/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/controlled_shutdown/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.894699 kio-0.1.0/src/kio/schema/create_acls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.894699 kio-0.1.0/src/kio/schema/create_acls/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.894699 kio-0.1.0/src/kio/schema/create_acls/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.894699 kio-0.1.0/src/kio/schema/create_acls/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.898699 kio-0.1.0/src/kio/schema/create_acls/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_acls/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.898699 kio-0.1.0/src/kio/schema/create_delegation_token/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.898699 kio-0.1.0/src/kio/schema/create_delegation_token/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.898699 kio-0.1.0/src/kio/schema/create_delegation_token/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.898699 kio-0.1.0/src/kio/schema/create_delegation_token/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.898699 kio-0.1.0/src/kio/schema/create_delegation_token/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_delegation_token/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.898699 kio-0.1.0/src/kio/schema/create_partitions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.898699 kio-0.1.0/src/kio/schema/create_partitions/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.898699 kio-0.1.0/src/kio/schema/create_partitions/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.902699 kio-0.1.0/src/kio/schema/create_partitions/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.902699 kio-0.1.0/src/kio/schema/create_partitions/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_partitions/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.902699 kio-0.1.0/src/kio/schema/create_topics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.902699 kio-0.1.0/src/kio/schema/create_topics/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.902699 kio-0.1.0/src/kio/schema/create_topics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.902699 kio-0.1.0/src/kio/schema/create_topics/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.902699 kio-0.1.0/src/kio/schema/create_topics/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.902699 kio-0.1.0/src/kio/schema/create_topics/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.902699 kio-0.1.0/src/kio/schema/create_topics/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.902699 kio-0.1.0/src/kio/schema/create_topics/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v6/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v6/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.906699 kio-0.1.0/src/kio/schema/create_topics/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v7/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/create_topics/v7/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.906699 kio-0.1.0/src/kio/schema/default_principal_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/default_principal_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.906699 kio-0.1.0/src/kio/schema/default_principal_data/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/default_principal_data/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/default_principal_data/v0/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.906699 kio-0.1.0/src/kio/schema/delete_acls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.906699 kio-0.1.0/src/kio/schema/delete_acls/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.906699 kio-0.1.0/src/kio/schema/delete_acls/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.906699 kio-0.1.0/src/kio/schema/delete_acls/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.906699 kio-0.1.0/src/kio/schema/delete_acls/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_acls/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.906699 kio-0.1.0/src/kio/schema/delete_groups/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.906699 kio-0.1.0/src/kio/schema/delete_groups/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_groups/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_groups/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_groups/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.906699 kio-0.1.0/src/kio/schema/delete_groups/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_groups/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_groups/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_groups/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.910699 kio-0.1.0/src/kio/schema/delete_groups/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_groups/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_groups/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_groups/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.910699 kio-0.1.0/src/kio/schema/delete_records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.910699 kio-0.1.0/src/kio/schema/delete_records/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_records/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_records/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_records/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.910699 kio-0.1.0/src/kio/schema/delete_records/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_records/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_records/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_records/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.910699 kio-0.1.0/src/kio/schema/delete_records/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_records/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_records/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_records/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.910699 kio-0.1.0/src/kio/schema/delete_topics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.910699 kio-0.1.0/src/kio/schema/delete_topics/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.910699 kio-0.1.0/src/kio/schema/delete_topics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.910699 kio-0.1.0/src/kio/schema/delete_topics/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.910699 kio-0.1.0/src/kio/schema/delete_topics/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.910699 kio-0.1.0/src/kio/schema/delete_topics/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.914699 kio-0.1.0/src/kio/schema/delete_topics/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.914699 kio-0.1.0/src/kio/schema/delete_topics/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v6/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/delete_topics/v6/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.914699 kio-0.1.0/src/kio/schema/describe_acls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.914699 kio-0.1.0/src/kio/schema/describe_acls/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.914699 kio-0.1.0/src/kio/schema/describe_acls/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.914699 kio-0.1.0/src/kio/schema/describe_acls/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.914699 kio-0.1.0/src/kio/schema/describe_acls/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_acls/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.914699 kio-0.1.0/src/kio/schema/describe_client_quotas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_client_quotas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.914699 kio-0.1.0/src/kio/schema/describe_client_quotas/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_client_quotas/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_client_quotas/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_client_quotas/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.914699 kio-0.1.0/src/kio/schema/describe_client_quotas/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_client_quotas/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_client_quotas/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_client_quotas/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.914699 kio-0.1.0/src/kio/schema/describe_cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.918699 kio-0.1.0/src/kio/schema/describe_cluster/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_cluster/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_cluster/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_cluster/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.918699 kio-0.1.0/src/kio/schema/describe_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.918699 kio-0.1.0/src/kio/schema/describe_configs/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.918699 kio-0.1.0/src/kio/schema/describe_configs/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.918699 kio-0.1.0/src/kio/schema/describe_configs/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.918699 kio-0.1.0/src/kio/schema/describe_configs/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.918699 kio-0.1.0/src/kio/schema/describe_configs/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_configs/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.918699 kio-0.1.0/src/kio/schema/describe_delegation_token/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.918699 kio-0.1.0/src/kio/schema/describe_delegation_token/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.918699 kio-0.1.0/src/kio/schema/describe_delegation_token/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.918699 kio-0.1.0/src/kio/schema/describe_delegation_token/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.922699 kio-0.1.0/src/kio/schema/describe_delegation_token/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_delegation_token/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.922699 kio-0.1.0/src/kio/schema/describe_groups/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.922699 kio-0.1.0/src/kio/schema/describe_groups/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.922699 kio-0.1.0/src/kio/schema/describe_groups/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.922699 kio-0.1.0/src/kio/schema/describe_groups/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.922699 kio-0.1.0/src/kio/schema/describe_groups/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.922699 kio-0.1.0/src/kio/schema/describe_groups/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.922699 kio-0.1.0/src/kio/schema/describe_groups/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_groups/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.922699 kio-0.1.0/src/kio/schema/describe_log_dirs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.922699 kio-0.1.0/src/kio/schema/describe_log_dirs/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_log_dirs/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_log_dirs/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_log_dirs/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_log_dirs/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_log_dirs/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_producers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_producers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_producers/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_producers/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_producers/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_producers/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_quorum/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_quorum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_quorum/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_quorum/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_quorum/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_quorum/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_quorum/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_quorum/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_quorum/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_quorum/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_transactions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_transactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_transactions/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_transactions/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_transactions/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_transactions/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.926699 kio-0.1.0/src/kio/schema/describe_user_scram_credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_user_scram_credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.930699 kio-0.1.0/src/kio/schema/describe_user_scram_credentials/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_user_scram_credentials/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_user_scram_credentials/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/describe_user_scram_credentials/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.930699 kio-0.1.0/src/kio/schema/elect_leaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/elect_leaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.930699 kio-0.1.0/src/kio/schema/elect_leaders/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/elect_leaders/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/elect_leaders/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/elect_leaders/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.930699 kio-0.1.0/src/kio/schema/elect_leaders/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/elect_leaders/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/elect_leaders/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/elect_leaders/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.930699 kio-0.1.0/src/kio/schema/elect_leaders/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/elect_leaders/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/elect_leaders/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/elect_leaders/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.930699 kio-0.1.0/src/kio/schema/end_quorum_epoch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_quorum_epoch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.930699 kio-0.1.0/src/kio/schema/end_quorum_epoch/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_quorum_epoch/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_quorum_epoch/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_quorum_epoch/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.930699 kio-0.1.0/src/kio/schema/end_txn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.930699 kio-0.1.0/src/kio/schema/end_txn/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.930699 kio-0.1.0/src/kio/schema/end_txn/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.930699 kio-0.1.0/src/kio/schema/end_txn/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/end_txn/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/end_txn/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/envelope/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/envelope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/envelope/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/envelope/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/envelope/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/envelope/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/expire_delegation_token/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/expire_delegation_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/expire_delegation_token/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/expire_delegation_token/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/expire_delegation_token/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/expire_delegation_token/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/expire_delegation_token/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/expire_delegation_token/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/expire_delegation_token/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/expire_delegation_token/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/expire_delegation_token/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/expire_delegation_token/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/expire_delegation_token/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/expire_delegation_token/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/fetch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/fetch/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/fetch/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/fetch/v10/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v10/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v10/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/fetch/v11/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v11/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v11/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.934699 kio-0.1.0/src/kio/schema/fetch/v12/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v12/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v12/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.938699 kio-0.1.0/src/kio/schema/fetch/v13/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v13/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v13/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.938699 kio-0.1.0/src/kio/schema/fetch/v14/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v14/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v14/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v14/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.938699 kio-0.1.0/src/kio/schema/fetch/v15/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v15/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v15/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v15/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.938699 kio-0.1.0/src/kio/schema/fetch/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.938699 kio-0.1.0/src/kio/schema/fetch/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.938699 kio-0.1.0/src/kio/schema/fetch/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.938699 kio-0.1.0/src/kio/schema/fetch/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.938699 kio-0.1.0/src/kio/schema/fetch/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v6/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v6/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.938699 kio-0.1.0/src/kio/schema/fetch/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v7/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v7/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.942699 kio-0.1.0/src/kio/schema/fetch/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v8/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v8/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.942699 kio-0.1.0/src/kio/schema/fetch/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v9/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch/v9/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.942699 kio-0.1.0/src/kio/schema/fetch_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch_snapshot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.942699 kio-0.1.0/src/kio/schema/fetch_snapshot/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch_snapshot/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch_snapshot/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/fetch_snapshot/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.942699 kio-0.1.0/src/kio/schema/find_coordinator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.942699 kio-0.1.0/src/kio/schema/find_coordinator/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.942699 kio-0.1.0/src/kio/schema/find_coordinator/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.942699 kio-0.1.0/src/kio/schema/find_coordinator/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.942699 kio-0.1.0/src/kio/schema/find_coordinator/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.942699 kio-0.1.0/src/kio/schema/find_coordinator/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/find_coordinator/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.942699 kio-0.1.0/src/kio/schema/heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.946699 kio-0.1.0/src/kio/schema/heartbeat/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.946699 kio-0.1.0/src/kio/schema/heartbeat/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.946699 kio-0.1.0/src/kio/schema/heartbeat/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.946699 kio-0.1.0/src/kio/schema/heartbeat/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.946699 kio-0.1.0/src/kio/schema/heartbeat/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/heartbeat/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.946699 kio-0.1.0/src/kio/schema/incremental_alter_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/incremental_alter_configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.946699 kio-0.1.0/src/kio/schema/incremental_alter_configs/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/incremental_alter_configs/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/incremental_alter_configs/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/incremental_alter_configs/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.946699 kio-0.1.0/src/kio/schema/incremental_alter_configs/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/incremental_alter_configs/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/incremental_alter_configs/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/incremental_alter_configs/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)   132050 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.946699 kio-0.1.0/src/kio/schema/init_producer_id/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.946699 kio-0.1.0/src/kio/schema/init_producer_id/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.950699 kio-0.1.0/src/kio/schema/init_producer_id/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.950699 kio-0.1.0/src/kio/schema/init_producer_id/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.950699 kio-0.1.0/src/kio/schema/init_producer_id/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.950699 kio-0.1.0/src/kio/schema/init_producer_id/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/init_producer_id/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.950699 kio-0.1.0/src/kio/schema/join_group/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.950699 kio-0.1.0/src/kio/schema/join_group/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.950699 kio-0.1.0/src/kio/schema/join_group/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.950699 kio-0.1.0/src/kio/schema/join_group/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.950699 kio-0.1.0/src/kio/schema/join_group/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.950699 kio-0.1.0/src/kio/schema/join_group/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.954699 kio-0.1.0/src/kio/schema/join_group/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.954699 kio-0.1.0/src/kio/schema/join_group/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v6/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v6/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.954699 kio-0.1.0/src/kio/schema/join_group/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v7/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v7/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.954699 kio-0.1.0/src/kio/schema/join_group/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v8/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v8/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.954699 kio-0.1.0/src/kio/schema/join_group/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v9/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/join_group/v9/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.954699 kio-0.1.0/src/kio/schema/leader_and_isr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.954699 kio-0.1.0/src/kio/schema/leader_and_isr/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.954699 kio-0.1.0/src/kio/schema/leader_and_isr/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.954699 kio-0.1.0/src/kio/schema/leader_and_isr/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.954699 kio-0.1.0/src/kio/schema/leader_and_isr/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leader_and_isr/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leader_and_isr/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leader_and_isr/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v6/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v6/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leader_and_isr/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v7/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_and_isr/v7/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leader_change_message/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_change_message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leader_change_message/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_change_message/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leader_change_message/v0/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leave_group/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leave_group/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leave_group/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leave_group/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leave_group/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.958699 kio-0.1.0/src/kio/schema/leave_group/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.962699 kio-0.1.0/src/kio/schema/leave_group/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/leave_group/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.962699 kio-0.1.0/src/kio/schema/list_groups/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.962699 kio-0.1.0/src/kio/schema/list_groups/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.962699 kio-0.1.0/src/kio/schema/list_groups/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.962699 kio-0.1.0/src/kio/schema/list_groups/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.962699 kio-0.1.0/src/kio/schema/list_groups/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.962699 kio-0.1.0/src/kio/schema/list_groups/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_groups/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.962699 kio-0.1.0/src/kio/schema/list_offsets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.962699 kio-0.1.0/src/kio/schema/list_offsets/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.962699 kio-0.1.0/src/kio/schema/list_offsets/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/list_offsets/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/list_offsets/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/list_offsets/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/list_offsets/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/list_offsets/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v6/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v6/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/list_offsets/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v7/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v7/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/list_offsets/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v8/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_offsets/v8/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/list_partition_reassignments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_partition_reassignments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/list_partition_reassignments/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_partition_reassignments/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_partition_reassignments/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_partition_reassignments/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/list_transactions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_transactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/list_transactions/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_transactions/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_transactions/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/list_transactions/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.966699 kio-0.1.0/src/kio/schema/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.970699 kio-0.1.0/src/kio/schema/metadata/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.970699 kio-0.1.0/src/kio/schema/metadata/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.970699 kio-0.1.0/src/kio/schema/metadata/v10/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v10/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v10/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.970699 kio-0.1.0/src/kio/schema/metadata/v11/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v11/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v11/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.970699 kio-0.1.0/src/kio/schema/metadata/v12/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v12/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v12/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.970699 kio-0.1.0/src/kio/schema/metadata/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.970699 kio-0.1.0/src/kio/schema/metadata/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.970699 kio-0.1.0/src/kio/schema/metadata/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.970699 kio-0.1.0/src/kio/schema/metadata/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.974699 kio-0.1.0/src/kio/schema/metadata/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v6/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v6/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.974699 kio-0.1.0/src/kio/schema/metadata/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v7/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v7/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.974699 kio-0.1.0/src/kio/schema/metadata/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v8/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v8/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.974699 kio-0.1.0/src/kio/schema/metadata/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v9/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/metadata/v9/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.974699 kio-0.1.0/src/kio/schema/offset_commit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.974699 kio-0.1.0/src/kio/schema/offset_commit/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.974699 kio-0.1.0/src/kio/schema/offset_commit/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.974699 kio-0.1.0/src/kio/schema/offset_commit/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.974699 kio-0.1.0/src/kio/schema/offset_commit/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.978700 kio-0.1.0/src/kio/schema/offset_commit/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.978700 kio-0.1.0/src/kio/schema/offset_commit/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.978700 kio-0.1.0/src/kio/schema/offset_commit/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v6/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v6/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.978700 kio-0.1.0/src/kio/schema/offset_commit/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v7/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v7/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.978700 kio-0.1.0/src/kio/schema/offset_commit/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v8/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v8/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.978700 kio-0.1.0/src/kio/schema/offset_commit/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v9/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_commit/v9/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.978700 kio-0.1.0/src/kio/schema/offset_delete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_delete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.978700 kio-0.1.0/src/kio/schema/offset_delete/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_delete/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_delete/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_delete/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.978700 kio-0.1.0/src/kio/schema/offset_fetch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.978700 kio-0.1.0/src/kio/schema/offset_fetch/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.978700 kio-0.1.0/src/kio/schema/offset_fetch/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.982699 kio-0.1.0/src/kio/schema/offset_fetch/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.982699 kio-0.1.0/src/kio/schema/offset_fetch/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.982699 kio-0.1.0/src/kio/schema/offset_fetch/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.982699 kio-0.1.0/src/kio/schema/offset_fetch/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.982699 kio-0.1.0/src/kio/schema/offset_fetch/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v6/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v6/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.982699 kio-0.1.0/src/kio/schema/offset_fetch/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v7/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v7/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.982699 kio-0.1.0/src/kio/schema/offset_fetch/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v8/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_fetch/v8/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.982699 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.982699 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.982699 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.986700 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.986700 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.986700 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.986700 kio-0.1.0/src/kio/schema/produce/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.986700 kio-0.1.0/src/kio/schema/produce/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.986700 kio-0.1.0/src/kio/schema/produce/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.986700 kio-0.1.0/src/kio/schema/produce/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.986700 kio-0.1.0/src/kio/schema/produce/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.986700 kio-0.1.0/src/kio/schema/produce/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.986700 kio-0.1.0/src/kio/schema/produce/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/produce/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v6/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v6/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/produce/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v7/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v7/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/produce/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v8/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v8/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/produce/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v9/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/produce/v9/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/renew_delegation_token/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/renew_delegation_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/renew_delegation_token/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/renew_delegation_token/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/renew_delegation_token/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/renew_delegation_token/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/renew_delegation_token/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/renew_delegation_token/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/renew_delegation_token/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/renew_delegation_token/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/renew_delegation_token/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/renew_delegation_token/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/renew_delegation_token/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/renew_delegation_token/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/request_header/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/request_header/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/request_header/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/request_header/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/request_header/v0/header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/request_header/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/request_header/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/request_header/v1/header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.990700 kio-0.1.0/src/kio/schema/request_header/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/request_header/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/request_header/v2/header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/response_header/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/response_header/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/response_header/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/response_header/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/response_header/v0/header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/response_header/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/response_header/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/response_header/v1/header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/sasl_authenticate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_authenticate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/sasl_authenticate/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_authenticate/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_authenticate/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_authenticate/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/sasl_authenticate/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_authenticate/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_authenticate/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_authenticate/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/sasl_authenticate/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_authenticate/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_authenticate/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_authenticate/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/sasl_handshake/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_handshake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/sasl_handshake/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_handshake/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_handshake/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_handshake/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/sasl_handshake/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_handshake/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_handshake/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sasl_handshake/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/snapshot_footer_record/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/snapshot_footer_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/snapshot_footer_record/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/snapshot_footer_record/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/snapshot_footer_record/v0/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/snapshot_header_record/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/snapshot_header_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.994700 kio-0.1.0/src/kio/schema/snapshot_header_record/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/snapshot_header_record/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/snapshot_header_record/v0/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.998700 kio-0.1.0/src/kio/schema/stop_replica/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.998700 kio-0.1.0/src/kio/schema/stop_replica/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.998700 kio-0.1.0/src/kio/schema/stop_replica/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.998700 kio-0.1.0/src/kio/schema/stop_replica/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.998700 kio-0.1.0/src/kio/schema/stop_replica/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.998700 kio-0.1.0/src/kio/schema/stop_replica/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/stop_replica/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.998700 kio-0.1.0/src/kio/schema/sync_group/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.998700 kio-0.1.0/src/kio/schema/sync_group/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.998700 kio-0.1.0/src/kio/schema/sync_group/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:34.998700 kio-0.1.0/src/kio/schema/sync_group/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/sync_group/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/sync_group/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-13 15:08:28.000000 kio-0.1.0/src/kio/schema/sync_group/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/sync_group/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/sync_group/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/sync_group/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/sync_group/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/txn_offset_commit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/txn_offset_commit/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/txn_offset_commit/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/txn_offset_commit/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/txn_offset_commit/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/txn_offset_commit/v3/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/unregister_broker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/unregister_broker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/unregister_broker/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/unregister_broker/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/unregister_broker/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/unregister_broker/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/update_features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.002700 kio-0.1.0/src/kio/schema/update_features/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_features/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_features/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_features/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.006700 kio-0.1.0/src/kio/schema/update_features/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_features/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_features/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_features/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.006700 kio-0.1.0/src/kio/schema/update_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.006700 kio-0.1.0/src/kio/schema/update_metadata/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.006700 kio-0.1.0/src/kio/schema/update_metadata/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.006700 kio-0.1.0/src/kio/schema/update_metadata/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v2/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v2/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.006700 kio-0.1.0/src/kio/schema/update_metadata/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.006700 kio-0.1.0/src/kio/schema/update_metadata/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v4/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v4/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.006700 kio-0.1.0/src/kio/schema/update_metadata/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v5/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v5/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.006700 kio-0.1.0/src/kio/schema/update_metadata/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v6/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v6/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.006700 kio-0.1.0/src/kio/schema/update_metadata/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v7/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v7/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.010700 kio-0.1.0/src/kio/schema/update_metadata/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v8/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/update_metadata/v8/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.010700 kio-0.1.0/src/kio/schema/vote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/vote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.010700 kio-0.1.0/src/kio/schema/vote/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/vote/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/vote/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/vote/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.010700 kio-0.1.0/src/kio/schema/write_txn_markers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/write_txn_markers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.010700 kio-0.1.0/src/kio/schema/write_txn_markers/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/write_txn_markers/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/write_txn_markers/v0/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/write_txn_markers/v0/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.010700 kio-0.1.0/src/kio/schema/write_txn_markers/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/write_txn_markers/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/write_txn_markers/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/schema/write_txn_markers/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.010700 kio-0.1.0/src/kio/serial/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/serial/_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/serial/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/serial/_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/serial/_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/serial/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/serial/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/serial/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.010700 kio-0.1.0/src/kio/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/static/_phantom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/static/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/static/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-13 15:08:29.000000 kio-0.1.0/src/kio/static/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:08:35.014700 kio-0.1.0/src/kio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-13 15:08:34.000000 kio-0.1.0/src/kio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    43094 2024-05-13 15:08:34.000000 kio-0.1.0/src/kio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:08:34.000000 kio-0.1.0/src/kio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 15:08:34.000000 kio-0.1.0/src/kio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-13 15:08:34.000000 kio-0.1.0/src/kio.egg-info/top_level.txt
```

### Comparing `kio-0.0.0a3/LICENSE` & `kio-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/PKG-INFO` & `kio-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: kio
-Version: 0.0.0a3
+Version: 0.1.0
 Summary: Python data types for the Apache Kafka® Protocol.
 Author-email: Anton Agestam <anton.agestam@aiven.io>
 License: Apache-2.0 license
 Project-URL: Source Repository, https://github.com/Aiven-Open/kio
+Project-URL: Documentation, https://aiven-open.github.io/kio/
 Project-URL: Bug Tracker, https://github.com/Aiven-Open/kio/issues
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: kio Version: 0.0.0a3 Summary: Python data types for
+Metadata-Version: 2.1 Name: kio Version: 0.1.0 Summary: Python data types for
 the Apache KafkaÂ® Protocol. Author-email: Anton Agestam
 aiven.io> License: Apache-2.0 license Project-URL: Source Repository, https://
-github.com/Aiven-Open/kio Project-URL: Bug Tracker, https://github.com/Aiven-
-Open/kio/issues Classifier: Intended Audience :: Developers Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.11 Classifier: Programming Language :: Python :: 3.12 Classifier: Typing ::
-Typed Classifier: Topic :: Database Requires-Python: >=3.11 Description-
-Content-Type: text/markdown; charset=UTF-8 License-File: LICENSE License-File:
-NOTICE Requires-Dist: typing-extensions>=4.6.0 Provides-Extra: test Requires-
-Dist: pytest; extra == "test" Requires-Dist: pytest-asyncio; extra == "test"
-Requires-Dist: pytest-icdiff; extra == "test" Requires-Dist: pytest-random-
-order; extra == "test" Requires-Dist: hypothesis>=6.61.0; extra == "test"
-Requires-Dist: coverage; extra == "test" Provides-Extra: codegen Requires-Dist:
+github.com/Aiven-Open/kio Project-URL: Documentation, https://aiven-
+open.github.io/kio/ Project-URL: Bug Tracker, https://github.com/Aiven-Open/
+kio/issues Classifier: Intended Audience :: Developers Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Typing :: Typed Classifier:
+Topic :: Database Requires-Python: >=3.11 Description-Content-Type: text/
+markdown; charset=UTF-8 License-File: LICENSE License-File: NOTICE Requires-
+Dist: typing-extensions>=4.6.0 Provides-Extra: test Requires-Dist: pytest;
+extra == "test" Requires-Dist: pytest-asyncio; extra == "test" Requires-Dist:
+pytest-icdiff; extra == "test" Requires-Dist: pytest-random-order; extra ==
+"test" Requires-Dist: hypothesis>=6.61.0; extra == "test" Requires-Dist:
+coverage; extra == "test" Provides-Extra: codegen Requires-Dist:
 pydantic<2,>=1.10.4; extra == "codegen" Requires-Dist: requests; extra ==
 "codegen" Requires-Dist: pre-commit; extra == "codegen" Provides-Extra: all
 Requires-Dist: kio[test]; extra == "all" Requires-Dist: kio[codegen]; extra ==
 "all"
                                ************ kkiioo ************
                     _[_C_I_ _B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_ _r_e_p_o_r_t_]
                         _[_P_y_P_I_ _P_a_c_k_a_g_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
```

### Comparing `kio-0.0.0a3/README.md` & `kio-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/pyproject.toml` & `kio-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -39,18 +39,19 @@
 all = [
   "kio[test]",
   "kio[codegen]",
 ]
 
 [project.urls]
 "Source Repository" = "https://github.com/Aiven-Open/kio"
+"Documentation" = "https://aiven-open.github.io/kio/"
 "Bug Tracker" = "https://github.com/Aiven-Open/kio/issues"
 
 [build-system]
-requires = ["setuptools>=68.1.2", "wheel"]
+requires = ["setuptools==69.0.3", "wheel==0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.dynamic]
 version = {attr = "kio.__version__"}
@@ -85,14 +86,16 @@
   "java: marks tests validating serialization against a Java process",
 ]
 
 
 [tool.ruff]
 fix = true
 target-version = "py311"
+
+[tool.ruff.lint]
 extend-select = [
   # bugbear
   "B",
   # comprehensions
   "C4",
   # mccabe
   "C90",
@@ -130,25 +133,26 @@
   # Ignore line-length. This is enforced by black, but all cases cannot be handled.
   # Ideally we'd only suppress this in generated files.
   "E501",
   # Allow function calls in argument defaults.
   "B008",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 lines-between-types = 1
 force-single-line = true
 known-first-party = ["kio", "tests", "codegen"]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 10
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "parents"
 
+
 [tool.importlinter]
 root_packages = ["kio", "codegen", "tests"]
 
 [[tool.importlinter.contracts]]
 name = "kio.schema.* does not depend on kio.serial.*"
 type = "forbidden"
 source_modules = "kio.schema"
```

### Comparing `kio-0.0.0a3/src/kio/_utils.py` & `kio-0.1.0/src/kio/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     from functools import cache
 
 
 if TYPE_CHECKING:
     from _typeshed import DataclassInstance
 else:
 
-    class DataclassInstance(Protocol):
-        ...
+    class DataclassInstance(Protocol): ...
```

### Comparing `kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v0/request.py` & `kio-0.1.0/src/kio/schema/add_offsets_to_txn/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v0/response.py` & `kio-0.1.0/src/kio/schema/add_offsets_to_txn/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v1/request.py` & `kio-0.1.0/src/kio/schema/add_offsets_to_txn/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v1/response.py` & `kio-0.1.0/src/kio/schema/add_offsets_to_txn/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v2/request.py` & `kio-0.1.0/src/kio/schema/add_offsets_to_txn/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v2/response.py` & `kio-0.1.0/src/kio/schema/add_offsets_to_txn/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v3/request.py` & `kio-0.1.0/src/kio/schema/add_offsets_to_txn/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_offsets_to_txn/v3/response.py` & `kio-0.1.0/src/kio/schema/add_offsets_to_txn/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v0/request.py` & `kio-0.1.0/src/kio/schema/add_partitions_to_txn/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v0/response.py` & `kio-0.1.0/src/kio/schema/add_partitions_to_txn/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v1/request.py` & `kio-0.1.0/src/kio/schema/add_partitions_to_txn/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v1/response.py` & `kio-0.1.0/src/kio/schema/add_partitions_to_txn/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v2/request.py` & `kio-0.1.0/src/kio/schema/add_partitions_to_txn/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v2/response.py` & `kio-0.1.0/src/kio/schema/add_partitions_to_txn/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v3/request.py` & `kio-0.1.0/src/kio/schema/add_partitions_to_txn/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v3/response.py` & `kio-0.1.0/src/kio/schema/add_partitions_to_txn/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v4/request.py` & `kio-0.1.0/src/kio/schema/add_partitions_to_txn/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/add_partitions_to_txn/v4/response.py` & `kio-0.1.0/src/kio/schema/add_partitions_to_txn/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/allocate_producer_ids/v0/request.py` & `kio-0.1.0/src/kio/schema/allocate_producer_ids/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/allocate_producer_ids/v0/response.py` & `kio-0.1.0/src/kio/schema/allocate_producer_ids/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_client_quotas/v0/request.py` & `kio-0.1.0/src/kio/schema/alter_client_quotas/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_client_quotas/v0/response.py` & `kio-0.1.0/src/kio/schema/alter_client_quotas/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_client_quotas/v1/request.py` & `kio-0.1.0/src/kio/schema/alter_client_quotas/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_client_quotas/v1/response.py` & `kio-0.1.0/src/kio/schema/alter_client_quotas/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_configs/v0/request.py` & `kio-0.1.0/src/kio/schema/alter_configs/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_configs/v0/response.py` & `kio-0.1.0/src/kio/schema/alter_configs/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_configs/v1/request.py` & `kio-0.1.0/src/kio/schema/alter_configs/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_configs/v1/response.py` & `kio-0.1.0/src/kio/schema/alter_configs/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_configs/v2/request.py` & `kio-0.1.0/src/kio/schema/alter_configs/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_configs/v2/response.py` & `kio-0.1.0/src/kio/schema/alter_configs/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_partition/v0/request.py` & `kio-0.1.0/src/kio/schema/alter_partition/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_partition/v0/response.py` & `kio-0.1.0/src/kio/schema/alter_partition/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_partition/v1/request.py` & `kio-0.1.0/src/kio/schema/alter_partition/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_partition/v1/response.py` & `kio-0.1.0/src/kio/schema/alter_partition/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_partition/v2/request.py` & `kio-0.1.0/src/kio/schema/alter_partition/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_partition/v2/response.py` & `kio-0.1.0/src/kio/schema/alter_partition/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_partition/v3/request.py` & `kio-0.1.0/src/kio/schema/alter_partition/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_partition/v3/response.py` & `kio-0.1.0/src/kio/schema/alter_partition/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_partition_reassignments/v0/request.py` & `kio-0.1.0/src/kio/schema/alter_partition_reassignments/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_partition_reassignments/v0/response.py` & `kio-0.1.0/src/kio/schema/alter_partition_reassignments/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v0/request.py` & `kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v0/response.py` & `kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v1/request.py` & `kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v1/response.py` & `kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v2/request.py` & `kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_replica_log_dirs/v2/response.py` & `kio-0.1.0/src/kio/schema/alter_replica_log_dirs/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_user_scram_credentials/v0/request.py` & `kio-0.1.0/src/kio/schema/alter_user_scram_credentials/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/alter_user_scram_credentials/v0/response.py` & `kio-0.1.0/src/kio/schema/alter_user_scram_credentials/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/api_versions/v0/request.py` & `kio-0.1.0/src/kio/schema/api_versions/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/api_versions/v0/response.py` & `kio-0.1.0/src/kio/schema/api_versions/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/api_versions/v1/request.py` & `kio-0.1.0/src/kio/schema/api_versions/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/api_versions/v1/response.py` & `kio-0.1.0/src/kio/schema/api_versions/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/api_versions/v2/request.py` & `kio-0.1.0/src/kio/schema/api_versions/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/api_versions/v2/response.py` & `kio-0.1.0/src/kio/schema/api_versions/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/api_versions/v3/request.py` & `kio-0.1.0/src/kio/schema/api_versions/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/api_versions/v3/response.py` & `kio-0.1.0/src/kio/schema/api_versions/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/begin_quorum_epoch/v0/request.py` & `kio-0.1.0/src/kio/schema/begin_quorum_epoch/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/begin_quorum_epoch/v0/response.py` & `kio-0.1.0/src/kio/schema/begin_quorum_epoch/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/broker_heartbeat/v0/request.py` & `kio-0.1.0/src/kio/schema/broker_heartbeat/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/broker_heartbeat/v0/response.py` & `kio-0.1.0/src/kio/schema/broker_heartbeat/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/broker_registration/v0/request.py` & `kio-0.1.0/src/kio/schema/broker_registration/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/broker_registration/v0/response.py` & `kio-0.1.0/src/kio/schema/broker_registration/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/broker_registration/v1/request.py` & `kio-0.1.0/src/kio/schema/broker_registration/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/broker_registration/v1/response.py` & `kio-0.1.0/src/kio/schema/broker_registration/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/consumer_group_heartbeat/v0/request.py` & `kio-0.1.0/src/kio/schema/consumer_group_heartbeat/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/consumer_group_heartbeat/v0/response.py` & `kio-0.1.0/src/kio/schema/consumer_group_heartbeat/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v0/data.py` & `kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v0/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v1/data.py` & `kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v1/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v2/data.py` & `kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v2/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/consumer_protocol_assignment/v3/data.py` & `kio-0.1.0/src/kio/schema/consumer_protocol_assignment/v3/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v0/data.py` & `kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v0/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v1/data.py` & `kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v1/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v2/data.py` & `kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v2/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/consumer_protocol_subscription/v3/data.py` & `kio-0.1.0/src/kio/schema/consumer_protocol_subscription/v3/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/controlled_shutdown/v0/request.py` & `kio-0.1.0/src/kio/schema/controlled_shutdown/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/controlled_shutdown/v0/response.py` & `kio-0.1.0/src/kio/schema/controlled_shutdown/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/controlled_shutdown/v1/request.py` & `kio-0.1.0/src/kio/schema/controlled_shutdown/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/controlled_shutdown/v1/response.py` & `kio-0.1.0/src/kio/schema/controlled_shutdown/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/controlled_shutdown/v2/request.py` & `kio-0.1.0/src/kio/schema/controlled_shutdown/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/controlled_shutdown/v2/response.py` & `kio-0.1.0/src/kio/schema/controlled_shutdown/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/controlled_shutdown/v3/request.py` & `kio-0.1.0/src/kio/schema/controlled_shutdown/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/controlled_shutdown/v3/response.py` & `kio-0.1.0/src/kio/schema/controlled_shutdown/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_acls/v0/request.py` & `kio-0.1.0/src/kio/schema/create_acls/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_acls/v0/response.py` & `kio-0.1.0/src/kio/schema/create_acls/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_acls/v1/request.py` & `kio-0.1.0/src/kio/schema/create_acls/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_acls/v1/response.py` & `kio-0.1.0/src/kio/schema/create_acls/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_acls/v2/request.py` & `kio-0.1.0/src/kio/schema/create_acls/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_acls/v2/response.py` & `kio-0.1.0/src/kio/schema/create_acls/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_acls/v3/request.py` & `kio-0.1.0/src/kio/schema/create_acls/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_acls/v3/response.py` & `kio-0.1.0/src/kio/schema/create_acls/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_delegation_token/v0/request.py` & `kio-0.1.0/src/kio/schema/create_delegation_token/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_delegation_token/v0/response.py` & `kio-0.1.0/src/kio/schema/create_delegation_token/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_delegation_token/v1/request.py` & `kio-0.1.0/src/kio/schema/create_delegation_token/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_delegation_token/v1/response.py` & `kio-0.1.0/src/kio/schema/create_delegation_token/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_delegation_token/v2/request.py` & `kio-0.1.0/src/kio/schema/create_delegation_token/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_delegation_token/v2/response.py` & `kio-0.1.0/src/kio/schema/create_delegation_token/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_delegation_token/v3/request.py` & `kio-0.1.0/src/kio/schema/create_delegation_token/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_delegation_token/v3/response.py` & `kio-0.1.0/src/kio/schema/create_delegation_token/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_partitions/v0/request.py` & `kio-0.1.0/src/kio/schema/create_partitions/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_partitions/v0/response.py` & `kio-0.1.0/src/kio/schema/create_partitions/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_partitions/v1/request.py` & `kio-0.1.0/src/kio/schema/create_partitions/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_partitions/v1/response.py` & `kio-0.1.0/src/kio/schema/create_partitions/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_partitions/v2/request.py` & `kio-0.1.0/src/kio/schema/create_partitions/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_partitions/v2/response.py` & `kio-0.1.0/src/kio/schema/create_partitions/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_partitions/v3/request.py` & `kio-0.1.0/src/kio/schema/create_partitions/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_partitions/v3/response.py` & `kio-0.1.0/src/kio/schema/create_partitions/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v0/request.py` & `kio-0.1.0/src/kio/schema/create_topics/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v0/response.py` & `kio-0.1.0/src/kio/schema/create_topics/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v1/request.py` & `kio-0.1.0/src/kio/schema/create_topics/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v1/response.py` & `kio-0.1.0/src/kio/schema/create_topics/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v2/request.py` & `kio-0.1.0/src/kio/schema/create_topics/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v2/response.py` & `kio-0.1.0/src/kio/schema/create_topics/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v3/request.py` & `kio-0.1.0/src/kio/schema/create_topics/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v3/response.py` & `kio-0.1.0/src/kio/schema/create_topics/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v4/request.py` & `kio-0.1.0/src/kio/schema/create_topics/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v4/response.py` & `kio-0.1.0/src/kio/schema/create_topics/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v5/request.py` & `kio-0.1.0/src/kio/schema/create_topics/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v5/response.py` & `kio-0.1.0/src/kio/schema/create_topics/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v6/request.py` & `kio-0.1.0/src/kio/schema/create_topics/v6/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v6/response.py` & `kio-0.1.0/src/kio/schema/create_topics/v6/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v7/request.py` & `kio-0.1.0/src/kio/schema/create_topics/v7/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/create_topics/v7/response.py` & `kio-0.1.0/src/kio/schema/create_topics/v7/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/default_principal_data/v0/data.py` & `kio-0.1.0/src/kio/schema/default_principal_data/v0/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_acls/v0/request.py` & `kio-0.1.0/src/kio/schema/delete_acls/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_acls/v0/response.py` & `kio-0.1.0/src/kio/schema/delete_acls/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_acls/v1/request.py` & `kio-0.1.0/src/kio/schema/delete_acls/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_acls/v1/response.py` & `kio-0.1.0/src/kio/schema/delete_acls/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_acls/v2/request.py` & `kio-0.1.0/src/kio/schema/delete_acls/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_acls/v2/response.py` & `kio-0.1.0/src/kio/schema/delete_acls/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_acls/v3/request.py` & `kio-0.1.0/src/kio/schema/delete_acls/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_acls/v3/response.py` & `kio-0.1.0/src/kio/schema/delete_acls/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_groups/v0/request.py` & `kio-0.1.0/src/kio/schema/delete_groups/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_groups/v0/response.py` & `kio-0.1.0/src/kio/schema/delete_groups/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_groups/v1/request.py` & `kio-0.1.0/src/kio/schema/delete_groups/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_groups/v1/response.py` & `kio-0.1.0/src/kio/schema/delete_groups/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_groups/v2/request.py` & `kio-0.1.0/src/kio/schema/delete_groups/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_groups/v2/response.py` & `kio-0.1.0/src/kio/schema/delete_groups/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_records/v0/request.py` & `kio-0.1.0/src/kio/schema/delete_records/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_records/v0/response.py` & `kio-0.1.0/src/kio/schema/delete_records/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_records/v1/request.py` & `kio-0.1.0/src/kio/schema/delete_records/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_records/v1/response.py` & `kio-0.1.0/src/kio/schema/delete_records/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_records/v2/request.py` & `kio-0.1.0/src/kio/schema/delete_records/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_records/v2/response.py` & `kio-0.1.0/src/kio/schema/delete_records/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v0/request.py` & `kio-0.1.0/src/kio/schema/delete_topics/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v0/response.py` & `kio-0.1.0/src/kio/schema/delete_topics/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v1/request.py` & `kio-0.1.0/src/kio/schema/delete_topics/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v1/response.py` & `kio-0.1.0/src/kio/schema/delete_topics/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v2/request.py` & `kio-0.1.0/src/kio/schema/delete_topics/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v2/response.py` & `kio-0.1.0/src/kio/schema/delete_topics/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v3/request.py` & `kio-0.1.0/src/kio/schema/delete_topics/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v3/response.py` & `kio-0.1.0/src/kio/schema/delete_topics/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v4/request.py` & `kio-0.1.0/src/kio/schema/delete_topics/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v4/response.py` & `kio-0.1.0/src/kio/schema/delete_topics/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v5/request.py` & `kio-0.1.0/src/kio/schema/delete_topics/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v5/response.py` & `kio-0.1.0/src/kio/schema/delete_topics/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v6/request.py` & `kio-0.1.0/src/kio/schema/delete_topics/v6/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/delete_topics/v6/response.py` & `kio-0.1.0/src/kio/schema/delete_topics/v6/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_acls/v0/request.py` & `kio-0.1.0/src/kio/schema/describe_acls/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_acls/v0/response.py` & `kio-0.1.0/src/kio/schema/describe_acls/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_acls/v1/request.py` & `kio-0.1.0/src/kio/schema/describe_acls/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_acls/v1/response.py` & `kio-0.1.0/src/kio/schema/describe_acls/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_acls/v2/request.py` & `kio-0.1.0/src/kio/schema/describe_acls/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_acls/v2/response.py` & `kio-0.1.0/src/kio/schema/describe_acls/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_acls/v3/request.py` & `kio-0.1.0/src/kio/schema/describe_acls/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_acls/v3/response.py` & `kio-0.1.0/src/kio/schema/describe_acls/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_client_quotas/v0/request.py` & `kio-0.1.0/src/kio/schema/describe_client_quotas/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_client_quotas/v0/response.py` & `kio-0.1.0/src/kio/schema/describe_client_quotas/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_client_quotas/v1/request.py` & `kio-0.1.0/src/kio/schema/describe_client_quotas/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_client_quotas/v1/response.py` & `kio-0.1.0/src/kio/schema/describe_client_quotas/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_cluster/v0/request.py` & `kio-0.1.0/src/kio/schema/describe_cluster/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_cluster/v0/response.py` & `kio-0.1.0/src/kio/schema/describe_cluster/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_configs/v0/request.py` & `kio-0.1.0/src/kio/schema/describe_configs/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_configs/v0/response.py` & `kio-0.1.0/src/kio/schema/describe_configs/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_configs/v1/request.py` & `kio-0.1.0/src/kio/schema/describe_configs/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_configs/v1/response.py` & `kio-0.1.0/src/kio/schema/describe_configs/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_configs/v2/request.py` & `kio-0.1.0/src/kio/schema/describe_configs/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_configs/v2/response.py` & `kio-0.1.0/src/kio/schema/describe_configs/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_configs/v3/request.py` & `kio-0.1.0/src/kio/schema/describe_configs/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_configs/v3/response.py` & `kio-0.1.0/src/kio/schema/describe_configs/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_configs/v4/request.py` & `kio-0.1.0/src/kio/schema/describe_configs/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_configs/v4/response.py` & `kio-0.1.0/src/kio/schema/describe_configs/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_delegation_token/v0/request.py` & `kio-0.1.0/src/kio/schema/describe_delegation_token/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_delegation_token/v0/response.py` & `kio-0.1.0/src/kio/schema/describe_delegation_token/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_delegation_token/v1/request.py` & `kio-0.1.0/src/kio/schema/describe_delegation_token/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_delegation_token/v1/response.py` & `kio-0.1.0/src/kio/schema/describe_delegation_token/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_delegation_token/v2/request.py` & `kio-0.1.0/src/kio/schema/describe_delegation_token/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_delegation_token/v2/response.py` & `kio-0.1.0/src/kio/schema/describe_delegation_token/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_delegation_token/v3/request.py` & `kio-0.1.0/src/kio/schema/describe_delegation_token/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_delegation_token/v3/response.py` & `kio-0.1.0/src/kio/schema/describe_delegation_token/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v0/request.py` & `kio-0.1.0/src/kio/schema/describe_groups/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v0/response.py` & `kio-0.1.0/src/kio/schema/describe_groups/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v1/request.py` & `kio-0.1.0/src/kio/schema/describe_groups/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v1/response.py` & `kio-0.1.0/src/kio/schema/describe_groups/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v2/request.py` & `kio-0.1.0/src/kio/schema/describe_groups/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v2/response.py` & `kio-0.1.0/src/kio/schema/describe_groups/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v3/request.py` & `kio-0.1.0/src/kio/schema/describe_groups/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v3/response.py` & `kio-0.1.0/src/kio/schema/describe_groups/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v4/request.py` & `kio-0.1.0/src/kio/schema/describe_groups/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v4/response.py` & `kio-0.1.0/src/kio/schema/describe_groups/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v5/request.py` & `kio-0.1.0/src/kio/schema/describe_groups/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_groups/v5/response.py` & `kio-0.1.0/src/kio/schema/describe_groups/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_log_dirs/v0/request.py` & `kio-0.1.0/src/kio/schema/describe_log_dirs/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_log_dirs/v0/response.py` & `kio-0.1.0/src/kio/schema/describe_log_dirs/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_log_dirs/v1/request.py` & `kio-0.1.0/src/kio/schema/describe_log_dirs/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_log_dirs/v1/response.py` & `kio-0.1.0/src/kio/schema/describe_log_dirs/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_log_dirs/v2/request.py` & `kio-0.1.0/src/kio/schema/describe_log_dirs/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_log_dirs/v2/response.py` & `kio-0.1.0/src/kio/schema/describe_log_dirs/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_log_dirs/v3/request.py` & `kio-0.1.0/src/kio/schema/describe_log_dirs/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_log_dirs/v3/response.py` & `kio-0.1.0/src/kio/schema/describe_log_dirs/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_log_dirs/v4/request.py` & `kio-0.1.0/src/kio/schema/describe_log_dirs/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_log_dirs/v4/response.py` & `kio-0.1.0/src/kio/schema/describe_log_dirs/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_producers/v0/request.py` & `kio-0.1.0/src/kio/schema/describe_producers/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_producers/v0/response.py` & `kio-0.1.0/src/kio/schema/describe_producers/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_quorum/v0/request.py` & `kio-0.1.0/src/kio/schema/describe_quorum/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_quorum/v0/response.py` & `kio-0.1.0/src/kio/schema/describe_quorum/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_quorum/v1/request.py` & `kio-0.1.0/src/kio/schema/describe_quorum/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_quorum/v1/response.py` & `kio-0.1.0/src/kio/schema/describe_quorum/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_transactions/v0/request.py` & `kio-0.1.0/src/kio/schema/describe_transactions/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_transactions/v0/response.py` & `kio-0.1.0/src/kio/schema/describe_transactions/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_user_scram_credentials/v0/request.py` & `kio-0.1.0/src/kio/schema/describe_user_scram_credentials/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/describe_user_scram_credentials/v0/response.py` & `kio-0.1.0/src/kio/schema/describe_user_scram_credentials/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/elect_leaders/v0/request.py` & `kio-0.1.0/src/kio/schema/elect_leaders/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/elect_leaders/v0/response.py` & `kio-0.1.0/src/kio/schema/elect_leaders/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/elect_leaders/v1/request.py` & `kio-0.1.0/src/kio/schema/elect_leaders/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/elect_leaders/v1/response.py` & `kio-0.1.0/src/kio/schema/elect_leaders/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/elect_leaders/v2/request.py` & `kio-0.1.0/src/kio/schema/elect_leaders/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/elect_leaders/v2/response.py` & `kio-0.1.0/src/kio/schema/elect_leaders/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/end_quorum_epoch/v0/request.py` & `kio-0.1.0/src/kio/schema/end_quorum_epoch/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/end_quorum_epoch/v0/response.py` & `kio-0.1.0/src/kio/schema/end_quorum_epoch/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/end_txn/v0/request.py` & `kio-0.1.0/src/kio/schema/end_txn/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/end_txn/v0/response.py` & `kio-0.1.0/src/kio/schema/end_txn/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/end_txn/v1/request.py` & `kio-0.1.0/src/kio/schema/end_txn/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/end_txn/v1/response.py` & `kio-0.1.0/src/kio/schema/end_txn/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/end_txn/v2/request.py` & `kio-0.1.0/src/kio/schema/end_txn/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/end_txn/v2/response.py` & `kio-0.1.0/src/kio/schema/end_txn/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/end_txn/v3/request.py` & `kio-0.1.0/src/kio/schema/end_txn/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/end_txn/v3/response.py` & `kio-0.1.0/src/kio/schema/end_txn/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/envelope/v0/request.py` & `kio-0.1.0/src/kio/schema/envelope/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/envelope/v0/response.py` & `kio-0.1.0/src/kio/schema/envelope/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/expire_delegation_token/v0/request.py` & `kio-0.1.0/src/kio/schema/expire_delegation_token/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/expire_delegation_token/v0/response.py` & `kio-0.1.0/src/kio/schema/expire_delegation_token/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/expire_delegation_token/v1/request.py` & `kio-0.1.0/src/kio/schema/expire_delegation_token/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/expire_delegation_token/v1/response.py` & `kio-0.1.0/src/kio/schema/expire_delegation_token/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/expire_delegation_token/v2/request.py` & `kio-0.1.0/src/kio/schema/expire_delegation_token/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/expire_delegation_token/v2/response.py` & `kio-0.1.0/src/kio/schema/expire_delegation_token/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v0/request.py` & `kio-0.1.0/src/kio/schema/fetch/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v0/response.py` & `kio-0.1.0/src/kio/schema/fetch/v0/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionData:
@@ -26,15 +27,15 @@
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     partition_index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
     error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
     """The error code, or 0 if there was no fetch error."""
     high_watermark: i64 = field(metadata={"kafka_type": "int64"})
     """The current high water mark."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(0)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v1/request.py` & `kio-0.1.0/src/kio/schema/fetch/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v1/response.py` & `kio-0.1.0/src/kio/schema/fetch/v1/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -27,15 +28,15 @@
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     partition_index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
     error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
     """The error code, or 0 if there was no fetch error."""
     high_watermark: i64 = field(metadata={"kafka_type": "int64"})
     """The current high water mark."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(1)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v10/request.py` & `kio-0.1.0/src/kio/schema/fetch/v10/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v10/response.py` & `kio-0.1.0/src/kio/schema/fetch/v6/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,37 +9,38 @@
 from typing import ClassVar
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import ProducerId
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class AbortedTransaction:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(10)
+    __version__: ClassVar[i16] = i16(6)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     producer_id: ProducerId = field(metadata={"kafka_type": "int64"})
     """The producer id associated with the aborted transaction."""
     first_offset: i64 = field(metadata={"kafka_type": "int64"})
     """The first offset in the aborted transaction."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(10)
+    __version__: ClassVar[i16] = i16(6)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     partition_index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
     error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
     """The error code, or 0 if there was no fetch error."""
@@ -47,39 +48,35 @@
     """The current high water mark."""
     last_stable_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The last stable offset (or LSO) of the partition. This is the last offset such that the state of all transactional records prior to this offset have been decided (ABORTED or COMMITTED)"""
     log_start_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The current log start offset."""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(10)
+    __version__: ClassVar[i16] = i16(6)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     topic: TopicName = field(metadata={"kafka_type": "string"})
     """The topic name."""
     partitions: tuple[PartitionData, ...]
     """The topic partitions."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchResponse:
     __type__: ClassVar = EntityType.response
-    __version__: ClassVar[i16] = i16(10)
+    __version__: ClassVar[i16] = i16(6)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     throttle_time: i32Timedelta = field(metadata={"kafka_type": "timedelta_i32"})
     """The duration in milliseconds for which the request was throttled due to a quota violation, or zero if the request did not violate any quota."""
-    error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
-    """The top level response error code."""
-    session_id: i32 = field(metadata={"kafka_type": "int32"}, default=i32(0))
-    """The fetch session ID, or 0 if this is not part of a fetch session."""
     responses: tuple[FetchableTopicResponse, ...]
     """The response topics."""
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v11/request.py` & `kio-0.1.0/src/kio/schema/fetch/v11/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v11/response.py` & `kio-0.1.0/src/kio/schema/fetch/v11/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import BrokerId
 from kio.schema.types import ProducerId
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -52,15 +53,15 @@
     """The current log start offset."""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
     preferred_read_replica: BrokerId = field(
         metadata={"kafka_type": "int32"}, default=BrokerId(-1)
     )
     """The preferred read replica for the consumer to use on its next fetch request"""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(11)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v12/request.py` & `kio-0.1.0/src/kio/schema/fetch/v12/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v12/response.py` & `kio-0.1.0/src/kio/schema/fetch/v12/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from kio.schema.response_header.v1.header import ResponseHeader
 from kio.schema.types import BrokerId
 from kio.schema.types import ProducerId
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -96,15 +97,15 @@
     """In the case of fetching an offset less than the LogStartOffset, this is the end offset and epoch that should be used in the FetchSnapshot request."""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
     preferred_read_replica: BrokerId = field(
         metadata={"kafka_type": "int32"}, default=BrokerId(-1)
     )
     """The preferred read replica for the consumer to use on its next fetch request"""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(12)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v13/request.py` & `kio-0.1.0/src/kio/schema/fetch/v13/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v13/response.py` & `kio-0.1.0/src/kio/schema/fetch/v13/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import ClassVar
 
 from kio.schema.response_header.v1.header import ResponseHeader
 from kio.schema.types import BrokerId
 from kio.schema.types import ProducerId
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -97,15 +98,15 @@
     """In the case of fetching an offset less than the LogStartOffset, this is the end offset and epoch that should be used in the FetchSnapshot request."""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
     preferred_read_replica: BrokerId = field(
         metadata={"kafka_type": "int32"}, default=BrokerId(-1)
     )
     """The preferred read replica for the consumer to use on its next fetch request"""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(13)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v14/request.py` & `kio-0.1.0/src/kio/schema/fetch/v14/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v14/response.py` & `kio-0.1.0/src/kio/schema/fetch/v15/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,72 +11,73 @@
 from typing import ClassVar
 
 from kio.schema.response_header.v1.header import ResponseHeader
 from kio.schema.types import BrokerId
 from kio.schema.types import ProducerId
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class EpochEndOffset:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(14)
+    __version__: ClassVar[i16] = i16(15)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     epoch: i32 = field(metadata={"kafka_type": "int32"}, default=i32(-1))
     end_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class LeaderIdAndEpoch:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(14)
+    __version__: ClassVar[i16] = i16(15)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     leader_id: BrokerId = field(metadata={"kafka_type": "int32"}, default=BrokerId(-1))
     """The ID of the current leader or -1 if the leader is unknown."""
     leader_epoch: i32 = field(metadata={"kafka_type": "int32"}, default=i32(-1))
     """The latest known leader epoch"""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class SnapshotId:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(14)
+    __version__: ClassVar[i16] = i16(15)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     end_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     epoch: i32 = field(metadata={"kafka_type": "int32"}, default=i32(-1))
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class AbortedTransaction:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(14)
+    __version__: ClassVar[i16] = i16(15)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     producer_id: ProducerId = field(metadata={"kafka_type": "int64"})
     """The producer id associated with the aborted transaction."""
     first_offset: i64 = field(metadata={"kafka_type": "int64"})
     """The first offset in the aborted transaction."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(14)
+    __version__: ClassVar[i16] = i16(15)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     partition_index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
     error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
     """The error code, or 0 if there was no fetch error."""
@@ -97,35 +98,35 @@
     """In the case of fetching an offset less than the LogStartOffset, this is the end offset and epoch that should be used in the FetchSnapshot request."""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
     preferred_read_replica: BrokerId = field(
         metadata={"kafka_type": "int32"}, default=BrokerId(-1)
     )
     """The preferred read replica for the consumer to use on its next fetch request"""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(14)
+    __version__: ClassVar[i16] = i16(15)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     topic_id: uuid.UUID | None = field(metadata={"kafka_type": "uuid"})
     """The unique topic ID"""
     partitions: tuple[PartitionData, ...]
     """The topic partitions."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchResponse:
     __type__: ClassVar = EntityType.response
-    __version__: ClassVar[i16] = i16(14)
+    __version__: ClassVar[i16] = i16(15)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     throttle_time: i32Timedelta = field(metadata={"kafka_type": "timedelta_i32"})
     """The duration in milliseconds for which the request was throttled due to a quota violation, or zero if the request did not violate any quota."""
     error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
     """The top level response error code."""
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v15/request.py` & `kio-0.1.0/src/kio/schema/fetch/v15/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v15/response.py` & `kio-0.1.0/src/kio/schema/fetch/v14/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,72 +11,73 @@
 from typing import ClassVar
 
 from kio.schema.response_header.v1.header import ResponseHeader
 from kio.schema.types import BrokerId
 from kio.schema.types import ProducerId
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class EpochEndOffset:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(15)
+    __version__: ClassVar[i16] = i16(14)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     epoch: i32 = field(metadata={"kafka_type": "int32"}, default=i32(-1))
     end_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class LeaderIdAndEpoch:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(15)
+    __version__: ClassVar[i16] = i16(14)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     leader_id: BrokerId = field(metadata={"kafka_type": "int32"}, default=BrokerId(-1))
     """The ID of the current leader or -1 if the leader is unknown."""
     leader_epoch: i32 = field(metadata={"kafka_type": "int32"}, default=i32(-1))
     """The latest known leader epoch"""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class SnapshotId:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(15)
+    __version__: ClassVar[i16] = i16(14)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     end_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     epoch: i32 = field(metadata={"kafka_type": "int32"}, default=i32(-1))
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class AbortedTransaction:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(15)
+    __version__: ClassVar[i16] = i16(14)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     producer_id: ProducerId = field(metadata={"kafka_type": "int64"})
     """The producer id associated with the aborted transaction."""
     first_offset: i64 = field(metadata={"kafka_type": "int64"})
     """The first offset in the aborted transaction."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(15)
+    __version__: ClassVar[i16] = i16(14)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     partition_index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
     error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
     """The error code, or 0 if there was no fetch error."""
@@ -97,35 +98,35 @@
     """In the case of fetching an offset less than the LogStartOffset, this is the end offset and epoch that should be used in the FetchSnapshot request."""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
     preferred_read_replica: BrokerId = field(
         metadata={"kafka_type": "int32"}, default=BrokerId(-1)
     )
     """The preferred read replica for the consumer to use on its next fetch request"""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(15)
+    __version__: ClassVar[i16] = i16(14)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     topic_id: uuid.UUID | None = field(metadata={"kafka_type": "uuid"})
     """The unique topic ID"""
     partitions: tuple[PartitionData, ...]
     """The topic partitions."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchResponse:
     __type__: ClassVar = EntityType.response
-    __version__: ClassVar[i16] = i16(15)
+    __version__: ClassVar[i16] = i16(14)
     __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     throttle_time: i32Timedelta = field(metadata={"kafka_type": "timedelta_i32"})
     """The duration in milliseconds for which the request was throttled due to a quota violation, or zero if the request did not violate any quota."""
     error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
     """The top level response error code."""
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v2/request.py` & `kio-0.1.0/src/kio/schema/fetch/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v2/response.py` & `kio-0.1.0/src/kio/schema/fetch/v2/response.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -27,15 +28,15 @@
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     partition_index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
     error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
     """The error code, or 0 if there was no fetch error."""
     high_watermark: i64 = field(metadata={"kafka_type": "int64"})
     """The current high water mark."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(2)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v3/request.py` & `kio-0.1.0/src/kio/schema/fetch/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v3/response.py` & `kio-0.1.0/src/kio/schema/fetch/v3/response.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -27,15 +28,15 @@
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     partition_index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
     error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
     """The error code, or 0 if there was no fetch error."""
     high_watermark: i64 = field(metadata={"kafka_type": "int64"})
     """The current high water mark."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(3)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v4/request.py` & `kio-0.1.0/src/kio/schema/fetch/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v4/response.py` & `kio-0.1.0/src/kio/schema/fetch/v4/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import ClassVar
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import ProducerId
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -45,15 +46,15 @@
     """The error code, or 0 if there was no fetch error."""
     high_watermark: i64 = field(metadata={"kafka_type": "int64"})
     """The current high water mark."""
     last_stable_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The last stable offset (or LSO) of the partition. This is the last offset such that the state of all transactional records prior to this offset have been decided (ABORTED or COMMITTED)"""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(4)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v5/request.py` & `kio-0.1.0/src/kio/schema/fetch/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v5/response.py` & `kio-0.1.0/src/kio/schema/fetch/v5/response.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import ClassVar
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import ProducerId
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -47,15 +48,15 @@
     """The current high water mark."""
     last_stable_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The last stable offset (or LSO) of the partition. This is the last offset such that the state of all transactional records prior to this offset have been decided (ABORTED or COMMITTED)"""
     log_start_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The current log start offset."""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(5)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v6/request.py` & `kio-0.1.0/src/kio/schema/fetch/v6/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v6/response.py` & `kio-0.1.0/src/kio/schema/fetch/v10/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,37 +9,38 @@
 from typing import ClassVar
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import ProducerId
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class AbortedTransaction:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(6)
+    __version__: ClassVar[i16] = i16(10)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     producer_id: ProducerId = field(metadata={"kafka_type": "int64"})
     """The producer id associated with the aborted transaction."""
     first_offset: i64 = field(metadata={"kafka_type": "int64"})
     """The first offset in the aborted transaction."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(6)
+    __version__: ClassVar[i16] = i16(10)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     partition_index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
     error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
     """The error code, or 0 if there was no fetch error."""
@@ -47,35 +48,39 @@
     """The current high water mark."""
     last_stable_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The last stable offset (or LSO) of the partition. This is the last offset such that the state of all transactional records prior to this offset have been decided (ABORTED or COMMITTED)"""
     log_start_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The current log start offset."""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(6)
+    __version__: ClassVar[i16] = i16(10)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     topic: TopicName = field(metadata={"kafka_type": "string"})
     """The topic name."""
     partitions: tuple[PartitionData, ...]
     """The topic partitions."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchResponse:
     __type__: ClassVar = EntityType.response
-    __version__: ClassVar[i16] = i16(6)
+    __version__: ClassVar[i16] = i16(10)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(1)
     __header_schema__: ClassVar[type[ResponseHeader]] = ResponseHeader
     throttle_time: i32Timedelta = field(metadata={"kafka_type": "timedelta_i32"})
     """The duration in milliseconds for which the request was throttled due to a quota violation, or zero if the request did not violate any quota."""
+    error_code: ErrorCode = field(metadata={"kafka_type": "error_code"})
+    """The top level response error code."""
+    session_id: i32 = field(metadata={"kafka_type": "int32"}, default=i32(0))
+    """The fetch session ID, or 0 if this is not part of a fetch session."""
     responses: tuple[FetchableTopicResponse, ...]
     """The response topics."""
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v7/request.py` & `kio-0.1.0/src/kio/schema/fetch/v7/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v7/response.py` & `kio-0.1.0/src/kio/schema/fetch/v7/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import ClassVar
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import ProducerId
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -47,15 +48,15 @@
     """The current high water mark."""
     last_stable_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The last stable offset (or LSO) of the partition. This is the last offset such that the state of all transactional records prior to this offset have been decided (ABORTED or COMMITTED)"""
     log_start_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The current log start offset."""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(7)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v8/request.py` & `kio-0.1.0/src/kio/schema/fetch/v8/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v8/response.py` & `kio-0.1.0/src/kio/schema/fetch/v8/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import ClassVar
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import ProducerId
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -47,15 +48,15 @@
     """The current high water mark."""
     last_stable_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The last stable offset (or LSO) of the partition. This is the last offset such that the state of all transactional records prior to this offset have been decided (ABORTED or COMMITTED)"""
     log_start_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The current log start offset."""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(8)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v9/request.py` & `kio-0.1.0/src/kio/schema/fetch/v9/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch/v9/response.py` & `kio-0.1.0/src/kio/schema/fetch/v9/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import ClassVar
 
 from kio.schema.response_header.v0.header import ResponseHeader
 from kio.schema.types import ProducerId
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -47,15 +48,15 @@
     """The current high water mark."""
     last_stable_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The last stable offset (or LSO) of the partition. This is the last offset such that the state of all transactional records prior to this offset have been decided (ABORTED or COMMITTED)"""
     log_start_offset: i64 = field(metadata={"kafka_type": "int64"}, default=i64(-1))
     """The current log start offset."""
     aborted_transactions: tuple[AbortedTransaction, ...] | None
     """The aborted transactions."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class FetchableTopicResponse:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(9)
```

### Comparing `kio-0.0.0a3/src/kio/schema/fetch_snapshot/v0/request.py` & `kio-0.1.0/src/kio/schema/fetch_snapshot/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/fetch_snapshot/v0/response.py` & `kio-0.1.0/src/kio/schema/fetch_snapshot/v0/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import ClassVar
 
 from kio.schema.response_header.v1.header import ResponseHeader
 from kio.schema.types import BrokerId
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
 from kio.static.constants import ErrorCode
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 from kio.static.primitive import i64
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
@@ -57,15 +58,15 @@
     snapshot_id: SnapshotId
     """The snapshot endOffset and epoch fetched"""
     current_leader: LeaderIdAndEpoch = field(metadata={"tag": 0})
     size: i64 = field(metadata={"kafka_type": "int64"})
     """The total size of the snapshot."""
     position: i64 = field(metadata={"kafka_type": "int64"})
     """The starting byte position within the snapshot included in the Bytes field."""
-    unaligned_records: bytes = field(metadata={"kafka_type": "records"})
+    unaligned_records: Records = field(metadata={"kafka_type": "records"})
     """Snapshot data in records format which may not be aligned on an offset boundary"""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class TopicSnapshot:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(0)
```

### Comparing `kio-0.0.0a3/src/kio/schema/find_coordinator/v0/request.py` & `kio-0.1.0/src/kio/schema/find_coordinator/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/find_coordinator/v0/response.py` & `kio-0.1.0/src/kio/schema/find_coordinator/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/find_coordinator/v1/request.py` & `kio-0.1.0/src/kio/schema/find_coordinator/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/find_coordinator/v1/response.py` & `kio-0.1.0/src/kio/schema/find_coordinator/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/find_coordinator/v2/request.py` & `kio-0.1.0/src/kio/schema/find_coordinator/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/find_coordinator/v2/response.py` & `kio-0.1.0/src/kio/schema/find_coordinator/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/find_coordinator/v3/request.py` & `kio-0.1.0/src/kio/schema/find_coordinator/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/find_coordinator/v3/response.py` & `kio-0.1.0/src/kio/schema/find_coordinator/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/find_coordinator/v4/request.py` & `kio-0.1.0/src/kio/schema/find_coordinator/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/find_coordinator/v4/response.py` & `kio-0.1.0/src/kio/schema/find_coordinator/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/heartbeat/v0/request.py` & `kio-0.1.0/src/kio/schema/heartbeat/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/heartbeat/v0/response.py` & `kio-0.1.0/src/kio/schema/heartbeat/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/heartbeat/v1/request.py` & `kio-0.1.0/src/kio/schema/heartbeat/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/heartbeat/v1/response.py` & `kio-0.1.0/src/kio/schema/heartbeat/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/heartbeat/v2/request.py` & `kio-0.1.0/src/kio/schema/heartbeat/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/heartbeat/v2/response.py` & `kio-0.1.0/src/kio/schema/heartbeat/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/heartbeat/v3/request.py` & `kio-0.1.0/src/kio/schema/heartbeat/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/heartbeat/v3/response.py` & `kio-0.1.0/src/kio/schema/heartbeat/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/heartbeat/v4/request.py` & `kio-0.1.0/src/kio/schema/heartbeat/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/heartbeat/v4/response.py` & `kio-0.1.0/src/kio/schema/heartbeat/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v0/request.py` & `kio-0.1.0/src/kio/schema/incremental_alter_configs/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v0/response.py` & `kio-0.1.0/src/kio/schema/incremental_alter_configs/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v1/request.py` & `kio-0.1.0/src/kio/schema/incremental_alter_configs/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/incremental_alter_configs/v1/response.py` & `kio-0.1.0/src/kio/schema/incremental_alter_configs/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/init_producer_id/v0/request.py` & `kio-0.1.0/src/kio/schema/init_producer_id/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/init_producer_id/v0/response.py` & `kio-0.1.0/src/kio/schema/init_producer_id/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/init_producer_id/v1/request.py` & `kio-0.1.0/src/kio/schema/init_producer_id/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/init_producer_id/v1/response.py` & `kio-0.1.0/src/kio/schema/init_producer_id/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/init_producer_id/v2/request.py` & `kio-0.1.0/src/kio/schema/init_producer_id/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/init_producer_id/v2/response.py` & `kio-0.1.0/src/kio/schema/init_producer_id/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/init_producer_id/v3/request.py` & `kio-0.1.0/src/kio/schema/init_producer_id/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/init_producer_id/v3/response.py` & `kio-0.1.0/src/kio/schema/init_producer_id/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/init_producer_id/v4/request.py` & `kio-0.1.0/src/kio/schema/init_producer_id/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/init_producer_id/v4/response.py` & `kio-0.1.0/src/kio/schema/init_producer_id/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v0/request.py` & `kio-0.1.0/src/kio/schema/join_group/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v0/response.py` & `kio-0.1.0/src/kio/schema/join_group/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v1/request.py` & `kio-0.1.0/src/kio/schema/join_group/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v1/response.py` & `kio-0.1.0/src/kio/schema/join_group/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v2/request.py` & `kio-0.1.0/src/kio/schema/join_group/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v2/response.py` & `kio-0.1.0/src/kio/schema/join_group/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v3/request.py` & `kio-0.1.0/src/kio/schema/join_group/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v3/response.py` & `kio-0.1.0/src/kio/schema/join_group/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v4/request.py` & `kio-0.1.0/src/kio/schema/join_group/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v4/response.py` & `kio-0.1.0/src/kio/schema/join_group/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v5/request.py` & `kio-0.1.0/src/kio/schema/join_group/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v5/response.py` & `kio-0.1.0/src/kio/schema/join_group/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v6/request.py` & `kio-0.1.0/src/kio/schema/join_group/v6/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v6/response.py` & `kio-0.1.0/src/kio/schema/join_group/v6/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v7/request.py` & `kio-0.1.0/src/kio/schema/join_group/v7/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v7/response.py` & `kio-0.1.0/src/kio/schema/join_group/v7/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v8/request.py` & `kio-0.1.0/src/kio/schema/join_group/v8/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v8/response.py` & `kio-0.1.0/src/kio/schema/join_group/v8/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v9/request.py` & `kio-0.1.0/src/kio/schema/join_group/v9/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/join_group/v9/response.py` & `kio-0.1.0/src/kio/schema/join_group/v9/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v0/request.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v0/response.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v1/request.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v1/response.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v2/request.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v2/response.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v3/request.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v3/response.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v4/request.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v4/response.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v5/request.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v5/response.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v6/request.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v6/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v6/response.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v6/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v7/request.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v7/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_and_isr/v7/response.py` & `kio-0.1.0/src/kio/schema/leader_and_isr/v7/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leader_change_message/v0/data.py` & `kio-0.1.0/src/kio/schema/leader_change_message/v0/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v0/request.py` & `kio-0.1.0/src/kio/schema/leave_group/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v0/response.py` & `kio-0.1.0/src/kio/schema/leave_group/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v1/request.py` & `kio-0.1.0/src/kio/schema/leave_group/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v1/response.py` & `kio-0.1.0/src/kio/schema/leave_group/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v2/request.py` & `kio-0.1.0/src/kio/schema/leave_group/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v2/response.py` & `kio-0.1.0/src/kio/schema/leave_group/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v3/request.py` & `kio-0.1.0/src/kio/schema/leave_group/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v3/response.py` & `kio-0.1.0/src/kio/schema/leave_group/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v4/request.py` & `kio-0.1.0/src/kio/schema/leave_group/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v4/response.py` & `kio-0.1.0/src/kio/schema/leave_group/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v5/request.py` & `kio-0.1.0/src/kio/schema/leave_group/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/leave_group/v5/response.py` & `kio-0.1.0/src/kio/schema/leave_group/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_groups/v0/request.py` & `kio-0.1.0/src/kio/schema/list_groups/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_groups/v0/response.py` & `kio-0.1.0/src/kio/schema/list_groups/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_groups/v1/request.py` & `kio-0.1.0/src/kio/schema/list_groups/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_groups/v1/response.py` & `kio-0.1.0/src/kio/schema/list_groups/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_groups/v2/request.py` & `kio-0.1.0/src/kio/schema/list_groups/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_groups/v2/response.py` & `kio-0.1.0/src/kio/schema/list_groups/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_groups/v3/request.py` & `kio-0.1.0/src/kio/schema/list_groups/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_groups/v3/response.py` & `kio-0.1.0/src/kio/schema/list_groups/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_groups/v4/request.py` & `kio-0.1.0/src/kio/schema/list_groups/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_groups/v4/response.py` & `kio-0.1.0/src/kio/schema/list_groups/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v0/request.py` & `kio-0.1.0/src/kio/schema/list_offsets/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v0/response.py` & `kio-0.1.0/src/kio/schema/list_offsets/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v1/request.py` & `kio-0.1.0/src/kio/schema/list_offsets/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v1/response.py` & `kio-0.1.0/src/kio/schema/list_offsets/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v2/request.py` & `kio-0.1.0/src/kio/schema/list_offsets/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v2/response.py` & `kio-0.1.0/src/kio/schema/list_offsets/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v3/request.py` & `kio-0.1.0/src/kio/schema/list_offsets/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v3/response.py` & `kio-0.1.0/src/kio/schema/list_offsets/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v4/request.py` & `kio-0.1.0/src/kio/schema/list_offsets/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v4/response.py` & `kio-0.1.0/src/kio/schema/list_offsets/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v5/request.py` & `kio-0.1.0/src/kio/schema/list_offsets/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v5/response.py` & `kio-0.1.0/src/kio/schema/list_offsets/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v6/request.py` & `kio-0.1.0/src/kio/schema/list_offsets/v6/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v6/response.py` & `kio-0.1.0/src/kio/schema/list_offsets/v6/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v7/request.py` & `kio-0.1.0/src/kio/schema/list_offsets/v7/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v7/response.py` & `kio-0.1.0/src/kio/schema/list_offsets/v7/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v8/request.py` & `kio-0.1.0/src/kio/schema/list_offsets/v8/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_offsets/v8/response.py` & `kio-0.1.0/src/kio/schema/list_offsets/v8/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_partition_reassignments/v0/request.py` & `kio-0.1.0/src/kio/schema/list_partition_reassignments/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_partition_reassignments/v0/response.py` & `kio-0.1.0/src/kio/schema/list_partition_reassignments/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_transactions/v0/request.py` & `kio-0.1.0/src/kio/schema/list_transactions/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/list_transactions/v0/response.py` & `kio-0.1.0/src/kio/schema/list_transactions/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v0/request.py` & `kio-0.1.0/src/kio/schema/metadata/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v0/response.py` & `kio-0.1.0/src/kio/schema/metadata/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v1/request.py` & `kio-0.1.0/src/kio/schema/metadata/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v1/response.py` & `kio-0.1.0/src/kio/schema/metadata/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v10/request.py` & `kio-0.1.0/src/kio/schema/metadata/v10/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v10/response.py` & `kio-0.1.0/src/kio/schema/metadata/v10/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v11/request.py` & `kio-0.1.0/src/kio/schema/metadata/v11/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v11/response.py` & `kio-0.1.0/src/kio/schema/metadata/v11/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v12/request.py` & `kio-0.1.0/src/kio/schema/metadata/v12/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v12/response.py` & `kio-0.1.0/src/kio/schema/metadata/v12/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v2/request.py` & `kio-0.1.0/src/kio/schema/metadata/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v2/response.py` & `kio-0.1.0/src/kio/schema/metadata/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v3/request.py` & `kio-0.1.0/src/kio/schema/metadata/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v3/response.py` & `kio-0.1.0/src/kio/schema/metadata/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v4/request.py` & `kio-0.1.0/src/kio/schema/metadata/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v4/response.py` & `kio-0.1.0/src/kio/schema/metadata/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v5/request.py` & `kio-0.1.0/src/kio/schema/metadata/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v5/response.py` & `kio-0.1.0/src/kio/schema/metadata/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v6/request.py` & `kio-0.1.0/src/kio/schema/metadata/v6/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v6/response.py` & `kio-0.1.0/src/kio/schema/metadata/v6/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v7/request.py` & `kio-0.1.0/src/kio/schema/metadata/v7/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v7/response.py` & `kio-0.1.0/src/kio/schema/metadata/v7/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v8/request.py` & `kio-0.1.0/src/kio/schema/metadata/v8/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v8/response.py` & `kio-0.1.0/src/kio/schema/metadata/v8/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v9/request.py` & `kio-0.1.0/src/kio/schema/metadata/v9/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/metadata/v9/response.py` & `kio-0.1.0/src/kio/schema/metadata/v9/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v0/request.py` & `kio-0.1.0/src/kio/schema/offset_commit/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v0/response.py` & `kio-0.1.0/src/kio/schema/offset_commit/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v1/request.py` & `kio-0.1.0/src/kio/schema/offset_commit/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v1/response.py` & `kio-0.1.0/src/kio/schema/offset_commit/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v2/request.py` & `kio-0.1.0/src/kio/schema/offset_commit/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v2/response.py` & `kio-0.1.0/src/kio/schema/offset_commit/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v3/request.py` & `kio-0.1.0/src/kio/schema/offset_commit/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v3/response.py` & `kio-0.1.0/src/kio/schema/offset_commit/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v4/request.py` & `kio-0.1.0/src/kio/schema/offset_commit/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v4/response.py` & `kio-0.1.0/src/kio/schema/offset_commit/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v5/request.py` & `kio-0.1.0/src/kio/schema/offset_commit/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v5/response.py` & `kio-0.1.0/src/kio/schema/offset_commit/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v6/request.py` & `kio-0.1.0/src/kio/schema/offset_commit/v6/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v6/response.py` & `kio-0.1.0/src/kio/schema/offset_commit/v6/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v7/request.py` & `kio-0.1.0/src/kio/schema/offset_commit/v7/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v7/response.py` & `kio-0.1.0/src/kio/schema/offset_commit/v7/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v8/request.py` & `kio-0.1.0/src/kio/schema/offset_commit/v8/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v8/response.py` & `kio-0.1.0/src/kio/schema/offset_commit/v8/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v9/request.py` & `kio-0.1.0/src/kio/schema/offset_commit/v9/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_commit/v9/response.py` & `kio-0.1.0/src/kio/schema/offset_commit/v9/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_delete/v0/request.py` & `kio-0.1.0/src/kio/schema/offset_delete/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_delete/v0/response.py` & `kio-0.1.0/src/kio/schema/offset_delete/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v0/request.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v0/response.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v1/request.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v1/response.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v2/request.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v2/response.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v3/request.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v3/response.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v4/request.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v4/response.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v5/request.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v5/response.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v6/request.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v6/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v6/response.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v6/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v7/request.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v7/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v7/response.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v7/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v8/request.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v8/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_fetch/v8/response.py` & `kio-0.1.0/src/kio/schema/offset_fetch/v8/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v0/request.py` & `kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v0/response.py` & `kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v1/request.py` & `kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v1/response.py` & `kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v2/request.py` & `kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v2/response.py` & `kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v3/request.py` & `kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v3/response.py` & `kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v4/request.py` & `kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/offset_for_leader_epoch/v4/response.py` & `kio-0.1.0/src/kio/schema/offset_for_leader_epoch/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v0/request.py` & `kio-0.1.0/src/kio/schema/produce/v0/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 from dataclasses import dataclass
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.request_header.v1.header import RequestHeader
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionProduceData:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(0)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data to be produced."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class TopicProduceData:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(0)
```

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v0/response.py` & `kio-0.1.0/src/kio/schema/produce/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v1/request.py` & `kio-0.1.0/src/kio/schema/produce/v1/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 from dataclasses import dataclass
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.request_header.v1.header import RequestHeader
 from kio.schema.types import TopicName
 from kio.static.constants import EntityType
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionProduceData:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(1)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data to be produced."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class TopicProduceData:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(1)
```

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v1/response.py` & `kio-0.1.0/src/kio/schema/produce/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v2/request.py` & `kio-0.1.0/src/kio/schema/produce/v3/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,52 +6,58 @@
 
 from dataclasses import dataclass
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.request_header.v1.header import RequestHeader
 from kio.schema.types import TopicName
+from kio.schema.types import TransactionalId
 from kio.static.constants import EntityType
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionProduceData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(2)
+    __version__: ClassVar[i16] = i16(3)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data to be produced."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class TopicProduceData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(2)
+    __version__: ClassVar[i16] = i16(3)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     name: TopicName = field(metadata={"kafka_type": "string"})
     """The topic name."""
     partition_data: tuple[PartitionProduceData, ...]
     """Each partition to produce to."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class ProduceRequest:
     __type__: ClassVar = EntityType.request
-    __version__: ClassVar[i16] = i16(2)
+    __version__: ClassVar[i16] = i16(3)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
+    transactional_id: TransactionalId | None = field(
+        metadata={"kafka_type": "string"}, default=None
+    )
+    """The transactional ID, or null if the producer is not transactional."""
     acks: i16 = field(metadata={"kafka_type": "int16"})
     """The number of acknowledgments the producer requires the leader to have received before considering a request complete. Allowed values: 0 for no acknowledgments, 1 for only the leader and -1 for the full ISR."""
     timeout: i32Timedelta = field(metadata={"kafka_type": "timedelta_i32"})
     """The timeout to await a response in milliseconds."""
     topic_data: tuple[TopicProduceData, ...]
     """Each topic to produce to."""
```

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v2/response.py` & `kio-0.1.0/src/kio/schema/produce/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v3/request.py` & `kio-0.1.0/src/kio/schema/produce/v5/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,49 +8,50 @@
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.request_header.v1.header import RequestHeader
 from kio.schema.types import TopicName
 from kio.schema.types import TransactionalId
 from kio.static.constants import EntityType
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionProduceData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(3)
+    __version__: ClassVar[i16] = i16(5)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data to be produced."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class TopicProduceData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(3)
+    __version__: ClassVar[i16] = i16(5)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     name: TopicName = field(metadata={"kafka_type": "string"})
     """The topic name."""
     partition_data: tuple[PartitionProduceData, ...]
     """Each partition to produce to."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class ProduceRequest:
     __type__: ClassVar = EntityType.request
-    __version__: ClassVar[i16] = i16(3)
+    __version__: ClassVar[i16] = i16(5)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     transactional_id: TransactionalId | None = field(
         metadata={"kafka_type": "string"}, default=None
     )
     """The transactional ID, or null if the producer is not transactional."""
```

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v3/response.py` & `kio-0.1.0/src/kio/schema/produce/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v4/request.py` & `kio-0.1.0/src/kio/schema/produce/v4/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.request_header.v1.header import RequestHeader
 from kio.schema.types import TopicName
 from kio.schema.types import TransactionalId
 from kio.static.constants import EntityType
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionProduceData:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(4)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data to be produced."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class TopicProduceData:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(4)
```

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v4/response.py` & `kio-0.1.0/src/kio/schema/produce/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v5/request.py` & `kio-0.1.0/src/kio/schema/produce/v6/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,49 +8,50 @@
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.request_header.v1.header import RequestHeader
 from kio.schema.types import TopicName
 from kio.schema.types import TransactionalId
 from kio.static.constants import EntityType
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionProduceData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(5)
+    __version__: ClassVar[i16] = i16(6)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data to be produced."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class TopicProduceData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(5)
+    __version__: ClassVar[i16] = i16(6)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     name: TopicName = field(metadata={"kafka_type": "string"})
     """The topic name."""
     partition_data: tuple[PartitionProduceData, ...]
     """Each partition to produce to."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class ProduceRequest:
     __type__: ClassVar = EntityType.request
-    __version__: ClassVar[i16] = i16(5)
+    __version__: ClassVar[i16] = i16(6)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     transactional_id: TransactionalId | None = field(
         metadata={"kafka_type": "string"}, default=None
     )
     """The transactional ID, or null if the producer is not transactional."""
```

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v5/response.py` & `kio-0.1.0/src/kio/schema/produce/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v6/request.py` & `kio-0.1.0/src/kio/schema/produce/v9/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,54 +4,55 @@
 https://github.com/apache/kafka/tree/3.6.0/clients/src/main/resources/common/message/ProduceRequest.json
 """
 
 from dataclasses import dataclass
 from dataclasses import field
 from typing import ClassVar
 
-from kio.schema.request_header.v1.header import RequestHeader
+from kio.schema.request_header.v2.header import RequestHeader
 from kio.schema.types import TopicName
 from kio.schema.types import TransactionalId
 from kio.static.constants import EntityType
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionProduceData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(6)
-    __flexible__: ClassVar[bool] = False
+    __version__: ClassVar[i16] = i16(9)
+    __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data to be produced."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class TopicProduceData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(6)
-    __flexible__: ClassVar[bool] = False
+    __version__: ClassVar[i16] = i16(9)
+    __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     name: TopicName = field(metadata={"kafka_type": "string"})
     """The topic name."""
     partition_data: tuple[PartitionProduceData, ...]
     """Each partition to produce to."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class ProduceRequest:
     __type__: ClassVar = EntityType.request
-    __version__: ClassVar[i16] = i16(6)
-    __flexible__: ClassVar[bool] = False
+    __version__: ClassVar[i16] = i16(9)
+    __flexible__: ClassVar[bool] = True
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     transactional_id: TransactionalId | None = field(
         metadata={"kafka_type": "string"}, default=None
     )
     """The transactional ID, or null if the producer is not transactional."""
     acks: i16 = field(metadata={"kafka_type": "int16"})
```

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v6/response.py` & `kio-0.1.0/src/kio/schema/produce/v6/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v7/request.py` & `kio-0.1.0/src/kio/schema/produce/v7/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.request_header.v1.header import RequestHeader
 from kio.schema.types import TopicName
 from kio.schema.types import TransactionalId
 from kio.static.constants import EntityType
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionProduceData:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(7)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data to be produced."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class TopicProduceData:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(7)
```

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v7/response.py` & `kio-0.1.0/src/kio/schema/produce/v7/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v8/request.py` & `kio-0.1.0/src/kio/schema/produce/v8/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 from dataclasses import field
 from typing import ClassVar
 
 from kio.schema.request_header.v1.header import RequestHeader
 from kio.schema.types import TopicName
 from kio.schema.types import TransactionalId
 from kio.static.constants import EntityType
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionProduceData:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(8)
     __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data to be produced."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class TopicProduceData:
     __type__: ClassVar = EntityType.nested
     __version__: ClassVar[i16] = i16(8)
```

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v8/response.py` & `kio-0.1.0/src/kio/schema/produce/v8/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v9/request.py` & `kio-0.1.0/src/kio/schema/produce/v2/request.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,59 +4,55 @@
 https://github.com/apache/kafka/tree/3.6.0/clients/src/main/resources/common/message/ProduceRequest.json
 """
 
 from dataclasses import dataclass
 from dataclasses import field
 from typing import ClassVar
 
-from kio.schema.request_header.v2.header import RequestHeader
+from kio.schema.request_header.v1.header import RequestHeader
 from kio.schema.types import TopicName
-from kio.schema.types import TransactionalId
 from kio.static.constants import EntityType
+from kio.static.primitive import Records
 from kio.static.primitive import i16
 from kio.static.primitive import i32
 from kio.static.primitive import i32Timedelta
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class PartitionProduceData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(9)
-    __flexible__: ClassVar[bool] = True
+    __version__: ClassVar[i16] = i16(2)
+    __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     index: i32 = field(metadata={"kafka_type": "int32"})
     """The partition index."""
-    records: bytes | None = field(metadata={"kafka_type": "records"})
+    records: Records | None = field(metadata={"kafka_type": "records"})
     """The record data to be produced."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class TopicProduceData:
     __type__: ClassVar = EntityType.nested
-    __version__: ClassVar[i16] = i16(9)
-    __flexible__: ClassVar[bool] = True
+    __version__: ClassVar[i16] = i16(2)
+    __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
     name: TopicName = field(metadata={"kafka_type": "string"})
     """The topic name."""
     partition_data: tuple[PartitionProduceData, ...]
     """Each partition to produce to."""
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class ProduceRequest:
     __type__: ClassVar = EntityType.request
-    __version__: ClassVar[i16] = i16(9)
-    __flexible__: ClassVar[bool] = True
+    __version__: ClassVar[i16] = i16(2)
+    __flexible__: ClassVar[bool] = False
     __api_key__: ClassVar[i16] = i16(0)
     __header_schema__: ClassVar[type[RequestHeader]] = RequestHeader
-    transactional_id: TransactionalId | None = field(
-        metadata={"kafka_type": "string"}, default=None
-    )
-    """The transactional ID, or null if the producer is not transactional."""
     acks: i16 = field(metadata={"kafka_type": "int16"})
     """The number of acknowledgments the producer requires the leader to have received before considering a request complete. Allowed values: 0 for no acknowledgments, 1 for only the leader and -1 for the full ISR."""
     timeout: i32Timedelta = field(metadata={"kafka_type": "timedelta_i32"})
     """The timeout to await a response in milliseconds."""
     topic_data: tuple[TopicProduceData, ...]
     """Each topic to produce to."""
```

### Comparing `kio-0.0.0a3/src/kio/schema/produce/v9/response.py` & `kio-0.1.0/src/kio/schema/produce/v9/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/renew_delegation_token/v0/request.py` & `kio-0.1.0/src/kio/schema/renew_delegation_token/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/renew_delegation_token/v0/response.py` & `kio-0.1.0/src/kio/schema/renew_delegation_token/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/renew_delegation_token/v1/request.py` & `kio-0.1.0/src/kio/schema/renew_delegation_token/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/renew_delegation_token/v1/response.py` & `kio-0.1.0/src/kio/schema/renew_delegation_token/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/renew_delegation_token/v2/request.py` & `kio-0.1.0/src/kio/schema/renew_delegation_token/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/renew_delegation_token/v2/response.py` & `kio-0.1.0/src/kio/schema/renew_delegation_token/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/request_header/v0/header.py` & `kio-0.1.0/src/kio/schema/request_header/v0/header.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/request_header/v1/header.py` & `kio-0.1.0/src/kio/schema/request_header/v1/header.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/request_header/v2/header.py` & `kio-0.1.0/src/kio/schema/request_header/v2/header.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/response_header/v0/header.py` & `kio-0.1.0/src/kio/schema/response_header/v0/header.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/response_header/v1/header.py` & `kio-0.1.0/src/kio/schema/response_header/v1/header.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sasl_authenticate/v0/request.py` & `kio-0.1.0/src/kio/schema/sasl_authenticate/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sasl_authenticate/v0/response.py` & `kio-0.1.0/src/kio/schema/sasl_authenticate/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sasl_authenticate/v1/request.py` & `kio-0.1.0/src/kio/schema/sasl_authenticate/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sasl_authenticate/v1/response.py` & `kio-0.1.0/src/kio/schema/sasl_authenticate/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sasl_authenticate/v2/request.py` & `kio-0.1.0/src/kio/schema/sasl_authenticate/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sasl_authenticate/v2/response.py` & `kio-0.1.0/src/kio/schema/sasl_authenticate/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sasl_handshake/v0/request.py` & `kio-0.1.0/src/kio/schema/sasl_handshake/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sasl_handshake/v0/response.py` & `kio-0.1.0/src/kio/schema/sasl_handshake/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sasl_handshake/v1/request.py` & `kio-0.1.0/src/kio/schema/sasl_handshake/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sasl_handshake/v1/response.py` & `kio-0.1.0/src/kio/schema/sasl_handshake/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/snapshot_footer_record/v0/data.py` & `kio-0.1.0/src/kio/schema/snapshot_footer_record/v0/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/snapshot_header_record/v0/data.py` & `kio-0.1.0/src/kio/schema/snapshot_header_record/v0/data.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/stop_replica/v0/request.py` & `kio-0.1.0/src/kio/schema/stop_replica/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/stop_replica/v0/response.py` & `kio-0.1.0/src/kio/schema/stop_replica/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/stop_replica/v1/request.py` & `kio-0.1.0/src/kio/schema/stop_replica/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/stop_replica/v1/response.py` & `kio-0.1.0/src/kio/schema/stop_replica/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/stop_replica/v2/request.py` & `kio-0.1.0/src/kio/schema/stop_replica/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/stop_replica/v2/response.py` & `kio-0.1.0/src/kio/schema/stop_replica/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/stop_replica/v3/request.py` & `kio-0.1.0/src/kio/schema/stop_replica/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/stop_replica/v3/response.py` & `kio-0.1.0/src/kio/schema/stop_replica/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/stop_replica/v4/request.py` & `kio-0.1.0/src/kio/schema/stop_replica/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/stop_replica/v4/response.py` & `kio-0.1.0/src/kio/schema/stop_replica/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v0/request.py` & `kio-0.1.0/src/kio/schema/sync_group/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v0/response.py` & `kio-0.1.0/src/kio/schema/sync_group/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v1/request.py` & `kio-0.1.0/src/kio/schema/sync_group/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v1/response.py` & `kio-0.1.0/src/kio/schema/sync_group/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v2/request.py` & `kio-0.1.0/src/kio/schema/sync_group/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v2/response.py` & `kio-0.1.0/src/kio/schema/sync_group/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v3/request.py` & `kio-0.1.0/src/kio/schema/sync_group/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v3/response.py` & `kio-0.1.0/src/kio/schema/sync_group/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v4/request.py` & `kio-0.1.0/src/kio/schema/sync_group/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v4/response.py` & `kio-0.1.0/src/kio/schema/sync_group/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v5/request.py` & `kio-0.1.0/src/kio/schema/sync_group/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/sync_group/v5/response.py` & `kio-0.1.0/src/kio/schema/sync_group/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/txn_offset_commit/v0/request.py` & `kio-0.1.0/src/kio/schema/txn_offset_commit/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/txn_offset_commit/v0/response.py` & `kio-0.1.0/src/kio/schema/txn_offset_commit/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/txn_offset_commit/v1/request.py` & `kio-0.1.0/src/kio/schema/txn_offset_commit/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/txn_offset_commit/v1/response.py` & `kio-0.1.0/src/kio/schema/txn_offset_commit/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/txn_offset_commit/v2/request.py` & `kio-0.1.0/src/kio/schema/txn_offset_commit/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/txn_offset_commit/v2/response.py` & `kio-0.1.0/src/kio/schema/txn_offset_commit/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/txn_offset_commit/v3/request.py` & `kio-0.1.0/src/kio/schema/txn_offset_commit/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/txn_offset_commit/v3/response.py` & `kio-0.1.0/src/kio/schema/txn_offset_commit/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/unregister_broker/v0/request.py` & `kio-0.1.0/src/kio/schema/unregister_broker/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/unregister_broker/v0/response.py` & `kio-0.1.0/src/kio/schema/unregister_broker/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_features/v0/request.py` & `kio-0.1.0/src/kio/schema/update_features/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_features/v0/response.py` & `kio-0.1.0/src/kio/schema/update_features/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_features/v1/request.py` & `kio-0.1.0/src/kio/schema/update_features/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_features/v1/response.py` & `kio-0.1.0/src/kio/schema/update_features/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v0/request.py` & `kio-0.1.0/src/kio/schema/update_metadata/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v0/response.py` & `kio-0.1.0/src/kio/schema/update_metadata/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v1/request.py` & `kio-0.1.0/src/kio/schema/update_metadata/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v1/response.py` & `kio-0.1.0/src/kio/schema/update_metadata/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v2/request.py` & `kio-0.1.0/src/kio/schema/update_metadata/v2/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v2/response.py` & `kio-0.1.0/src/kio/schema/update_metadata/v2/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v3/request.py` & `kio-0.1.0/src/kio/schema/update_metadata/v3/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v3/response.py` & `kio-0.1.0/src/kio/schema/update_metadata/v3/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v4/request.py` & `kio-0.1.0/src/kio/schema/update_metadata/v4/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v4/response.py` & `kio-0.1.0/src/kio/schema/update_metadata/v4/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v5/request.py` & `kio-0.1.0/src/kio/schema/update_metadata/v5/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v5/response.py` & `kio-0.1.0/src/kio/schema/update_metadata/v5/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v6/request.py` & `kio-0.1.0/src/kio/schema/update_metadata/v6/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v6/response.py` & `kio-0.1.0/src/kio/schema/update_metadata/v6/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v7/request.py` & `kio-0.1.0/src/kio/schema/update_metadata/v7/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v7/response.py` & `kio-0.1.0/src/kio/schema/update_metadata/v7/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v8/request.py` & `kio-0.1.0/src/kio/schema/update_metadata/v8/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/update_metadata/v8/response.py` & `kio-0.1.0/src/kio/schema/update_metadata/v8/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/vote/v0/request.py` & `kio-0.1.0/src/kio/schema/vote/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/vote/v0/response.py` & `kio-0.1.0/src/kio/schema/vote/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/write_txn_markers/v0/request.py` & `kio-0.1.0/src/kio/schema/write_txn_markers/v0/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/write_txn_markers/v0/response.py` & `kio-0.1.0/src/kio/schema/write_txn_markers/v0/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/write_txn_markers/v1/request.py` & `kio-0.1.0/src/kio/schema/write_txn_markers/v1/request.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/schema/write_txn_markers/v1/response.py` & `kio-0.1.0/src/kio/schema/write_txn_markers/v1/response.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/serial/_introspect.py` & `kio-0.1.0/src/kio/serial/_introspect.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/serial/_parse.py` & `kio-0.1.0/src/kio/serial/_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,26 +132,20 @@
 E = TypeVar("E", bound=Entity)
 
 
 @overload
 def entity_reader(
     entity_type: type[E],
     nullable: Literal[False] = ...,
-) -> readers.Reader[E]:
-    ...
-
-
+) -> readers.Reader[E]: ...
 @overload
 def entity_reader(
     entity_type: type[E],
     nullable: Literal[True],
-) -> readers.Reader[E | None]:
-    ...
-
-
+) -> readers.Reader[E | None]: ...
 @cache
 def entity_reader(
     entity_type: type[E],
     nullable: bool = False,
 ) -> readers.Reader[E | None]:
     field_readers = {}
     tagged_field_readers = {}
```

### Comparing `kio-0.0.0a3/src/kio/serial/_serialize.py` & `kio-0.1.0/src/kio/serial/_serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,23 +157,23 @@
         write_int8(buffer, NullableEntityMarker.not_null.value)
         write_entity(buffer, entity)
 
     return write_nullable
 
 
 @overload
-def entity_writer(entity_type: type[E], nullable: Literal[False] = ...) -> Writer[E]:
-    ...
-
-
+def entity_writer(
+    entity_type: type[E],
+    nullable: Literal[False] = ...,
+) -> Writer[E]: ...
 @overload
-def entity_writer(entity_type: type[E], nullable: Literal[True]) -> Writer[E | None]:
-    ...
-
-
+def entity_writer(
+    entity_type: type[E],
+    nullable: Literal[True],
+) -> Writer[E | None]: ...
 @cache
 def entity_writer(entity_type: type[E], nullable: bool = False) -> Writer[E | None]:
     field_writers = {}
     tagged_field_writers = {}
     is_request_header = entity_type.__name__ == "RequestHeader"
 
     for field in fields(entity_type):
```

### Comparing `kio-0.0.0a3/src/kio/serial/readers.py` & `kio-0.1.0/src/kio/serial/readers.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/serial/writers.py` & `kio-0.1.0/src/kio/serial/writers.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/static/_phantom.py` & `kio-0.1.0/src/kio/static/_phantom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This is a less powerful, but good enough approximation of the phantom-types library,
 lacking some bells and whistles like Pydantic support and bounds checks.
 """
+
 from __future__ import annotations
 
 import abc
 
 from collections.abc import Callable
 from types import ModuleType
 from typing import Generic
@@ -25,24 +26,21 @@
 
 U = TypeVar("U")
 Predicate: TypeAlias = Callable[[U], bool]
 
 
 @runtime_checkable
 class InstanceCheckable(Protocol):
-    def __instancecheck__(self, instance: object) -> bool:
-        ...
+    def __instancecheck__(self, instance: object) -> bool: ...
 
 
 class PhantomMeta(abc.ABCMeta):
     def __instancecheck__(self, instance: object) -> bool:
-        return issubclass(
-            self, InstanceCheckable
-        ) and self.__instancecheck__(  # type: ignore[attr-defined]
-            instance,
+        return (
+            issubclass(self, InstanceCheckable) and self.__instancecheck__(instance)  # type: ignore[attr-defined]
         )
 
     def __call__(cls, instance):  # type: ignore[no-untyped-def]
         return cls.parse(instance)  # type: ignore[attr-defined]
 
 
 T = TypeVar("T")
@@ -71,16 +69,15 @@
         else:
             cls.__predicate__ = predicate
 
         if hypothesis is not None:  # pragma: no cover
             cls.__hypothesis_hook__()
 
     @classmethod
-    def __hypothesis_hook__(cls) -> None:
-        ...
+    def __hypothesis_hook__(cls) -> None: ...
 
     @classmethod
     def __instancecheck__(cls, instance: object) -> bool:
         return isinstance(instance, cls.__bound__) and cls.__predicate__(instance)
 
     @classmethod
     def parse(cls, instance: object) -> Self:
```

### Comparing `kio-0.0.0a3/src/kio/static/constants.py` & `kio-0.1.0/src/kio/static/constants.py`

 * *Files identical despite different names*

### Comparing `kio-0.0.0a3/src/kio/static/primitive.py` & `kio-0.1.0/src/kio/static/primitive.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from typing import Final
 from typing import Self
 
 from ._phantom import Phantom
 from ._phantom import Predicate
 
 
+class Records(bytes, Phantom, predicate=lambda _: True, bound=bytes): ...
+
+
 def inclusive_interval(low: int, high: int) -> Predicate[int]:
     def check(value: int) -> bool:
         return low <= value <= high
 
     return check
 
 
@@ -53,44 +56,36 @@
             integers(  # type: ignore[arg-type]
                 min_value=getattr(cls, "__low__", None),
                 max_value=getattr(cls, "__high__", None),
             ),
         )
 
 
-class i64(Interval, low=-(2**63), high=2**63 - 1):
-    ...
+class i64(Interval, low=-(2**63), high=2**63 - 1): ...
 
 
-class i32(i64, low=-(2**31), high=2**31 - 1):
-    ...
+class i32(i64, low=-(2**31), high=2**31 - 1): ...
 
 
-class i16(i32, low=-(2**15), high=2**15 - 1):
-    ...
+class i16(i32, low=-(2**15), high=2**15 - 1): ...
 
 
-class i8(i16, low=-128, high=127):
-    ...
+class i8(i16, low=-128, high=127): ...
 
 
-class u64(Interval, low=0, high=2**64 - 1):
-    ...
+class u64(Interval, low=0, high=2**64 - 1): ...
 
 
-class u32(u64, high=2**32 - 1):
-    ...
+class u32(u64, high=2**32 - 1): ...
 
 
-class u16(u32, high=2**16 - 1):
-    ...
+class u16(u32, high=2**16 - 1): ...
 
 
-class u8(u16, high=2**8 - 1):
-    ...
+class u8(u16, high=2**8 - 1): ...
 
 
 class f64(float, Phantom, bound=float, predicate=math.isfinite):
     @classmethod
     def __hypothesis_hook__(cls) -> None:
         from hypothesis.strategies import floats
         from hypothesis.strategies import register_type_strategy
```

### Comparing `kio-0.0.0a3/src/kio/static/protocol.py` & `kio-0.1.0/src/kio/static/protocol.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,19 +32,22 @@
 
 
 RequestHeader: TypeAlias = (
     kio.schema.request_header.v0.RequestHeader
     | kio.schema.request_header.v1.RequestHeader
     | kio.schema.request_header.v2.RequestHeader
 )
+"""Convenient union type of all possible request header types."""
 ResponseHeader: TypeAlias = (
     kio.schema.response_header.v0.ResponseHeader
     | kio.schema.response_header.v1.ResponseHeader
 )
+"""Convenient union type of all possible response header types."""
 Header: TypeAlias = RequestHeader | ResponseHeader
+"""Convenient union type of all possible request and response header types."""
 
 
 class Entity(DataclassInstance, Protocol):
     """All schema entities adhere to this protocol."""
 
     __type__: ClassVar[EntityType]
     __version__: ClassVar[i16]
@@ -89,32 +92,44 @@
         """
         The header entity type that should be used when sending or receiving this
         payload.
         """
 
 
 class HeaderV0RequestPayload(Payload, Protocol):
+    """Protocol describing a request payload entity type with a V0 header."""
+
     __header_schema__: ClassVar[type[kio.schema.request_header.v0.RequestHeader]]
 
 
 class HeaderV1RequestPayload(Payload, Protocol):
+    """Protocol describing a request payload entity type with a V1 header."""
+
     __header_schema__: ClassVar[type[kio.schema.request_header.v1.RequestHeader]]
 
 
 class HeaderV2RequestPayload(Payload, Protocol):
+    """Protocol describing a request payload entity type with a V2 header."""
+
     __header_schema__: ClassVar[type[kio.schema.request_header.v2.RequestHeader]]
 
 
 RequestPayload: TypeAlias = (
     HeaderV0RequestPayload | HeaderV1RequestPayload | HeaderV2RequestPayload
 )
+"""Convenient union type of all possible request payloads."""
 
 
 class HeaderV0ResponsePayload(Payload, Protocol):
+    """Protocol describing a response payload entity type with a V0 header."""
+
     __header_schema__: ClassVar[type[kio.schema.response_header.v0.ResponseHeader]]
 
 
 class HeaderV1ResponsePayload(Payload, Protocol):
+    """Protocol describing a response payload entity type with a V1 header."""
+
     __header_schema__: ClassVar[type[kio.schema.response_header.v1.ResponseHeader]]
 
 
 ResponsePayload: TypeAlias = HeaderV0ResponsePayload | HeaderV1ResponsePayload
+"""Convenient union type of all possible response payloads."""
```

### Comparing `kio-0.0.0a3/src/kio.egg-info/PKG-INFO` & `kio-0.1.0/src/kio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: kio
-Version: 0.0.0a3
+Version: 0.1.0
 Summary: Python data types for the Apache Kafka® Protocol.
 Author-email: Anton Agestam <anton.agestam@aiven.io>
 License: Apache-2.0 license
 Project-URL: Source Repository, https://github.com/Aiven-Open/kio
+Project-URL: Documentation, https://aiven-open.github.io/kio/
 Project-URL: Bug Tracker, https://github.com/Aiven-Open/kio/issues
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: kio Version: 0.0.0a3 Summary: Python data types for
+Metadata-Version: 2.1 Name: kio Version: 0.1.0 Summary: Python data types for
 the Apache KafkaÂ® Protocol. Author-email: Anton Agestam
 aiven.io> License: Apache-2.0 license Project-URL: Source Repository, https://
-github.com/Aiven-Open/kio Project-URL: Bug Tracker, https://github.com/Aiven-
-Open/kio/issues Classifier: Intended Audience :: Developers Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.11 Classifier: Programming Language :: Python :: 3.12 Classifier: Typing ::
-Typed Classifier: Topic :: Database Requires-Python: >=3.11 Description-
-Content-Type: text/markdown; charset=UTF-8 License-File: LICENSE License-File:
-NOTICE Requires-Dist: typing-extensions>=4.6.0 Provides-Extra: test Requires-
-Dist: pytest; extra == "test" Requires-Dist: pytest-asyncio; extra == "test"
-Requires-Dist: pytest-icdiff; extra == "test" Requires-Dist: pytest-random-
-order; extra == "test" Requires-Dist: hypothesis>=6.61.0; extra == "test"
-Requires-Dist: coverage; extra == "test" Provides-Extra: codegen Requires-Dist:
+github.com/Aiven-Open/kio Project-URL: Documentation, https://aiven-
+open.github.io/kio/ Project-URL: Bug Tracker, https://github.com/Aiven-Open/
+kio/issues Classifier: Intended Audience :: Developers Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Typing :: Typed Classifier:
+Topic :: Database Requires-Python: >=3.11 Description-Content-Type: text/
+markdown; charset=UTF-8 License-File: LICENSE License-File: NOTICE Requires-
+Dist: typing-extensions>=4.6.0 Provides-Extra: test Requires-Dist: pytest;
+extra == "test" Requires-Dist: pytest-asyncio; extra == "test" Requires-Dist:
+pytest-icdiff; extra == "test" Requires-Dist: pytest-random-order; extra ==
+"test" Requires-Dist: hypothesis>=6.61.0; extra == "test" Requires-Dist:
+coverage; extra == "test" Provides-Extra: codegen Requires-Dist:
 pydantic<2,>=1.10.4; extra == "codegen" Requires-Dist: requests; extra ==
 "codegen" Requires-Dist: pre-commit; extra == "codegen" Provides-Extra: all
 Requires-Dist: kio[test]; extra == "all" Requires-Dist: kio[codegen]; extra ==
 "all"
                                ************ kkiioo ************
                     _[_C_I_ _B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_ _r_e_p_o_r_t_]
                         _[_P_y_P_I_ _P_a_c_k_a_g_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
```

### Comparing `kio-0.0.0a3/src/kio.egg-info/SOURCES.txt` & `kio-0.1.0/src/kio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 LICENSE
 MANIFEST.in
 NOTICE
 README.md
 pyproject.toml
 src/kio/__init__.py
 src/kio/_utils.py
+src/kio/index.py
 src/kio/py.typed
 src/kio.egg-info/PKG-INFO
 src/kio.egg-info/SOURCES.txt
 src/kio.egg-info/dependency_links.txt
 src/kio.egg-info/requires.txt
 src/kio.egg-info/top_level.txt
 src/kio/schema/__init__.py
+src/kio/schema/index.py
 src/kio/schema/types.py
 src/kio/schema/add_offsets_to_txn/__init__.py
 src/kio/schema/add_offsets_to_txn/v0/__init__.py
 src/kio/schema/add_offsets_to_txn/v0/request.py
 src/kio/schema/add_offsets_to_txn/v0/response.py
 src/kio/schema/add_offsets_to_txn/v1/__init__.py
 src/kio/schema/add_offsets_to_txn/v1/request.py
```

