# Comparing `tmp/csle_collector-0.5.2.tar.gz` & `tmp/csle_collector-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_collector-0.5.2.tar", last modified: Tue Apr 30 10:49:23 2024, max compression
+gzip compressed data, was "csle_collector-0.5.3.tar", last modified: Mon May 13 17:19:31 2024, max compression
```

## Comparing `csle_collector-0.5.2.tar` & `csle_collector-0.5.3.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.994574 csle_collector-0.5.2/
--rw-rw-r--   0 kim       (1000) kim       (1000)      793 2024-04-30 10:49:23.994574 csle_collector-0.5.2/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     6209 2024-01-29 11:24:00.000000 csle_collector-0.5.2/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      674 2023-08-08 14:54:06.000000 csle_collector-0.5.2/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     2012 2024-04-30 10:49:23.994574 csle_collector-0.5.2/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_collector-0.5.2/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.966574 csle_collector-0.5.2/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.966574 csle_collector-0.5.2/src/csle_collector/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 csle_collector-0.5.2/src/csle_collector/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.970574 csle_collector-0.5.2/src/csle_collector/client_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/client_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11529 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/client_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5708 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/client_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8592 2023-06-04 07:11:42.000000 csle_collector-0.5.2/src/csle_collector/client_manager/client_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2179 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/client_manager/client_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4905 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/client_population_metrics.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.974573 csle_collector-0.5.2/src/csle_collector/client_manager/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-30 09:40:47.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1538 2023-08-24 07:47:35.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10142 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/client.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      340 2023-05-30 13:25:09.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/client_arrival_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2646 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/constant_arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3498 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/eptmp_arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3333 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3647 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/sine_arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3037 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/spiking_arrival_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5442 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/workflow_markov_chain.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5167 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/workflow_service.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5506 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/dao/workflows_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4274 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/query_clients.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.974573 csle_collector-0.5.2/src/csle_collector/client_manager/threads/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-30 09:20:57.000000 csle_collector-0.5.2/src/csle_collector/client_manager/threads/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7493 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/client_manager/threads/arrival_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      972 2023-06-10 13:26:02.000000 csle_collector-0.5.2/src/csle_collector/client_manager/threads/client_thread.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2375 2023-06-10 13:26:02.000000 csle_collector-0.5.2/src/csle_collector/client_manager/threads/producer_thread.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.974573 csle_collector-0.5.2/src/csle_collector/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    36628 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.974573 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.974573 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12998 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/dao/docker_stats.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8158 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/docker_stats_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2578 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6193 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8932 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/docker_stats_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4276 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.974573 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/threads/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/threads/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6475 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/docker_stats_manager/threads/docker_stats_thread.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.978574 csle_collector-0.5.2/src/csle_collector/elk_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/elk_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10740 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/elk_manager/elk_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2642 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/elk_manager/elk_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14300 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1540 2023-08-08 10:01:45.000000 csle_collector-0.5.2/src/csle_collector/elk_manager/elk_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6227 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/elk_manager/query_elk_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.978574 csle_collector-0.5.2/src/csle_collector/host_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/host_manager/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.978574 csle_collector-0.5.2/src/csle_collector/host_manager/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-08-10 07:39:54.000000 csle_collector-0.5.2/src/csle_collector/host_manager/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2152 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/host_manager/dao/failed_login_attempt.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8321 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/host_manager/dao/host_metrics.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2697 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/host_manager/dao/successful_login.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    61864 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/host_manager/host_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6844 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/host_manager/host_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    28800 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/host_manager/host_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    34458 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/host_manager/host_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17833 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/host_manager/query_host_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.978574 csle_collector-0.5.2/src/csle_collector/host_manager/threads/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-08-10 07:39:54.000000 csle_collector-0.5.2/src/csle_collector/host_manager/threads/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2684 2023-08-10 07:39:54.000000 csle_collector-0.5.2/src/csle_collector/host_manager/threads/host_monitor_thread.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.982574 csle_collector-0.5.2/src/csle_collector/kafka_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/kafka_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6487 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/kafka_manager/kafka_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2146 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/kafka_manager/kafka_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8484 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1726 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/kafka_manager/kafka_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3501 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/kafka_manager/query_kafka_server.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.982574 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.982574 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-06-13 15:07:00.000000 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3665 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13966 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert_counters.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     9655 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4448 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13730 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5883 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.982574 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/threads/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-06-13 15:05:09.000000 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/threads/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2108 2023-06-13 16:05:29.000000 csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/threads/ossec_ids_monitor_thread.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.986574 csle_collector-0.5.2/src/csle_collector/ryu_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/ryu_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4241 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ryu_manager/query_ryu_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15273 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ryu_manager/ryu_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2414 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ryu_manager/ryu_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8367 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2102 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ryu_manager/ryu_manager_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.986574 csle_collector-0.5.2/src/csle_collector/ryu_manager/threads/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ryu_manager/threads/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3332 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/ryu_manager/threads/failure_detector.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.986574 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.986574 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-08-10 07:39:54.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11068 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/snort_ids_alert.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12629 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/snort_ids_alert_counters.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2520 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/snort_ids_fast_log_alert.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     9819 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/snort_ids_ip_alert_counters.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4903 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/snort_ids_rule_counters.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6293 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10517 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/snort_ids_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5252 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    16968 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.986574 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/threads/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-08-10 07:39:54.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/threads/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2839 2023-08-10 07:39:54.000000 csle_collector-0.5.2/src/csle_collector/snort_ids_manager/threads/snort_ids_monitor_thread.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.990574 csle_collector-0.5.2/src/csle_collector/traffic_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/traffic_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2753 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/traffic_manager/query_traffic_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7861 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/traffic_manager/traffic_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1735 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/traffic_manager/traffic_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5596 2023-03-28 14:03:22.000000 csle_collector-0.5.2/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1526 2024-01-29 11:24:00.000000 csle_collector-0.5.2/src/csle_collector/traffic_manager/traffic_manager_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.970574 csle_collector-0.5.2/src/csle_collector.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      793 2024-04-30 10:49:23.000000 csle_collector-0.5.2/src/csle_collector.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     6419 2024-04-30 10:49:23.000000 csle_collector-0.5.2/src/csle_collector.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:49:23.000000 csle_collector-0.5.2/src/csle_collector.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:37.000000 csle_collector-0.5.2/src/csle_collector.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      612 2024-04-30 10:49:23.000000 csle_collector-0.5.2/src/csle_collector.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       15 2024-04-30 10:49:23.000000 csle_collector-0.5.2/src/csle_collector.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:23.990574 csle_collector-0.5.2/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)    17047 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_client_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7897 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_client_manager_dao.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7187 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_docker_stats_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      830 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_docker_stats_manager_dao.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8856 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_elk_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    34019 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_host_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2564 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_host_manager_dao.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5250 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_kafka_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12484 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_ossec_ids_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1875 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_ossec_ids_manager_dao.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     9883 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_ryu_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12634 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_snort_ids_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4708 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_snort_ids_manager_dao.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5094 2024-01-29 11:24:00.000000 csle_collector-0.5.2/tests/test_traffic_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.210441 csle_collector-0.5.3/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      793 2024-05-13 17:19:31.210441 csle_collector-0.5.3/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6209 2024-01-29 11:24:00.000000 csle_collector-0.5.3/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      674 2023-08-08 14:54:06.000000 csle_collector-0.5.3/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2012 2024-05-13 17:19:31.210441 csle_collector-0.5.3/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_collector-0.5.3/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.182441 csle_collector-0.5.3/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.186441 csle_collector-0.5.3/src/csle_collector/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_collector-0.5.3/src/csle_collector/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.186441 csle_collector-0.5.3/src/csle_collector/client_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/client_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11529 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/client_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5708 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/client_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8592 2023-06-04 07:11:42.000000 csle_collector-0.5.3/src/csle_collector/client_manager/client_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2179 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/client_manager/client_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4905 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/client_population_metrics.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.190441 csle_collector-0.5.3/src/csle_collector/client_manager/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-30 09:40:47.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1538 2023-08-24 07:47:35.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10142 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/client.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      340 2023-05-30 13:25:09.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/client_arrival_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2646 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/constant_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3498 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/eptmp_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3333 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3647 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/sine_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3037 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/spiking_arrival_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5442 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/workflow_markov_chain.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5167 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/workflow_service.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5506 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/dao/workflows_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4274 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/query_clients.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.190441 csle_collector-0.5.3/src/csle_collector/client_manager/threads/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-30 09:20:57.000000 csle_collector-0.5.3/src/csle_collector/client_manager/threads/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7493 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/client_manager/threads/arrival_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      972 2023-06-10 13:26:02.000000 csle_collector-0.5.3/src/csle_collector/client_manager/threads/client_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2375 2023-06-10 13:26:02.000000 csle_collector-0.5.3/src/csle_collector/client_manager/threads/producer_thread.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.190441 csle_collector-0.5.3/src/csle_collector/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    36628 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.194441 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.194441 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12998 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/dao/docker_stats.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8158 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/docker_stats_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2578 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6193 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8932 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/docker_stats_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4276 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.194441 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/threads/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/threads/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6475 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/docker_stats_manager/threads/docker_stats_thread.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.194441 csle_collector-0.5.3/src/csle_collector/elk_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/elk_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10740 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/elk_manager/elk_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2642 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/elk_manager/elk_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14300 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1540 2023-08-08 10:01:45.000000 csle_collector-0.5.3/src/csle_collector/elk_manager/elk_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6227 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/elk_manager/query_elk_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.194441 csle_collector-0.5.3/src/csle_collector/host_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/host_manager/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.198441 csle_collector-0.5.3/src/csle_collector/host_manager/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-08-10 07:39:54.000000 csle_collector-0.5.3/src/csle_collector/host_manager/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2152 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/host_manager/dao/failed_login_attempt.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8321 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/host_manager/dao/host_metrics.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2697 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/host_manager/dao/successful_login.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    61864 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/host_manager/host_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6844 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/host_manager/host_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28800 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/host_manager/host_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    34458 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/host_manager/host_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17833 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/host_manager/query_host_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.198441 csle_collector-0.5.3/src/csle_collector/host_manager/threads/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-08-10 07:39:54.000000 csle_collector-0.5.3/src/csle_collector/host_manager/threads/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2684 2023-08-10 07:39:54.000000 csle_collector-0.5.3/src/csle_collector/host_manager/threads/host_monitor_thread.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.198441 csle_collector-0.5.3/src/csle_collector/kafka_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/kafka_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6487 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/kafka_manager/kafka_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2146 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/kafka_manager/kafka_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8484 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1726 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/kafka_manager/kafka_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3501 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/kafka_manager/query_kafka_server.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.198441 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.202441 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-06-13 15:07:00.000000 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3665 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13966 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9655 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4448 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13730 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5883 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.202441 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/threads/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-06-13 15:05:09.000000 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/threads/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2108 2023-06-13 16:05:29.000000 csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/threads/ossec_ids_monitor_thread.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.202441 csle_collector-0.5.3/src/csle_collector/ryu_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/ryu_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4241 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ryu_manager/query_ryu_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15273 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ryu_manager/ryu_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2414 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ryu_manager/ryu_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8367 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2102 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ryu_manager/ryu_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.202441 csle_collector-0.5.3/src/csle_collector/ryu_manager/threads/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ryu_manager/threads/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3332 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/ryu_manager/threads/failure_detector.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.202441 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.206441 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-08-10 07:39:54.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11068 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/snort_ids_alert.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12629 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/snort_ids_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2520 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/snort_ids_fast_log_alert.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9819 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/snort_ids_ip_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4903 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/snort_ids_rule_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6293 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10517 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/snort_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5252 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16968 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.206441 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/threads/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-08-10 07:39:54.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/threads/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2839 2023-08-10 07:39:54.000000 csle_collector-0.5.3/src/csle_collector/snort_ids_manager/threads/snort_ids_monitor_thread.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.206441 csle_collector-0.5.3/src/csle_collector/traffic_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/traffic_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2753 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/traffic_manager/query_traffic_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7861 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/traffic_manager/traffic_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1735 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/traffic_manager/traffic_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5596 2023-03-28 14:03:22.000000 csle_collector-0.5.3/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1526 2024-01-29 11:24:00.000000 csle_collector-0.5.3/src/csle_collector/traffic_manager/traffic_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.186441 csle_collector-0.5.3/src/csle_collector.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      793 2024-05-13 17:19:31.000000 csle_collector-0.5.3/src/csle_collector.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6419 2024-05-13 17:19:31.000000 csle_collector-0.5.3/src/csle_collector.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:19:31.000000 csle_collector-0.5.3/src/csle_collector.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:37.000000 csle_collector-0.5.3/src/csle_collector.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      612 2024-05-13 17:19:31.000000 csle_collector-0.5.3/src/csle_collector.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       15 2024-05-13 17:19:31.000000 csle_collector-0.5.3/src/csle_collector.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:31.210441 csle_collector-0.5.3/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17047 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_client_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7897 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_client_manager_dao.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7187 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_docker_stats_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      830 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_docker_stats_manager_dao.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8856 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_elk_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    34019 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_host_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2564 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_host_manager_dao.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5250 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_kafka_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12484 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_ossec_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1875 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_ossec_ids_manager_dao.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9883 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_ryu_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12634 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_snort_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4708 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_snort_ids_manager_dao.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5094 2024-01-29 11:24:00.000000 csle_collector-0.5.3/tests/test_traffic_manager.py
```

### Comparing `csle_collector-0.5.2/PKG-INFO` & `csle_collector-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_collector
-Version: 0.5.2
+Version: 0.5.3
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.5.2/README.md` & `csle_collector-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/pyproject.toml` & `csle_collector-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/setup.cfg` & `csle_collector-0.5.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-base>=0.5.2
+	csle-base>=0.5.3
 	grpcio>=1.57.0
 	grpcio-tools>=1.57.0
 	scipy>=1.0.0
 	confluent-kafka>=1.8.2
 	docker>=3.0.0
 	PyYaml>=5.1.1
 	requests>=2.19.0
```

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/client_manager.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/client_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/client_manager_pb2.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/client_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/client_manager_pb2_grpc.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/client_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/client_manager_util.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/client_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/client_population_metrics.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/client_population_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/dao/arrival_config.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/dao/arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/dao/client.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/dao/client.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/dao/constant_arrival_config.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/dao/constant_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/dao/eptmp_arrival_config.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/dao/eptmp_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/dao/sine_arrival_config.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/dao/sine_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/dao/spiking_arrival_config.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/dao/spiking_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/dao/workflow_markov_chain.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/dao/workflow_markov_chain.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/dao/workflow_service.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/dao/workflow_service.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/dao/workflows_config.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/dao/workflows_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/query_clients.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/query_clients.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/threads/arrival_thread.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/threads/arrival_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/threads/client_thread.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/threads/client_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/client_manager/threads/producer_thread.py` & `csle_collector-0.5.3/src/csle_collector/client_manager/threads/producer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/constants/constants.py` & `csle_collector-0.5.3/src/csle_collector/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/docker_stats_manager/dao/docker_stats.py` & `csle_collector-0.5.3/src/csle_collector/docker_stats_manager/dao/docker_stats.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/docker_stats_manager/docker_stats_manager.py` & `csle_collector-0.5.3/src/csle_collector/docker_stats_manager/docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py` & `csle_collector-0.5.3/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py` & `csle_collector-0.5.3/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/docker_stats_manager/docker_stats_util.py` & `csle_collector-0.5.3/src/csle_collector/docker_stats_manager/docker_stats_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py` & `csle_collector-0.5.3/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/docker_stats_manager/threads/docker_stats_thread.py` & `csle_collector-0.5.3/src/csle_collector/docker_stats_manager/threads/docker_stats_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/elk_manager/elk_manager.py` & `csle_collector-0.5.3/src/csle_collector/elk_manager/elk_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/elk_manager/elk_manager_pb2.py` & `csle_collector-0.5.3/src/csle_collector/elk_manager/elk_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py` & `csle_collector-0.5.3/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/elk_manager/elk_manager_util.py` & `csle_collector-0.5.3/src/csle_collector/elk_manager/elk_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/elk_manager/query_elk_manager.py` & `csle_collector-0.5.3/src/csle_collector/elk_manager/query_elk_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/host_manager/dao/failed_login_attempt.py` & `csle_collector-0.5.3/src/csle_collector/host_manager/dao/failed_login_attempt.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/host_manager/dao/host_metrics.py` & `csle_collector-0.5.3/src/csle_collector/host_manager/dao/host_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/host_manager/dao/successful_login.py` & `csle_collector-0.5.3/src/csle_collector/host_manager/dao/successful_login.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/host_manager/host_manager.py` & `csle_collector-0.5.3/src/csle_collector/host_manager/host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/host_manager/host_manager_pb2.py` & `csle_collector-0.5.3/src/csle_collector/host_manager/host_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/host_manager/host_manager_pb2_grpc.py` & `csle_collector-0.5.3/src/csle_collector/host_manager/host_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/host_manager/host_manager_util.py` & `csle_collector-0.5.3/src/csle_collector/host_manager/host_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/host_manager/query_host_manager.py` & `csle_collector-0.5.3/src/csle_collector/host_manager/query_host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/host_manager/threads/host_monitor_thread.py` & `csle_collector-0.5.3/src/csle_collector/host_manager/threads/host_monitor_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/kafka_manager/kafka_manager.py` & `csle_collector-0.5.3/src/csle_collector/kafka_manager/kafka_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/kafka_manager/kafka_manager_pb2.py` & `csle_collector-0.5.3/src/csle_collector/kafka_manager/kafka_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py` & `csle_collector-0.5.3/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/kafka_manager/kafka_manager_util.py` & `csle_collector-0.5.3/src/csle_collector/kafka_manager/kafka_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/kafka_manager/query_kafka_server.py` & `csle_collector-0.5.3/src/csle_collector/kafka_manager/query_kafka_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert.py` & `csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert_counters.py` & `csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py` & `csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py` & `csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py` & `csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py` & `csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py` & `csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ossec_ids_manager/threads/ossec_ids_monitor_thread.py` & `csle_collector-0.5.3/src/csle_collector/ossec_ids_manager/threads/ossec_ids_monitor_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ryu_manager/query_ryu_manager.py` & `csle_collector-0.5.3/src/csle_collector/ryu_manager/query_ryu_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ryu_manager/ryu_manager.py` & `csle_collector-0.5.3/src/csle_collector/ryu_manager/ryu_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ryu_manager/ryu_manager_pb2.py` & `csle_collector-0.5.3/src/csle_collector/ryu_manager/ryu_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py` & `csle_collector-0.5.3/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ryu_manager/ryu_manager_util.py` & `csle_collector-0.5.3/src/csle_collector/ryu_manager/ryu_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/ryu_manager/threads/failure_detector.py` & `csle_collector-0.5.3/src/csle_collector/ryu_manager/threads/failure_detector.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/snort_ids_alert.py` & `csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/snort_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/snort_ids_alert_counters.py` & `csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/snort_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/snort_ids_fast_log_alert.py` & `csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/snort_ids_fast_log_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/snort_ids_ip_alert_counters.py` & `csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/snort_ids_ip_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/snort_ids_manager/dao/snort_ids_rule_counters.py` & `csle_collector-0.5.3/src/csle_collector/snort_ids_manager/dao/snort_ids_rule_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py` & `csle_collector-0.5.3/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/snort_ids_manager/snort_ids_manager.py` & `csle_collector-0.5.3/src/csle_collector/snort_ids_manager/snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py` & `csle_collector-0.5.3/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py` & `csle_collector-0.5.3/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py` & `csle_collector-0.5.3/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/snort_ids_manager/threads/snort_ids_monitor_thread.py` & `csle_collector-0.5.3/src/csle_collector/snort_ids_manager/threads/snort_ids_monitor_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/traffic_manager/query_traffic_manager.py` & `csle_collector-0.5.3/src/csle_collector/traffic_manager/query_traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/traffic_manager/traffic_manager.py` & `csle_collector-0.5.3/src/csle_collector/traffic_manager/traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/traffic_manager/traffic_manager_pb2.py` & `csle_collector-0.5.3/src/csle_collector/traffic_manager/traffic_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py` & `csle_collector-0.5.3/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector/traffic_manager/traffic_manager_util.py` & `csle_collector-0.5.3/src/csle_collector/traffic_manager/traffic_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector.egg-info/PKG-INFO` & `csle_collector-0.5.3/src/csle_collector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-collector
-Version: 0.5.2
+Version: 0.5.3
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.5.2/src/csle_collector.egg-info/SOURCES.txt` & `csle_collector-0.5.3/src/csle_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/src/csle_collector.egg-info/requires.txt` & `csle_collector-0.5.3/src/csle_collector.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-csle-base>=0.5.2
+csle-base>=0.5.3
 grpcio>=1.57.0
 grpcio-tools>=1.57.0
 scipy>=1.0.0
 confluent-kafka>=1.8.2
 docker>=3.0.0
 PyYaml>=5.1.1
 requests>=2.19.0
```

### Comparing `csle_collector-0.5.2/tests/test_client_manager.py` & `csle_collector-0.5.3/tests/test_client_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_client_manager_dao.py` & `csle_collector-0.5.3/tests/test_client_manager_dao.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_docker_stats_manager.py` & `csle_collector-0.5.3/tests/test_docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_docker_stats_manager_dao.py` & `csle_collector-0.5.3/tests/test_docker_stats_manager_dao.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_elk_manager.py` & `csle_collector-0.5.3/tests/test_elk_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_host_manager.py` & `csle_collector-0.5.3/tests/test_host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_host_manager_dao.py` & `csle_collector-0.5.3/tests/test_host_manager_dao.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_kafka_manager.py` & `csle_collector-0.5.3/tests/test_kafka_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_ossec_ids_manager.py` & `csle_collector-0.5.3/tests/test_ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_ossec_ids_manager_dao.py` & `csle_collector-0.5.3/tests/test_ossec_ids_manager_dao.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_ryu_manager.py` & `csle_collector-0.5.3/tests/test_ryu_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_snort_ids_manager.py` & `csle_collector-0.5.3/tests/test_snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_snort_ids_manager_dao.py` & `csle_collector-0.5.3/tests/test_snort_ids_manager_dao.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.5.2/tests/test_traffic_manager.py` & `csle_collector-0.5.3/tests/test_traffic_manager.py`

 * *Files identical despite different names*

