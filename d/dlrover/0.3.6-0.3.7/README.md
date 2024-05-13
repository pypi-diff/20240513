# Comparing `tmp/dlrover-0.3.6-py3-none-any.whl.zip` & `tmp/dlrover-0.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,157 +1,177 @@
-Zip file size: 397277 bytes, number of entries: 236
+Zip file size: 418656 bytes, number of entries: 256
 -rw-r--r--  2.0 unx      411 b- defN 23-Mar-07 11:16 dlrover/Makefile
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/__init__.py
 -rw-r--r--  2.0 unx     4439 b- defN 23-May-08 02:53 dlrover/proto/brain.proto
--rw-r--r--  2.0 unx    12755 b- defN 24-Apr-24 06:10 dlrover/proto/brain_pb2.py
--rw-r--r--  2.0 unx     5867 b- defN 24-Apr-24 06:10 dlrover/proto/brain_pb2_grpc.py
--rw-r--r--  2.0 unx      463 b- defN 23-Nov-21 06:27 dlrover/proto/elastic_training.proto
--rw-r--r--  2.0 unx     1951 b- defN 24-Apr-24 06:10 dlrover/proto/elastic_training_pb2.py
--rw-r--r--  2.0 unx     4164 b- defN 24-Apr-24 06:10 dlrover/proto/elastic_training_pb2_grpc.py
+-rw-r--r--  2.0 unx    12755 b- defN 24-May-13 05:53 dlrover/proto/brain_pb2.py
+-rw-r--r--  2.0 unx     5867 b- defN 24-May-13 05:53 dlrover/proto/brain_pb2_grpc.py
+-rw-r--r--  2.0 unx      424 b- defN 24-May-13 05:21 dlrover/proto/elastic_training.proto
+-rw-r--r--  2.0 unx     1838 b- defN 24-May-13 05:53 dlrover/proto/elastic_training_pb2.py
+-rw-r--r--  2.0 unx     4164 b- defN 24-May-13 05:53 dlrover/proto/elastic_training_pb2_grpc.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/__init__.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/brain/__init__.py
 -rw-r--r--  2.0 unx    11103 b- defN 23-Nov-23 02:06 dlrover/python/brain/client.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/common/__init__.py
--rw-r--r--  2.0 unx     7036 b- defN 24-Mar-26 01:58 dlrover/python/common/constants.py
--rw-r--r--  2.0 unx     1715 b- defN 24-Mar-18 07:49 dlrover/python/common/env_utils.py
+-rw-r--r--  2.0 unx     7195 b- defN 24-May-09 02:02 dlrover/python/common/constants.py
+-rw-r--r--  2.0 unx     2102 b- defN 24-May-09 02:02 dlrover/python/common/diagnosis.py
+-rw-r--r--  2.0 unx     1851 b- defN 24-May-09 02:02 dlrover/python/common/env_utils.py
 -rw-r--r--  2.0 unx     7547 b- defN 24-Mar-21 04:14 dlrover/python/common/global_context.py
--rw-r--r--  2.0 unx     9966 b- defN 24-Apr-16 02:09 dlrover/python/common/grpc.py
+-rw-r--r--  2.0 unx    10181 b- defN 24-May-09 02:02 dlrover/python/common/grpc.py
 -rw-r--r--  2.0 unx     1377 b- defN 23-Nov-21 06:27 dlrover/python/common/log.py
--rw-r--r--  2.0 unx    18440 b- defN 24-Apr-23 06:44 dlrover/python/common/multi_process.py
+-rw-r--r--  2.0 unx    18440 b- defN 24-Apr-29 08:42 dlrover/python/common/multi_process.py
 -rw-r--r--  2.0 unx    11858 b- defN 24-Mar-26 01:58 dlrover/python/common/node.py
 -rw-r--r--  2.0 unx     1186 b- defN 24-Mar-07 06:35 dlrover/python/common/serialize.py
 -rw-r--r--  2.0 unx     1489 b- defN 24-Feb-20 02:57 dlrover/python/common/singleton.py
--rw-r--r--  2.0 unx     8635 b- defN 24-Feb-06 06:42 dlrover/python/common/storage.py
+-rw-r--r--  2.0 unx     9636 b- defN 24-May-09 02:02 dlrover/python/common/storage.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/__init__.py
--rw-r--r--  2.0 unx    14237 b- defN 24-Apr-23 06:44 dlrover/python/elastic_agent/master_client.py
+-rw-r--r--  2.0 unx    14808 b- defN 24-May-09 02:02 dlrover/python/elastic_agent/master_client.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Nov-21 06:27 dlrover/python/elastic_agent/config/__init__.py
 -rw-r--r--  2.0 unx     3717 b- defN 24-Feb-20 02:57 dlrover/python/elastic_agent/config/paral_config_tuner.py
+-rw-r--r--  2.0 unx      599 b- defN 24-May-09 02:02 dlrover/python/elastic_agent/datacollector/__init__.py
+-rw-r--r--  2.0 unx      983 b- defN 24-May-09 02:02 dlrover/python/elastic_agent/datacollector/cuda_log_collector.py
+-rw-r--r--  2.0 unx     1124 b- defN 24-May-09 02:02 dlrover/python/elastic_agent/datacollector/data_collector.py
+-rw-r--r--  2.0 unx      987 b- defN 24-May-09 02:02 dlrover/python/elastic_agent/datacollector/log_collector.py
+-rw-r--r--  2.0 unx     1009 b- defN 24-May-09 02:02 dlrover/python/elastic_agent/datacollector/metrics_collector.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/monitor/__init__.py
+-rw-r--r--  2.0 unx     3768 b- defN 24-May-09 02:02 dlrover/python/elastic_agent/monitor/diagnosis.py
 -rw-r--r--  2.0 unx     5980 b- defN 24-Mar-05 07:05 dlrover/python/elastic_agent/monitor/resource.py
 -rw-r--r--  2.0 unx     4659 b- defN 24-Mar-26 09:59 dlrover/python/elastic_agent/monitor/training.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/sharding/__init__.py
 -rw-r--r--  2.0 unx    11734 b- defN 24-Feb-06 01:58 dlrover/python/elastic_agent/sharding/client.py
 -rw-r--r--  2.0 unx      599 b- defN 23-May-08 02:53 dlrover/python/elastic_agent/sychronization/__init__.py
 -rw-r--r--  2.0 unx     2686 b- defN 23-Nov-23 02:06 dlrover/python/elastic_agent/sychronization/sync_client.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/tensorflow/__init__.py
 -rw-r--r--  2.0 unx     3424 b- defN 24-Feb-06 01:58 dlrover/python/elastic_agent/tensorflow/elastic_ps.py
 -rw-r--r--  2.0 unx     4226 b- defN 24-Feb-06 01:58 dlrover/python/elastic_agent/tensorflow/hooks.py
 -rw-r--r--  2.0 unx     4556 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/tensorflow/profile_extractor.py
 -rw-r--r--  2.0 unx      599 b- defN 23-May-08 02:53 dlrover/python/elastic_agent/torch/__init__.py
--rw-r--r--  2.0 unx    40769 b- defN 24-Apr-23 06:44 dlrover/python/elastic_agent/torch/ckpt_saver.py
+-rw-r--r--  2.0 unx    40977 b- defN 24-May-09 02:02 dlrover/python/elastic_agent/torch/ckpt_saver.py
 -rw-r--r--  2.0 unx     4594 b- defN 23-Nov-23 02:06 dlrover/python/elastic_agent/torch/master_kv_store.py
--rw-r--r--  2.0 unx    39591 b- defN 24-Apr-23 06:44 dlrover/python/elastic_agent/torch/training.py
+-rw-r--r--  2.0 unx    40001 b- defN 24-May-09 02:02 dlrover/python/elastic_agent/torch/training.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/__init__.py
 -rw-r--r--  2.0 unx     3044 b- defN 24-Mar-28 12:07 dlrover/python/master/args.py
 -rw-r--r--  2.0 unx    11296 b- defN 24-Apr-01 02:41 dlrover/python/master/dist_master.py
--rw-r--r--  2.0 unx     4416 b- defN 24-Apr-18 06:28 dlrover/python/master/local_master.py
+-rw-r--r--  2.0 unx     4416 b- defN 24-Apr-29 04:18 dlrover/python/master/local_master.py
 -rw-r--r--  2.0 unx     2550 b- defN 24-Mar-05 07:32 dlrover/python/master/main.py
 -rw-r--r--  2.0 unx      928 b- defN 23-Nov-21 06:27 dlrover/python/master/master.py
--rw-r--r--  2.0 unx    23356 b- defN 24-Apr-17 05:53 dlrover/python/master/servicer.py
+-rw-r--r--  2.0 unx    25426 b- defN 24-May-09 02:02 dlrover/python/master/servicer.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Nov-07 07:11 dlrover/python/master/cluster/__init__.py
 -rw-r--r--  2.0 unx     1124 b- defN 23-Nov-07 07:11 dlrover/python/master/cluster/quota.py
+-rw-r--r--  2.0 unx      599 b- defN 24-May-09 02:02 dlrover/python/master/diagnosis/__init__.py
+-rw-r--r--  2.0 unx     2665 b- defN 24-May-09 02:02 dlrover/python/master/diagnosis/diagnosis.py
+-rw-r--r--  2.0 unx     2068 b- defN 24-May-09 02:02 dlrover/python/master/diagnosis/diagnosis_data.py
+-rw-r--r--  2.0 unx     1369 b- defN 24-May-09 02:02 dlrover/python/master/diagnosis/diagnostician.py
+-rw-r--r--  2.0 unx      599 b- defN 24-May-09 02:02 dlrover/python/master/diagnosis/inferencechain/__init__.py
+-rw-r--r--  2.0 unx     2313 b- defN 24-May-09 02:02 dlrover/python/master/diagnosis/inferencechain/common.py
+-rw-r--r--  2.0 unx     2398 b- defN 24-May-09 02:02 dlrover/python/master/diagnosis/inferencechain/inference_chain.py
+-rw-r--r--  2.0 unx      599 b- defN 24-May-09 02:02 dlrover/python/master/diagnosis/operator/__init__.py
+-rw-r--r--  2.0 unx     1592 b- defN 24-May-09 02:02 dlrover/python/master/diagnosis/operator/check_training_hang_operator.py
+-rw-r--r--  2.0 unx     1053 b- defN 24-May-09 02:02 dlrover/python/master/diagnosis/operator/operator.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/elastic_training/__init__.py
 -rw-r--r--  2.0 unx     3494 b- defN 23-Mar-07 11:16 dlrover/python/master/elastic_training/elastic_ps.py
 -rw-r--r--  2.0 unx     1017 b- defN 23-Nov-07 07:11 dlrover/python/master/elastic_training/kv_store_service.py
--rw-r--r--  2.0 unx     2852 b- defN 24-Apr-23 06:44 dlrover/python/master/elastic_training/net_topology.py
--rw-r--r--  2.0 unx    22102 b- defN 24-Apr-23 06:44 dlrover/python/master/elastic_training/rdzv_manager.py
+-rw-r--r--  2.0 unx     2852 b- defN 24-Apr-29 08:42 dlrover/python/master/elastic_training/net_topology.py
+-rw-r--r--  2.0 unx    22102 b- defN 24-Apr-29 08:42 dlrover/python/master/elastic_training/rdzv_manager.py
 -rw-r--r--  2.0 unx     4971 b- defN 23-Nov-21 06:27 dlrover/python/master/elastic_training/sync_service.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Nov-21 06:27 dlrover/python/master/hyperparams/__init__.py
 -rw-r--r--  2.0 unx     6818 b- defN 24-Feb-06 01:58 dlrover/python/master/hyperparams/simple_strategy_generator.py
 -rw-r--r--  2.0 unx     1000 b- defN 23-Nov-21 06:27 dlrover/python/master/hyperparams/strategy_generator.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/monitor/__init__.py
--rw-r--r--  2.0 unx     4490 b- defN 24-Mar-26 01:58 dlrover/python/master/monitor/error_monitor.py
+-rw-r--r--  2.0 unx     4490 b- defN 24-May-06 08:09 dlrover/python/master/monitor/error_monitor.py
 -rw-r--r--  2.0 unx     7384 b- defN 24-Mar-29 02:24 dlrover/python/master/monitor/speed_monitor.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/node/__init__.py
--rw-r--r--  2.0 unx    34327 b- defN 24-Apr-23 06:44 dlrover/python/master/node/dist_job_manager.py
--rw-r--r--  2.0 unx    13001 b- defN 24-Mar-26 01:58 dlrover/python/master/node/event_callback.py
+-rw-r--r--  2.0 unx    34327 b- defN 24-Apr-29 08:42 dlrover/python/master/node/dist_job_manager.py
+-rw-r--r--  2.0 unx    13075 b- defN 24-May-09 02:02 dlrover/python/master/node/event_callback.py
 -rw-r--r--  2.0 unx    12665 b- defN 23-Dec-13 06:11 dlrover/python/master/node/job_auto_scaler.py
 -rw-r--r--  2.0 unx     3661 b- defN 24-Mar-04 05:56 dlrover/python/master/node/job_manager.py
 -rw-r--r--  2.0 unx     5342 b- defN 24-Mar-12 05:23 dlrover/python/master/node/local_job_manager.py
 -rw-r--r--  2.0 unx    14448 b- defN 23-Dec-21 04:12 dlrover/python/master/node/ps.py
 -rw-r--r--  2.0 unx     4094 b- defN 23-Nov-21 06:27 dlrover/python/master/node/status_flow.py
 -rw-r--r--  2.0 unx    13398 b- defN 23-Dec-21 04:12 dlrover/python/master/node/training_node.py
--rw-r--r--  2.0 unx    11300 b- defN 24-Apr-23 06:44 dlrover/python/master/node/worker.py
+-rw-r--r--  2.0 unx    11300 b- defN 24-Apr-29 08:42 dlrover/python/master/node/worker.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/resource/__init__.py
 -rw-r--r--  2.0 unx     4187 b- defN 23-May-08 02:53 dlrover/python/master/resource/brain_optimizer.py
 -rw-r--r--  2.0 unx    21672 b- defN 24-Feb-23 09:24 dlrover/python/master/resource/job.py
 -rw-r--r--  2.0 unx    15828 b- defN 24-Feb-06 01:58 dlrover/python/master/resource/local_optimizer.py
 -rw-r--r--  2.0 unx     6187 b- defN 23-Nov-21 06:27 dlrover/python/master/resource/optimizer.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/scaler/__init__.py
 -rw-r--r--  2.0 unx     2202 b- defN 23-Nov-23 02:06 dlrover/python/master/scaler/base_scaler.py
 -rw-r--r--  2.0 unx     8541 b- defN 23-Nov-23 02:06 dlrover/python/master/scaler/elasticjob_scaler.py
 -rw-r--r--  2.0 unx     1370 b- defN 23-Nov-21 06:27 dlrover/python/master/scaler/factory.py
--rw-r--r--  2.0 unx    24649 b- defN 24-Apr-16 02:09 dlrover/python/master/scaler/pod_scaler.py
+-rw-r--r--  2.0 unx    25968 b- defN 24-May-09 02:02 dlrover/python/master/scaler/pod_scaler.py
 -rw-r--r--  2.0 unx     4659 b- defN 23-Nov-23 02:06 dlrover/python/master/scaler/ray_scaler.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/shard/__init__.py
 -rw-r--r--  2.0 unx     4574 b- defN 23-Nov-07 07:11 dlrover/python/master/shard/base_dataset_manager.py
 -rw-r--r--  2.0 unx     6964 b- defN 23-Nov-07 07:11 dlrover/python/master/shard/batch_dataset_manager.py
 -rw-r--r--  2.0 unx    16305 b- defN 24-Jan-30 06:31 dlrover/python/master/shard/dataset_splitter.py
 -rw-r--r--  2.0 unx     7064 b- defN 24-Jan-11 07:28 dlrover/python/master/shard/streaming_dataset_manager.py
--rw-r--r--  2.0 unx    11152 b- defN 24-Apr-01 02:35 dlrover/python/master/shard/task_manager.py
+-rw-r--r--  2.0 unx    11152 b- defN 24-Apr-29 04:18 dlrover/python/master/shard/task_manager.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/stats/__init__.py
--rw-r--r--  2.0 unx     6444 b- defN 23-Nov-21 06:27 dlrover/python/master/stats/job_collector.py
+-rw-r--r--  2.0 unx     6683 b- defN 24-May-09 02:02 dlrover/python/master/stats/job_collector.py
 -rw-r--r--  2.0 unx     8776 b- defN 24-Feb-20 02:57 dlrover/python/master/stats/reporter.py
 -rw-r--r--  2.0 unx     1567 b- defN 23-Mar-07 11:16 dlrover/python/master/stats/stats_backend.py
 -rw-r--r--  2.0 unx     4820 b- defN 23-Nov-21 06:27 dlrover/python/master/stats/training_metrics.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/watcher/__init__.py
 -rw-r--r--  2.0 unx     1241 b- defN 23-Mar-07 11:16 dlrover/python/master/watcher/base_watcher.py
 -rw-r--r--  2.0 unx     1906 b- defN 23-Nov-21 06:27 dlrover/python/master/watcher/factory.py
--rw-r--r--  2.0 unx    11775 b- defN 24-Mar-28 09:11 dlrover/python/master/watcher/k8s_watcher.py
+-rw-r--r--  2.0 unx    11775 b- defN 24-May-13 02:02 dlrover/python/master/watcher/k8s_watcher.py
 -rw-r--r--  2.0 unx     3247 b- defN 23-Mar-07 11:16 dlrover/python/master/watcher/ray_watcher.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/scheduler/__init__.py
 -rw-r--r--  2.0 unx     1924 b- defN 23-Nov-21 06:27 dlrover/python/scheduler/factory.py
 -rw-r--r--  2.0 unx     4285 b- defN 24-Mar-29 02:24 dlrover/python/scheduler/job.py
 -rw-r--r--  2.0 unx    18558 b- defN 24-Mar-29 02:24 dlrover/python/scheduler/kubernetes.py
 -rw-r--r--  2.0 unx     7397 b- defN 23-Nov-21 06:27 dlrover/python/scheduler/ray.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/tests/__init__.py
 -rw-r--r--  2.0 unx     2799 b- defN 24-Feb-06 01:58 dlrover/python/tests/test_agent_config_tuner.py
--rw-r--r--  2.0 unx     3405 b- defN 24-Apr-18 06:18 dlrover/python/tests/test_agent_monitor.py
+-rw-r--r--  2.0 unx     4236 b- defN 24-May-09 02:02 dlrover/python/tests/test_agent_monitor.py
 -rw-r--r--  2.0 unx     1049 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_args.py
--rw-r--r--  2.0 unx    10521 b- defN 24-Apr-23 06:44 dlrover/python/tests/test_ckpt_saver.py
+-rw-r--r--  2.0 unx    10521 b- defN 24-Apr-29 08:42 dlrover/python/tests/test_ckpt_saver.py
 -rw-r--r--  2.0 unx     4583 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_dataset_splitter.py
 -rw-r--r--  2.0 unx     4905 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_dataset_task_manager.py
--rw-r--r--  2.0 unx    14928 b- defN 24-Apr-23 06:44 dlrover/python/tests/test_elastic_training_agent.py
+-rw-r--r--  2.0 unx     2128 b- defN 24-May-09 02:02 dlrover/python/tests/test_diagnosis.py
+-rw-r--r--  2.0 unx    14958 b- defN 24-May-09 02:02 dlrover/python/tests/test_elastic_training_agent.py
 -rw-r--r--  2.0 unx     3383 b- defN 23-Nov-23 02:06 dlrover/python/tests/test_elasticjob_scaler.py
 -rw-r--r--  2.0 unx     1873 b- defN 23-Dec-22 03:13 dlrover/python/tests/test_env_utils.py
 -rw-r--r--  2.0 unx     1527 b- defN 24-Mar-12 05:23 dlrover/python/tests/test_error_monitor.py
 -rw-r--r--  2.0 unx     3635 b- defN 24-Mar-26 01:58 dlrover/python/tests/test_event_callback.py
 -rw-r--r--  2.0 unx     1268 b- defN 23-Nov-23 02:06 dlrover/python/tests/test_global_context.py
 -rw-r--r--  2.0 unx     2158 b- defN 23-Dec-26 03:16 dlrover/python/tests/test_grpc_utils.py
 -rw-r--r--  2.0 unx     5292 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_job_auto_scaler.py
 -rw-r--r--  2.0 unx    21350 b- defN 24-Mar-21 07:24 dlrover/python/tests/test_job_manager.py
 -rw-r--r--  2.0 unx     2183 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_job_params.py
+-rw-r--r--  2.0 unx     1391 b- defN 24-May-09 02:02 dlrover/python/tests/test_k8s_util.py
 -rw-r--r--  2.0 unx     3188 b- defN 24-Mar-12 05:23 dlrover/python/tests/test_k8s_utils.py
 -rw-r--r--  2.0 unx     5920 b- defN 24-Feb-20 02:57 dlrover/python/tests/test_k8s_watcher.py
 -rw-r--r--  2.0 unx     9142 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_local_optimizer.py
 -rw-r--r--  2.0 unx     5449 b- defN 24-Mar-05 07:32 dlrover/python/tests/test_master.py
--rw-r--r--  2.0 unx     5455 b- defN 24-Apr-16 02:09 dlrover/python/tests/test_master_client.py
--rw-r--r--  2.0 unx     3773 b- defN 24-Apr-23 06:44 dlrover/python/tests/test_multi_process.py
--rw-r--r--  2.0 unx     1816 b- defN 24-Apr-23 06:44 dlrover/python/tests/test_net_topology.py
+-rw-r--r--  2.0 unx     5455 b- defN 24-Apr-29 04:18 dlrover/python/tests/test_master_client.py
+-rw-r--r--  2.0 unx     3773 b- defN 24-Apr-29 08:42 dlrover/python/tests/test_multi_process.py
+-rw-r--r--  2.0 unx     1816 b- defN 24-Apr-29 08:42 dlrover/python/tests/test_net_topology.py
 -rw-r--r--  2.0 unx     1943 b- defN 24-Feb-21 09:03 dlrover/python/tests/test_node.py
--rw-r--r--  2.0 unx     9506 b- defN 24-Apr-16 02:09 dlrover/python/tests/test_pod_scaler.py
+-rw-r--r--  2.0 unx    10099 b- defN 24-May-09 02:02 dlrover/python/tests/test_pod_scaler.py
 -rw-r--r--  2.0 unx     7411 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_ps_manager.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_ray_client.py
 -rw-r--r--  2.0 unx     1976 b- defN 23-Nov-23 02:06 dlrover/python/tests/test_ray_job_args.py
 -rw-r--r--  2.0 unx      971 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_ray_scaler.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_ray_watcher.py
--rw-r--r--  2.0 unx    12564 b- defN 24-Apr-16 02:09 dlrover/python/tests/test_rdzv_manager.py
+-rw-r--r--  2.0 unx    12564 b- defN 24-Apr-29 04:18 dlrover/python/tests/test_rdzv_manager.py
 -rw-r--r--  2.0 unx    11635 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_resource_optimizer.py
--rw-r--r--  2.0 unx    18420 b- defN 24-Apr-09 01:37 dlrover/python/tests/test_servicer.py
+-rw-r--r--  2.0 unx    18420 b- defN 24-Apr-29 04:18 dlrover/python/tests/test_servicer.py
 -rw-r--r--  2.0 unx     3687 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_sharding_client.py
 -rw-r--r--  2.0 unx     1783 b- defN 24-Apr-01 02:29 dlrover/python/tests/test_speed_monitor.py
 -rw-r--r--  2.0 unx     1344 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_state_backend.py
--rw-r--r--  2.0 unx     3287 b- defN 24-Feb-06 01:58 dlrover/python/tests/test_stats_collector.py
--rw-r--r--  2.0 unx     2703 b- defN 24-Feb-06 06:42 dlrover/python/tests/test_storage.py
+-rw-r--r--  2.0 unx     3535 b- defN 24-May-09 02:02 dlrover/python/tests/test_stats_collector.py
+-rw-r--r--  2.0 unx     3497 b- defN 24-May-09 02:02 dlrover/python/tests/test_storage.py
 -rw-r--r--  2.0 unx     3303 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_strategy_generator.py
 -rw-r--r--  2.0 unx     2460 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_sync_service.py
 -rw-r--r--  2.0 unx     5425 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_task_manager.py
--rw-r--r--  2.0 unx     8599 b- defN 24-Apr-18 06:28 dlrover/python/tests/test_utils.py
--rw-r--r--  2.0 unx     7354 b- defN 24-Apr-23 06:44 dlrover/python/tests/test_worker_manager.py
+-rw-r--r--  2.0 unx     9310 b- defN 24-May-09 02:02 dlrover/python/tests/test_utils.py
+-rw-r--r--  2.0 unx     7354 b- defN 24-Apr-29 08:42 dlrover/python/tests/test_worker_manager.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/__init__.py
+-rw-r--r--  2.0 unx     1169 b- defN 24-May-09 02:02 dlrover/python/util/k8s_util.py
 -rw-r--r--  2.0 unx     3856 b- defN 23-Mar-07 11:16 dlrover/python/util/reflect_util.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/actor_util/__init__.py
 -rw-r--r--  2.0 unx     1552 b- defN 23-Mar-07 11:16 dlrover/python/util/actor_util/parse_actor.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/queue/__init__.py
 -rw-r--r--  2.0 unx     2834 b- defN 23-Mar-07 11:16 dlrover/python/util/queue/queue.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/state/__init__.py
 -rw-r--r--  2.0 unx     2322 b- defN 23-Mar-07 11:16 dlrover/python/util/state/memory_store.py
@@ -193,46 +213,46 @@
 -rw-r--r--  2.0 unx     5429 b- defN 23-Nov-07 07:11 dlrover/trainer/tensorflow/util/dataset_util.py
 -rw-r--r--  2.0 unx     8506 b- defN 23-Nov-07 07:11 dlrover/trainer/tensorflow/util/estimator_util.py
 -rw-r--r--  2.0 unx     1122 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/util/path_util.py
 -rw-r--r--  2.0 unx     1598 b- defN 23-May-08 02:53 dlrover/trainer/tensorflow/util/tf_env_util.py
 -rw-r--r--  2.0 unx    15226 b- defN 23-Nov-07 07:11 dlrover/trainer/tensorflow/util/tf_patch_util.py
 -rw-r--r--  2.0 unx     1104 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/util/tf_version_util.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Jun-30 07:14 dlrover/trainer/torch/__init__.py
--rw-r--r--  2.0 unx    11832 b- defN 24-Apr-18 02:40 dlrover/trainer/torch/elastic_run.py
+-rw-r--r--  2.0 unx    12051 b- defN 24-May-13 05:21 dlrover/trainer/torch/elastic_run.py
 -rw-r--r--  2.0 unx      690 b- defN 23-Nov-07 07:11 dlrover/trainer/torch/main.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Nov-21 06:27 dlrover/trainer/torch/elastic/__init__.py
 -rw-r--r--  2.0 unx     5422 b- defN 23-Nov-21 06:27 dlrover/trainer/torch/elastic/dataloader.py
 -rw-r--r--  2.0 unx     5981 b- defN 24-Apr-09 12:05 dlrover/trainer/torch/elastic/sampler.py
 -rw-r--r--  2.0 unx    11244 b- defN 24-Mar-26 08:26 dlrover/trainer/torch/elastic/trainer.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Dec-22 03:13 dlrover/trainer/torch/flash_checkpoint/__init__.py
--rw-r--r--  2.0 unx     2534 b- defN 24-Jan-10 08:04 dlrover/trainer/torch/flash_checkpoint/checkpointer.py
--rw-r--r--  2.0 unx     4247 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/ddp.py
--rw-r--r--  2.0 unx     8646 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/deepspeed.py
--rw-r--r--  2.0 unx     6280 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/deepspeed_engine.py
--rw-r--r--  2.0 unx    14280 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/engine.py
--rw-r--r--  2.0 unx    10397 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/fsdp.py
--rw-r--r--  2.0 unx    19976 b- defN 24-Feb-01 02:40 dlrover/trainer/torch/flash_checkpoint/fsdp_engine.py
--rw-r--r--  2.0 unx     7885 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/full_ckpt_engine.py
--rw-r--r--  2.0 unx    14246 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/hf_trainer.py
--rw-r--r--  2.0 unx     7823 b- defN 24-Feb-20 02:57 dlrover/trainer/torch/flash_checkpoint/megatron.py
--rw-r--r--  2.0 unx    20464 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/megatron_dist_ckpt.py
--rw-r--r--  2.0 unx     9626 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/megatron_engine.py
+-rw-r--r--  2.0 unx     2534 b- defN 24-Apr-29 02:56 dlrover/trainer/torch/flash_checkpoint/checkpointer.py
+-rw-r--r--  2.0 unx     4827 b- defN 24-May-09 02:02 dlrover/trainer/torch/flash_checkpoint/ddp.py
+-rw-r--r--  2.0 unx     9239 b- defN 24-May-09 02:02 dlrover/trainer/torch/flash_checkpoint/deepspeed.py
+-rw-r--r--  2.0 unx     6221 b- defN 24-May-09 02:02 dlrover/trainer/torch/flash_checkpoint/deepspeed_engine.py
+-rw-r--r--  2.0 unx    14498 b- defN 24-May-09 02:02 dlrover/trainer/torch/flash_checkpoint/engine.py
+-rw-r--r--  2.0 unx    10902 b- defN 24-May-09 02:02 dlrover/trainer/torch/flash_checkpoint/fsdp.py
+-rw-r--r--  2.0 unx    20083 b- defN 24-May-09 02:02 dlrover/trainer/torch/flash_checkpoint/fsdp_engine.py
+-rw-r--r--  2.0 unx     7953 b- defN 24-May-09 02:02 dlrover/trainer/torch/flash_checkpoint/full_ckpt_engine.py
+-rw-r--r--  2.0 unx    14246 b- defN 24-Apr-29 09:21 dlrover/trainer/torch/flash_checkpoint/hf_trainer.py
+-rw-r--r--  2.0 unx     8159 b- defN 24-May-09 02:02 dlrover/trainer/torch/flash_checkpoint/megatron.py
+-rw-r--r--  2.0 unx    25238 b- defN 24-May-09 02:02 dlrover/trainer/torch/flash_checkpoint/megatron_dist_ckpt.py
+-rw-r--r--  2.0 unx     9903 b- defN 24-May-09 02:02 dlrover/trainer/torch/flash_checkpoint/megatron_engine.py
 -rw-r--r--  2.0 unx      599 b- defN 24-Mar-11 07:21 dlrover/trainer/torch/node_check/__init__.py
 -rw-r--r--  2.0 unx     1645 b- defN 24-Mar-12 05:23 dlrover/trainer/torch/node_check/ascend_npu.py
 -rw-r--r--  2.0 unx     1373 b- defN 24-Mar-12 05:23 dlrover/trainer/torch/node_check/nvidia_gpu.py
--rw-r--r--  2.0 unx     2890 b- defN 24-Apr-18 07:29 dlrover/trainer/torch/node_check/utils.py
+-rw-r--r--  2.0 unx     2930 b- defN 24-May-13 05:53 dlrover/trainer/torch/node_check/utils.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/util/__init__.py
 -rw-r--r--  2.0 unx     2031 b- defN 23-Mar-07 11:16 dlrover/trainer/util/args_util.py
 -rw-r--r--  2.0 unx     6436 b- defN 24-Feb-20 02:57 dlrover/trainer/util/conf_util.py
 -rw-r--r--  2.0 unx     2863 b- defN 23-Mar-07 11:16 dlrover/trainer/util/log_util.py
 -rw-r--r--  2.0 unx      736 b- defN 23-Mar-07 11:16 dlrover/trainer/util/net_util.py
 -rw-r--r--  2.0 unx     3860 b- defN 23-Mar-07 11:16 dlrover/trainer/util/reflect_util.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/worker/__init__.py
 -rw-r--r--  2.0 unx     3540 b- defN 23-Nov-07 07:11 dlrover/trainer/worker/tf_kubernetes_worker.py
 -rw-r--r--  2.0 unx     6927 b- defN 23-Nov-23 02:06 dlrover/trainer/worker/tf_ray_worker.py
--rw-r--r--  2.0 unx    13484 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1008 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    23241 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/RECORD
-236 files, 1269758 bytes uncompressed, 359585 bytes compressed:  71.7%
+-rw-r--r--  2.0 unx    13484 b- defN 24-May-13 05:53 dlrover-0.3.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1008 b- defN 24-May-13 05:53 dlrover-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 05:53 dlrover-0.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 24-May-13 05:53 dlrover-0.3.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-May-13 05:53 dlrover-0.3.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    25405 b- defN 24-May-13 05:54 dlrover-0.3.7.dist-info/RECORD
+256 files, 1319552 bytes uncompressed, 377388 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -33,14 +33,17 @@
 
 Filename: dlrover/python/common/__init__.py
 Comment: 
 
 Filename: dlrover/python/common/constants.py
 Comment: 
 
+Filename: dlrover/python/common/diagnosis.py
+Comment: 
+
 Filename: dlrover/python/common/env_utils.py
 Comment: 
 
 Filename: dlrover/python/common/global_context.py
 Comment: 
 
 Filename: dlrover/python/common/grpc.py
@@ -72,17 +75,35 @@
 
 Filename: dlrover/python/elastic_agent/config/__init__.py
 Comment: 
 
 Filename: dlrover/python/elastic_agent/config/paral_config_tuner.py
 Comment: 
 
+Filename: dlrover/python/elastic_agent/datacollector/__init__.py
+Comment: 
+
+Filename: dlrover/python/elastic_agent/datacollector/cuda_log_collector.py
+Comment: 
+
+Filename: dlrover/python/elastic_agent/datacollector/data_collector.py
+Comment: 
+
+Filename: dlrover/python/elastic_agent/datacollector/log_collector.py
+Comment: 
+
+Filename: dlrover/python/elastic_agent/datacollector/metrics_collector.py
+Comment: 
+
 Filename: dlrover/python/elastic_agent/monitor/__init__.py
 Comment: 
 
+Filename: dlrover/python/elastic_agent/monitor/diagnosis.py
+Comment: 
+
 Filename: dlrover/python/elastic_agent/monitor/resource.py
 Comment: 
 
 Filename: dlrover/python/elastic_agent/monitor/training.py
 Comment: 
 
 Filename: dlrover/python/elastic_agent/sharding/__init__.py
@@ -144,14 +165,44 @@
 
 Filename: dlrover/python/master/cluster/__init__.py
 Comment: 
 
 Filename: dlrover/python/master/cluster/quota.py
 Comment: 
 
+Filename: dlrover/python/master/diagnosis/__init__.py
+Comment: 
+
+Filename: dlrover/python/master/diagnosis/diagnosis.py
+Comment: 
+
+Filename: dlrover/python/master/diagnosis/diagnosis_data.py
+Comment: 
+
+Filename: dlrover/python/master/diagnosis/diagnostician.py
+Comment: 
+
+Filename: dlrover/python/master/diagnosis/inferencechain/__init__.py
+Comment: 
+
+Filename: dlrover/python/master/diagnosis/inferencechain/common.py
+Comment: 
+
+Filename: dlrover/python/master/diagnosis/inferencechain/inference_chain.py
+Comment: 
+
+Filename: dlrover/python/master/diagnosis/operator/__init__.py
+Comment: 
+
+Filename: dlrover/python/master/diagnosis/operator/check_training_hang_operator.py
+Comment: 
+
+Filename: dlrover/python/master/diagnosis/operator/operator.py
+Comment: 
+
 Filename: dlrover/python/master/elastic_training/__init__.py
 Comment: 
 
 Filename: dlrover/python/master/elastic_training/elastic_ps.py
 Comment: 
 
 Filename: dlrover/python/master/elastic_training/kv_store_service.py
@@ -327,14 +378,17 @@
 
 Filename: dlrover/python/tests/test_dataset_splitter.py
 Comment: 
 
 Filename: dlrover/python/tests/test_dataset_task_manager.py
 Comment: 
 
+Filename: dlrover/python/tests/test_diagnosis.py
+Comment: 
+
 Filename: dlrover/python/tests/test_elastic_training_agent.py
 Comment: 
 
 Filename: dlrover/python/tests/test_elasticjob_scaler.py
 Comment: 
 
 Filename: dlrover/python/tests/test_env_utils.py
@@ -357,14 +411,17 @@
 
 Filename: dlrover/python/tests/test_job_manager.py
 Comment: 
 
 Filename: dlrover/python/tests/test_job_params.py
 Comment: 
 
+Filename: dlrover/python/tests/test_k8s_util.py
+Comment: 
+
 Filename: dlrover/python/tests/test_k8s_utils.py
 Comment: 
 
 Filename: dlrover/python/tests/test_k8s_watcher.py
 Comment: 
 
 Filename: dlrover/python/tests/test_local_optimizer.py
@@ -441,14 +498,17 @@
 
 Filename: dlrover/python/tests/test_worker_manager.py
 Comment: 
 
 Filename: dlrover/python/util/__init__.py
 Comment: 
 
+Filename: dlrover/python/util/k8s_util.py
+Comment: 
+
 Filename: dlrover/python/util/reflect_util.py
 Comment: 
 
 Filename: dlrover/python/util/actor_util/__init__.py
 Comment: 
 
 Filename: dlrover/python/util/actor_util/parse_actor.py
@@ -684,26 +744,26 @@
 
 Filename: dlrover/trainer/worker/tf_kubernetes_worker.py
 Comment: 
 
 Filename: dlrover/trainer/worker/tf_ray_worker.py
 Comment: 
 
-Filename: dlrover-0.3.6.dist-info/LICENSE
+Filename: dlrover-0.3.7.dist-info/LICENSE
 Comment: 
 
-Filename: dlrover-0.3.6.dist-info/METADATA
+Filename: dlrover-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: dlrover-0.3.6.dist-info/WHEEL
+Filename: dlrover-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: dlrover-0.3.6.dist-info/entry_points.txt
+Filename: dlrover-0.3.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: dlrover-0.3.6.dist-info/top_level.txt
+Filename: dlrover-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: dlrover-0.3.6.dist-info/RECORD
+Filename: dlrover-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dlrover/proto/elastic_training.proto

```diff
@@ -1,13 +1,11 @@
 syntax = "proto3";
 
 package elastic;
 
-import "google/protobuf/empty.proto";
-
 enum TaskType {
   NONE = 0;
   TRAINING = 1;
   EVALUATION = 2;
   PREDICTION = 3;
   WAIT = 4;
   TRAIN_END_CALLBACK = 5;
```

## dlrover/proto/elastic_training_pb2.py

```diff
@@ -7,27 +7,26 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$dlrover/proto/elastic_training.proto\x12\x07\x65lastic\x1a\x1bgoogle/protobuf/empty.proto\"+\n\x08Response\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0e\n\x06reason\x18\x02 \x01(\t\";\n\x07Message\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\x12\x11\n\tnode_type\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c*d\n\x08TaskType\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nEVALUATION\x10\x02\x12\x0e\n\nPREDICTION\x10\x03\x12\x08\n\x04WAIT\x10\x04\x12\x16\n\x12TRAIN_END_CALLBACK\x10\x05\x32\x62\n\x06Master\x12-\n\x06report\x12\x10.elastic.Message\x1a\x11.elastic.Response\x12)\n\x03get\x12\x10.elastic.Message\x1a\x10.elastic.Messageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$dlrover/proto/elastic_training.proto\x12\x07\x65lastic\"+\n\x08Response\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0e\n\x06reason\x18\x02 \x01(\t\";\n\x07Message\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\x12\x11\n\tnode_type\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c*d\n\x08TaskType\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nEVALUATION\x10\x02\x12\x0e\n\nPREDICTION\x10\x03\x12\x08\n\x04WAIT\x10\x04\x12\x16\n\x12TRAIN_END_CALLBACK\x10\x05\x32\x62\n\x06Master\x12-\n\x06report\x12\x10.elastic.Message\x1a\x11.elastic.Response\x12)\n\x03get\x12\x10.elastic.Message\x1a\x10.elastic.Messageb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dlrover.proto.elastic_training_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _globals['_TASKTYPE']._serialized_start=184
-  _globals['_TASKTYPE']._serialized_end=284
-  _globals['_RESPONSE']._serialized_start=78
-  _globals['_RESPONSE']._serialized_end=121
-  _globals['_MESSAGE']._serialized_start=123
-  _globals['_MESSAGE']._serialized_end=182
-  _globals['_MASTER']._serialized_start=286
-  _globals['_MASTER']._serialized_end=384
+  _globals['_TASKTYPE']._serialized_start=155
+  _globals['_TASKTYPE']._serialized_end=255
+  _globals['_RESPONSE']._serialized_start=49
+  _globals['_RESPONSE']._serialized_end=92
+  _globals['_MESSAGE']._serialized_start=94
+  _globals['_MESSAGE']._serialized_end=153
+  _globals['_MASTER']._serialized_start=257
+  _globals['_MASTER']._serialized_end=355
 # @@protoc_insertion_point(module_scope)
```

## dlrover/python/common/constants.py

```diff
@@ -99,14 +99,20 @@
     WORKER_ERROR = "WorkerError"
     PS_OOM_ERROR = "PSOOM"
     PS_ERROR = "PSError"
     EVALUATOR_OOM = "EvaluatorOOM"
     EVALUATOR_ERROR = "EvaluatorError"
     UNKNOWN_ERROR = "UnknownError"
     HANG_ERROR = "HangError"
+    RDZV_TIMEOUT_ERROR = "RdzvTimeout"
+
+
+class CustomMetricKeys:
+    RDZV_ROUND = "rdzv_round"
+    TRAINING_ERROR_LEVEL = "error_level"
 
 
 class ExitCode(object):
     FATAL_ERROR_CODE = 1
     KILLED_CODE = 137
     TERMED_CODE = 143
     CORE_DUMP_ERROR_CODE = 134
@@ -280,12 +286,13 @@
     NETWORK_CHECK_DATA_DIR = "/tmp/dlrover/network_check/"
 
 
 class CheckpointConstant(object):
     TRACER_FILE_NAME = "dlrover_latest.txt"
     MODEL_STATES_NAME = "model_states"
     OPTIM_STATES_NAME = "optim_states"
+    SAVE_TIMEOUT = 600
 
 
 class Accelerators(object):
     NVIDIA_GPU = "nvidia.com/gpu"
     ASCEND_NPU = "ascend-npu"
```

## dlrover/python/common/env_utils.py

```diff
@@ -58,7 +58,13 @@
     return node_type
 
 
 def get_node_num():
     """Get the number of node."""
     node_num = int(os.getenv(NodeEnv.NODE_NUM, 0))
     return node_num
+
+
+def get_env(env_key):
+    """Get the specified environment variable."""
+    env_value = os.getenv(env_key, None)
+    return env_value
```

## dlrover/python/common/grpc.py

```diff
@@ -447,7 +447,22 @@
     optimizer: OptimizerConfig = OptimizerConfig()
     restart: bool = False
 
 
 @dataclass
 class NodeCheckpointState(Message):
     step: int = 0
+
+
+@dataclass
+class DiagnosisTrainingLog(Message):
+    timestamp: int = 0
+
+
+@dataclass
+class DiagnosisCudaLog(Message):
+    timestamp: int = 0
+
+
+@dataclass
+class DiagnosisChipMetrics(Message):
+    timestamp: int = 0
```

## dlrover/python/common/storage.py

```diff
@@ -12,14 +12,15 @@
 # limitations under the License.
 
 import os
 import shutil
 from abc import ABCMeta, abstractmethod
 from typing import Callable, List
 
+from .constants import CheckpointConstant
 from .log import default_logger as logger
 from .serialize import ClassMeta
 
 
 class CheckpointStorage(metaclass=ABCMeta):
     """
     We can implement interfaces of CheckpointStorage to
@@ -217,18 +218,18 @@
         self._checkpoint_dir = checkpoint_dir
 
     def clean_up(self, step, delete_func):
         if step % self._keep_interval == 0:
             return
         rm_dir = os.path.join(self._checkpoint_dir, str(step))
         try:
+            logger.info(f"Clean path {rm_dir}")
             delete_func(rm_dir)
-            print(f"Clean path {rm_dir}")
         except Exception:
-            print(f"Fail to clean path {rm_dir}!")
+            logger.warning(f"Fail to clean path {rm_dir}!")
 
 
 class KeepLatestStepStrategy(CheckpointDeletionStrategy):
     """
     The strategy only remains the latest steps and delete the outdated
     checkpoints.
     Arguments:
@@ -244,39 +245,57 @@
 
     def clean_up(self, step, delete_func):
         self._steps.append(step)
         if len(self._steps) == self._max_to_keep:
             rm_step = self._steps.pop(0)
             rm_dir = os.path.join(self._checkpoint_dir, str(rm_step))
             try:
+                logger.info(f"Clean path {rm_dir}")
                 delete_func(rm_dir)
-                print(f"Clean path {rm_dir}")
             except Exception:
-                print(f"Fail to clean path {rm_dir}!")
+                logger.warning(f"Fail to clean path {rm_dir}!")
 
 
 class PosixStorageWithDeletion(PosixDiskStorage):
     """
     The storage will call a CheckpointDeletionStrategy to
     delete the outdated checkpoints.
 
     Arguments:
-        tracker_file (int): the file name to store the latest checkpoint step.
+        tracker_file (str): the file name to store the latest checkpoint step.
         deletion_strategy (str): the strategy to clean outdated checkpoints.
+
+    Example::
+        from dlrover.python.common.storage import KeepStepIntervalStrategy
+        from dlrover.trainer.torch.flash_checkpoint.ddp import DdpCheckpointer
+
+        # Only keep the checkpoint
+        keep_strategy = KeepStepIntervalStrategy(
+            keep_interval=250,
+            checkpoint_dir="./checkpoint/",
+        )
+        storage = PosixStorageWithDeletion(
+            deletion_strategy=keep_strategy,
+        )
+        checkpointer = DdpCheckpointer(
+            checkpoint_dir="./checkpoint/",
+            storage=storage,
+        )
     """
 
     def __init__(
         self, tracker_file: str, deletion_strategy: CheckpointDeletionStrategy
     ):
         super().__init__()
         self._deletion_strategy = deletion_strategy
         self._tracker_file = tracker_file
         self._pre_step = 0
 
     def write(self, content, path: str):
+        path = str(path)  # The path maybe a PosixPath.
         if path.endswith(self._tracker_file):
             pre_step = self.read(path)
             if pre_step:
                 self._pre_step = int(pre_step)
         super().write(content, path)
 
     def commit(self, step, success):
@@ -292,7 +311,18 @@
         }
         class_mata = ClassMeta(
             module_path=self.__class__.__module__,
             class_name=self.__class__.__name__,
             kwargs=kwargs,
         )
         return class_mata
+
+
+def get_checkpoint_storage(deletion_strategy=None):
+    if deletion_strategy:
+        storage = PosixStorageWithDeletion(
+            tracker_file=CheckpointConstant.TRACER_FILE_NAME,
+            deletion_strategy=deletion_strategy,
+        )
+    else:
+        storage = PosixDiskStorage()
+    return storage
```

## dlrover/python/elastic_agent/master_client.py

```diff
@@ -16,14 +16,15 @@
 import threading
 import time
 from contextlib import closing
 
 from dlrover.proto import elastic_training_pb2, elastic_training_pb2_grpc
 from dlrover.python.common import env_utils, grpc
 from dlrover.python.common.constants import NetworkFailureReason, NodeEnv
+from dlrover.python.common.diagnosis import ChipMetrics, CudaLog, TrainingLog
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.singleton import Singleton
 
 
 def retry_grpc_request(func):
     def wrapper(self, *args, **kwargs):
         retry = kwargs.get("retry", 10)
@@ -371,14 +372,26 @@
     def report_failures(self, error_data, restart_count=-1, level=""):
         message = grpc.NodeFailure(error_data, restart_count, level)
         self._report(message)
 
     def report_paral_config(self, config: grpc.ParallelConfig):
         self._report(config)
 
+    def report_diagnosis_training_log(self, training_log: TrainingLog):
+        message = grpc.DiagnosisTrainingLog(training_log.timestamp)
+        self._report(message)
+
+    def report_diagnosis_chip_metrics(self, chip_metrics: ChipMetrics):
+        message = grpc.DiagnosisChipMetrics(chip_metrics.timestamp)
+        self._report(message)
+
+    def report_diagnosis_cuda_log(self, cuda_log: CudaLog):
+        message = grpc.DiagnosisCudaLog(cuda_log.timestamp)
+        self._report(message)
+
     def get_paral_config(self) -> grpc.ParallelConfig:
         request = grpc.ParallelConfigRequest()
         result = self._get(request)
         return result
 
     def need_to_restart_training(self):
         request = grpc.CheckHardwareResetRequest()
```

## dlrover/python/elastic_agent/torch/ckpt_saver.py

```diff
@@ -363,23 +363,25 @@
 
     def __init__(
         self,
         checkpoint_dir,
         storage_meta: ClassMeta,
         local_shard_num=1,
         global_shard_num=1,
+        save_timeout=CheckpointConstant.SAVE_TIMEOUT,
     ) -> None:
         self.checkpoint_dir = checkpoint_dir
         self.local_shard_num = local_shard_num
         self.global_shard_num = global_shard_num
         self._node_rank = env_utils.get_node_rank()
         self._is_agent_rank_0 = self._node_rank == 0
         self._shm_handlers: List[SharedMemoryHandler] = []
         self._shm_locks: List[SharedLock] = []
         self._stop_commit = False
+        self._save_timeout = save_timeout
 
         module = importlib.import_module(storage_meta.module_path)
         storage_class_def = getattr(module, storage_meta.class_name)
         self.storage = storage_class_def(**storage_meta.kwargs)
 
         # Indicate whether the saver is writing state to storage
         self._writing_storage = False
@@ -506,15 +508,15 @@
         self._event_queue.put(event)
         for i in range(self.local_shard_num):
             if self._shm_handlers[i]:
                 self._shm_handlers[i].close()
                 self._shm_handlers[i].unlink()
             self._shm_locks[i].unlink()
         self._event_queue.unlink()
-        self._executor.shutdown()
+        self._executor.shutdown(wait=False)
 
     def _sync_shm_to_storage(self):
         """
         The loop to persist the state dict from the memory
         buffer into the storage.
         """
         logger.info("Async flash checkpoint saver starts!")
@@ -845,15 +847,17 @@
                 f"step {step}"
             )
             return
 
         # commit checkpoint
         if self._is_agent_rank_0:
             self._stop_commit = False
-            self.commit_checkpoint(step, step_done_dir)
+            self.commit_checkpoint(
+                step, step_done_dir, timeout=self._save_timeout
+            )
 
         self._writing_storage = False
 
     def commit_checkpoint(self, step: int, step_done_dir: str, timeout=600):
         """
         The node rank 0 will update the tracker file with the step
         after the number of done files is equal to the number of shard.
@@ -982,14 +986,15 @@
         # commit checkpoint
         if self._is_agent_rank_0:
             self.commit_checkpoint(
                 step,
                 step_done_dir=step_done_dir,
                 tmp_path=temp_dir,
                 target_path=ckpt_dir,
+                timeout=self._save_timeout,
             )
 
         self._writing_storage = False
 
     def _replace_path_dir(self, ckpt_config: CheckpointConfig, temp_dir: str):
         """
         Replace the directory with the temp directory.
```

## dlrover/python/elastic_agent/torch/training.py

```diff
@@ -16,14 +16,15 @@
 import os
 import shutil
 import signal
 import socket
 import tempfile
 import time
 import uuid
+from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import torch
 import torch.distributed.elastic.timer as timer
 from torch.distributed import PrefixStore, Store
@@ -380,14 +381,17 @@
         self._restart_count = 0
         self._remaining_failovers = self._remaining_restarts
         self._client = MasterClient.singleton_instance()
         if config.auto_tunning:
             self._paral_config_tuner = ParalConfigTuner.singleton_instance()
             self._paral_config_tuner.start()
 
+        self._save_ckpt_executor = ThreadPoolExecutor(max_workers=1)
+        self._save_ckpt_future = None
+
     @prof
     def _rendezvous(self, worker_group: WorkerGroup) -> None:
         r"""
         Runs rendezvous for the workers specified by worker spec.
         Assigns workers a new global rank and world size.
         Updates the rendezvous store for the worker group.
         """
@@ -633,15 +637,17 @@
         """
         The agent can save the checkpointing state dict in the shared
         memory into the storage before restarting training processes.
         """
         saver: AsyncCheckpointSaver = AsyncCheckpointSaver.get_ckpt_saver()
         if saver and self._config.save_at_breakpoint:
             logger.info("Start saving checkpoint at the breakpoint.")
-            saver.save_shm_to_storage(master_client=self._client)
+            self._save_ckpt_future = self._save_ckpt_executor.submit(
+                saver.save_shm_to_storage, 60, self._client
+            )
 
     def _stop_workers_to_restart(self):
         """
         The agent query from the dlrover job master to check whether to restart
         workers. If true, the agent firstly stops all workers.
         """
         restart = self._client.need_to_restart_training()
@@ -687,14 +693,18 @@
                 f"[{role}] Detected {num_nodes_waiting} "
                 f"new nodes from group_rank={group_rank}; "
                 f"will restart worker group"
             )
             return True
         return False
 
+    def stop_executor(self):
+        """Shutdown the executor to save the checkpoint."""
+        self._save_ckpt_executor.shutdown(wait=False)
+
 
 def launch_agent(
     config: ElasticLaunchConfig,
     entrypoint: Union[Callable, str, None],
     args: List[Any],
 ) -> Dict[int, Any]:
     if not config.run_id:
@@ -795,14 +805,15 @@
         raise
     except Exception:
         events.record(agent.get_event_failed())
         raise
     finally:
         if shutdown_rdzv:
             spec.rdzv_handler.shutdown()
+        agent.stop_executor()
         monitor.stop()
 
 
 class NodeCheckElasticAgent(ElasticTrainingAgent):
     """
     An implementation of :py:class:`torchelastic.agent.server.ElasticAgent`
     that handles host-local workers. This agent will run 2 rounds allgather
```

## dlrover/python/master/servicer.py

```diff
@@ -18,21 +18,30 @@
 
 import grpc as grpc_lib
 
 from dlrover.proto import elastic_training_pb2, elastic_training_pb2_grpc
 from dlrover.python.common import grpc
 from dlrover.python.common.constants import (
     GRPC,
+    CustomMetricKeys,
     NodeStatus,
     NodeType,
     RendezvousName,
+    TrainingExceptionLevel,
     TrainingLoopStatus,
 )
+from dlrover.python.common.diagnosis import (
+    ChipMetrics,
+    CudaLog,
+    DiagnosisDataType,
+    TrainingLog,
+)
 from dlrover.python.common.global_context import Context
 from dlrover.python.common.log import default_logger as logger
+from dlrover.python.master.diagnosis.diagnosis import DiagnosisManager
 from dlrover.python.master.elastic_training.kv_store_service import (
     KVStoreService,
 )
 from dlrover.python.master.elastic_training.rdzv_manager import (
     NetworkCheckRendezvousManager,
     RendezvousManager,
 )
@@ -72,14 +81,15 @@
         elastic_ps_service=None,
         sync_service=None,
     ):
         self._task_manager: TaskManager = task_manager
         self._job_manager: JobManager = job_manager
         self._speed_monitor = speed_monitor
         self._rdzv_managers = rdzv_managers
+        self._diagnosis_manager: DiagnosisManager = DiagnosisManager()
         self._kv_store = KVStoreService()
         self._job_metric_collector: JobMetricCollector = job_metric_collector
         self._elastic_ps_service: ElasticPsService = elastic_ps_service
         self._sync_service: SyncService = sync_service
         self._lock = threading.Lock()
         self._version = 0
         self._start_training_time = 0
@@ -255,14 +265,18 @@
         rdzv_manager = self._rdzv_managers[request.rdzv_name]
         rdzv_round, group, nodes = rdzv_manager.get_comm_world(request.node_id)
         res = grpc.RendezvousState(world={})
         res.group = group
         res.round = rdzv_round
         for rank_id, meta in nodes.items():
             res.world[rank_id] = meta.process_num
+        if nodes and request.rdzv_name == RendezvousName.ELASTIC_TRAINING:
+            rdzv_round = rdzv_manager.get_rdzv_round()
+            metrics = {CustomMetricKeys.RDZV_ROUND: rdzv_round}
+            self._job_metric_collector.collect_custom_data(metrics)
         return res
 
     def _kv_store_get(self, request: grpc.KeyValuePair):
         value = self._kv_store.get(request.key)
         res = grpc.KeyValuePair(request.key, value)
         return res
 
@@ -328,14 +342,20 @@
             success = self._kv_store_set(message)
         elif isinstance(message, grpc.ParallelConfig):
             success = self._report_paral_config(node_type, node_id, message)
         elif isinstance(message, grpc.HeartBeat):
             success = self._report_heartbeat(node_type, node_id, message)
         elif isinstance(message, grpc.NodeCheckpointState):
             success = self._sync_checkpoint(node_type, node_id, message)
+        elif isinstance(message, grpc.DiagnosisChipMetrics):
+            success = self._report_chip_metrics(node_type, node_id, message)
+        elif isinstance(message, grpc.DiagnosisCudaLog):
+            success = self._report_cuda_log(node_type, node_id, message)
+        elif isinstance(message, grpc.DiagnosisTrainingLog):
+            success = self._report_training_log(node_type, node_id, message)
 
         response.success = success
         return response
 
     def _ready_for_ps_relaunch(self):
         self._job_manager.post_ps_ready()
         return True
@@ -533,14 +553,19 @@
         self._job_manager.handle_training_failure(
             node_type,
             node_id,
             message.restart_count,
             message.error_data,
             message.level,
         )
+        if message.level == TrainingExceptionLevel.RDZV_ERROR:
+            custom_data = {
+                CustomMetricKeys.TRAINING_ERROR_LEVEL: message.level
+            }
+            self._job_metric_collector.collect_custom_data(custom_data)
         return True
 
     def _kv_store_set(self, message: grpc.KeyValuePair):
         self._kv_store.set(message.key, message.value)
         return True
 
     def _report_paral_config(
@@ -570,14 +595,41 @@
         self, node_type, node_id, message: grpc.NodeCheckpointState
     ):
         if RendezvousName.ELASTIC_TRAINING not in self._rdzv_managers:
             return False
         rdzv_manager = self._rdzv_managers[RendezvousName.ELASTIC_TRAINING]
         return rdzv_manager.sync_ckpt_nodes(node_id, message.step)
 
+    def _report_chip_metrics(
+        self, node_type, node_id, message: grpc.DiagnosisChipMetrics
+    ):
+        data = ChipMetrics(message.timestamp)
+        self._diagnosis_manager.collect_diagnosis_data(
+            DiagnosisDataType.CHIPMETRICES, data
+        )
+        return True
+
+    def _report_training_log(
+        self, node_type, node_id, message: grpc.DiagnosisTrainingLog
+    ):
+        data = TrainingLog(message.timestamp)
+        self._diagnosis_manager.collect_diagnosis_data(
+            DiagnosisDataType.TRAININGLOG, data
+        )
+        return True
+
+    def _report_cuda_log(
+        self, node_type, node_id, message: grpc.DiagnosisCudaLog
+    ):
+        data = CudaLog(message.timestamp)
+        self._diagnosis_manager.collect_diagnosis_data(
+            DiagnosisDataType.CUDALOG, data
+        )
+        return True
+
 
 def create_master_service(
     port,
     task_manager,
     job_manager,
     speed_monitor,
     rdzv_managers,
```

## dlrover/python/master/node/event_callback.py

```diff
@@ -262,14 +262,15 @@
             if completed:
                 self._master.request_stop(
                     success=True,
                     reason=JobExitReason.SUCCEEDED,
                     msg="All critical nodes completed",
                 )
         self._speed_monitor.remove_running_worker(node.type, node.id)
+        self._remove_node_from_rdzv(node)
 
     @NodeEventCallback.log_callback_exception
     def on_node_failed(self, node: Node, cluster_context):
         node.finish_time = datetime.now()  # type: ignore
         self._failed_worker_count += 1
         self._stop_job_if_needed(node)
         if node.is_unrecoverable_failure():
@@ -279,21 +280,23 @@
         if node.exit_reason == NodeExitReason.HARDWARE_ERROR:
             self._master.job_manager.handle_training_failure(
                 node.type,
                 node.id,
                 error_data=NodeExitReason.HARDWARE_ERROR,
                 level=TrainingExceptionLevel.NODE_ERROR,
             )
-        for manager in self._rdzv_managers.values():
-            manager.remove_alive_node(node)
+        self._remove_node_from_rdzv(node)
 
     @NodeEventCallback.log_callback_exception
     def on_node_deleted(self, node, cluster_context):
         node.finish_time = datetime.now()  # type: ignore
         self._stop_job_if_needed(node)
+        self._remove_node_from_rdzv(node)
+
+    def _remove_node_from_rdzv(self, node):
         for manager in self._rdzv_managers.values():
             manager.remove_alive_node(node)
 
     def _stop_job_if_needed(self, node: Node):
         stop_node = False
         if node.exit_reason == NodeExitReason.FATAL_ERROR:
             if not _dlrover_ctx.relaunch_always:
```

## dlrover/python/master/scaler/pod_scaler.py

```diff
@@ -40,14 +40,15 @@
     convert_memory_to_mb,
     get_main_container,
     get_pod_name,
     k8sClient,
     k8sServiceFactory,
     set_container_resource,
 )
+from dlrover.python.util import k8s_util
 
 _dlrover_context = Context.singleton_instance()
 
 
 class FakeKubeResponse:
     def __init__(self, obj):
         self.data = json.dumps(obj)
@@ -157,23 +158,53 @@
             )
             if job:
                 return job
             else:
                 time.sleep(5)
         return None
 
+    def _get_master_pod_labels(self):
+        return {
+            ElasticJobLabel.JOB_KEY: self._job_name,
+            ElasticJobLabel.REPLICA_TYPE_KEY: NodeType.DLROVER_MASTER,
+        }
+
     def _retry_to_get_master_pod(self):
-        master_name = f"elasticjob-{self._job_name}-dlrover-master"
+        """
+        Get master pod by labels.
+        Notice: Labels might be different in different environments for now.
+        """
+        master_labels_selector = k8s_util.gen_k8s_label_selector_from_dict(
+            self._get_master_pod_labels()
+        )
+        logger.info(f"Get master pod by labels : {master_labels_selector}.")
         for _ in range(3):
-            pod = self._k8s_client.get_pod(master_name)
-            if pod:
-                return pod
-            else:
-                time.sleep(5)
-        raise ValueError(f"{master_name} is not Found!")
+            pods = self._k8s_client.list_namespaced_pod(master_labels_selector)
+            if pods and len(pods.items) > 0:
+                if (
+                    len(pods.items) == 1
+                    and pods.items[0].status.phase == NodeStatus.RUNNING
+                ):
+                    # return the only running master
+                    return pods.items[0]
+                elif len(pods.items) > 1:
+                    # return the last running master
+                    pods.items.sort(
+                        key=lambda pod: (
+                            pod.metadata.creation_timestamp is None,
+                            pod.metadata.creation_timestamp,
+                        ),
+                        reverse=True,
+                    )
+                    for pod in pods.items:
+                        if pod.status.phase == NodeStatus.RUNNING:
+                            return pod
+        raise ValueError(
+            f"Master pod is not found by labels: {master_labels_selector}"
+        )
 
     def scale(self, plan: ScalePlan):
         """Scale in/out Pods by a ScalePlan."""
 
         if not self._elasticjob_exists():
             plan_json = plan.to_json()
             logger.info(
```

## dlrover/python/master/stats/job_collector.py

```diff
@@ -68,14 +68,22 @@
 
     @abstractmethod
     def collect_runtime_stats(
         self, speed_monitor: SpeedMonitor, running_nodes: List[Node]
     ):
         pass
 
+    @abstractmethod
+    def collect_custom_data(self, metric_dict):
+        pass
+
+    @abstractmethod
+    def collect_job_exit_reason(self, reason):
+        pass
+
 
 class JobMetricCollector(BaseMetricCollector):
     """The collector receives model parameters message from workers
     and processes the message. Then, it will report model parameters
     to EasyDL server.
     """
 
@@ -121,15 +129,20 @@
         self._stats_reporter.report_model_info(model_info)
 
     @BaseMetricCollector.catch_exception
     def _report_runtime_stats(self):
         self._stats_reporter.report_runtime_stats(self._runtime_metric)
 
     @BaseMetricCollector.catch_exception
-    def collect_custom_data(self):
+    def collect_custom_data(self, metric_dict=None):
+        if (
+            metric_dict
+            and not metric_dict.items() <= self._custom_metric.items()
+        ):
+            self._custom_metric.update(metric_dict)
         self._stats_reporter.report_customized_data(self._custom_metric)
 
     def collect_runtime_stats(
         self, speed_monitor: SpeedMonitor, running_nodes: List[Node]
     ):
         """Set runtime info by global step"""
         if (
@@ -138,23 +151,18 @@
         ):
             return
         self._runtime_metric.clear()
         self._runtime_metric.global_step = speed_monitor.completed_global_step
         self._runtime_metric.timestamp = int(time.time())
         self._runtime_metric.speed = speed_monitor.running_speed
 
-        if (
-            speed_monitor.init_training_time > 0
-            and self._custom_metric.get(CustomMetricKey.INIT_TRAINING_TIME, 0)
-            == 0
-        ):
-            self._custom_metric[
-                CustomMetricKey.INIT_TRAINING_TIME
-            ] = speed_monitor.init_training_time
-            self.collect_custom_data()
+        if speed_monitor.init_training_time > 0:
+            init_time_key = CustomMetricKey.INIT_TRAINING_TIME
+            metric = {init_time_key: speed_monitor.init_training_time}
+            self.collect_custom_data(metric)
         for node in running_nodes:
             node_sample = copy.deepcopy(node)
             node_sample.used_resource.memory *= MemoryUnit.MB
             if (node.type, node.id) in speed_monitor.running_workers:
                 self._runtime_metric.running_nodes.append(node_sample)
             else:
                 self._runtime_metric.running_nodes.append(node_sample)
```

## dlrover/python/tests/test_agent_monitor.py

```diff
@@ -15,18 +15,22 @@
 import os
 import time
 import unittest
 from unittest.mock import patch
 
 from dlrover.python.common.constants import NodeEnv
 from dlrover.python.common.grpc import GPUStats
+from dlrover.python.elastic_agent.datacollector.data_collector import (
+    CollectorType,
+)
 from dlrover.python.elastic_agent.master_client import (
     MasterClient,
     build_master_client,
 )
+from dlrover.python.elastic_agent.monitor.diagnosis import DiagnosisMonitor
 from dlrover.python.elastic_agent.monitor.resource import ResourceMonitor
 from dlrover.python.elastic_agent.monitor.training import (
     TFTrainingReporter,
     is_tf_chief,
 )
 from dlrover.python.tests.test_utils import start_local_master
 
@@ -86,10 +90,28 @@
         reporter1 = TFTrainingReporter.singleton_instance()
         self.assertEqual(reporter0, reporter1)
         reporter0.set_start_time()
         self.assertTrue(reporter0._start_time > 0)
         reporter0._last_timestamp = time.time() - 30
         reporter0.report_resource_with_step(100)
 
+    def test_diagnosis_monitor(self):
+        monitor = DiagnosisMonitor.singleton_instance()
+        monitor.start()
+        collectors = monitor.get_collectors()
+        self.assertEqual(len(collectors), 3)
+
+        cuda_event = monitor.collect_data(CollectorType.CUDALOG)
+        self.assertFalse(not cuda_event)
+        monitor.report_diagnosis_data(cuda_event)
+
+        logs = monitor.collect_data(CollectorType.TRAININGLOG)
+        self.assertFalse(not logs)
+        monitor.report_diagnosis_data(logs)
+
+        metrics = monitor.collect_data(CollectorType.CHIPMETRICS)
+        self.assertFalse(not metrics)
+        monitor.report_diagnosis_data(metrics)
+
 
 if __name__ == "__main__":
     unittest.main()
```

## dlrover/python/tests/test_elastic_training_agent.py

```diff
@@ -301,14 +301,15 @@
         )
         storage = PosixDiskStorage()
         saver = DdpCheckpointSaver("/tmp/test", storage.get_class_meta())
         AsyncCheckpointSaver._saver_instance = saver
         agent._save_ckpt_to_storage()
         agent._stop_workers_to_restart()
         agent._wait_async_saver()
+        agent.stop_executor()
 
 
 class NodeCheckElasticAgentTest(unittest.TestCase):
     def setUp(self) -> None:
         self._master, addr = start_local_master()
         MasterClient._instance = build_master_client(addr, 0.5)
         launch_config = LaunchConfig(
```

## dlrover/python/tests/test_pod_scaler.py

```diff
@@ -10,15 +10,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import unittest
 
-from dlrover.python.common.constants import DistributionStrategy, NodeType
+from dlrover.python.common.constants import (
+    DistributionStrategy,
+    ElasticJobLabel,
+    NodeType,
+)
 from dlrover.python.common.global_context import Context
 from dlrover.python.common.node import Node, NodeGroupResource, NodeResource
 from dlrover.python.master.scaler.base_scaler import ScalePlan
 from dlrover.python.master.scaler.pod_scaler import PodScaler, new_tf_config
 from dlrover.python.tests.test_utils import mock_k8s_client
 
 _dlrover_ctx = Context.singleton_instance()
@@ -236,7 +240,24 @@
         cur_nodes = [Node(NodeType.WORKER, 1, rank_index=0)]
         scaler._scale_up_pods(NodeType.WORKER, scale_plan, cur_nodes, 1)
         self.assertEqual(len(scaler._create_node_queue), 4)
         self.assertEqual(
             scaler._create_node_queue[0].service_addr,
             "elasticjob-sample-edljob-worker-1.default.svc:3333",
         )
+
+    def test_get_master_pod(self):
+        scaler = PodScaler("elasticjob-sample", "default")
+        scaler.start()
+
+        for _ in range(10):
+            master_pod = scaler._retry_to_get_master_pod()
+            self.assertIsNotNone(master_pod)
+            self.assertEqual(
+                "1",
+                master_pod.metadata.labels.get(
+                    ElasticJobLabel.REPLICA_INDEX_KEY
+                ),
+            )
+            self.assertTrue(
+                ElasticJobLabel.REPLICA_TYPE_KEY in master_pod.metadata.labels
+            )
```

## dlrover/python/tests/test_stats_collector.py

```diff
@@ -60,20 +60,25 @@
         self.assertEqual(len(reporter._runtime_stats), 8)
 
 
 class StatsCollectorTest(unittest.TestCase):
     def test_job_metric_collector(self):
         collector = JobMetricCollector("1111", "default", "local", "dlrover")
         collector.collect_dataset_metric("test", 1000)
+        custom_metric = {"key0": 100}
+        collector.collect_custom_data(custom_metric)
+        self.assertDictEqual(custom_metric, collector._custom_metric)
 
         speed_monitor = SpeedMonitor()
         t = int(time.time())
         speed_monitor.set_target_worker_num(1)
         speed_monitor.collect_global_step(100, t)
         speed_monitor.collect_global_step(1100, t + 10)
         speed_monitor.add_running_worker(NodeType.WORKER, 0)
         worker = Node(NodeType.WORKER, 0, None)
         collector._stats_reporter._runtime_stats = []
+        speed_monitor._start_training_time = 100
+        speed_monitor._init_time = 10
         collector.collect_runtime_stats(speed_monitor, [worker])
         self.assertEqual(len(collector._runtime_metric.running_nodes), 1)
         self.assertEqual(collector._runtime_metric.speed, 100)
         self.assertEqual(len(collector._stats_reporter._runtime_stats), 1)
```

## dlrover/python/tests/test_storage.py

```diff
@@ -15,15 +15,16 @@
 import shutil
 import tempfile
 import unittest
 
 from dlrover.python.common.storage import (
     KeepLatestStepStrategy,
     KeepStepIntervalStrategy,
-    PosixStorageWithDeletion,
+    PosixDiskStorage,
+    get_checkpoint_storage,
 )
 
 
 class TestLocalStrategyGenerator(unittest.TestCase):
     def test_keep_latest_deletion_strategy(self):
         with tempfile.TemporaryDirectory() as tmpdir:
             deletion_strategy = KeepLatestStepStrategy(3, tmpdir)
@@ -40,28 +41,49 @@
             for i in range(2, 6):
                 step = i * 2
                 os.makedirs(os.path.join(tmpdir, str(step)))
                 deletion_strategy.clean_up(step - 2, shutil.rmtree)
             self.assertListEqual(sorted(os.listdir(tmpdir)), ["10", "4", "8"])
 
     def test_posix_storage_with_deletion(self):
+        tracker_file = "dlrover_latest.txt"
+
         with tempfile.TemporaryDirectory() as tmpdir:
-            deletion_strategy = KeepLatestStepStrategy(3, tmpdir)
-            tracker_file = "dlrover_latest.txt"
             tracker_file_path = os.path.join(tmpdir, tracker_file)
-            storage = PosixStorageWithDeletion(tracker_file, deletion_strategy)
+            strategy = KeepLatestStepStrategy(
+                max_to_keep=3, checkpoint_dir=tmpdir
+            )
+            storage = get_checkpoint_storage(strategy)
 
             for step in range(1, 5):
                 storage.write(str(step), tracker_file_path)
                 os.makedirs(os.path.join(tmpdir, str(step)))
                 storage.commit(step, True)
 
             files = os.listdir(tmpdir)
             files.remove(tracker_file)
             self.assertListEqual(sorted(files), ["2", "3", "4"])
 
             class_meta = storage.get_class_meta()
             self.assertEqual(class_meta.class_name, "PosixStorageWithDeletion")
 
+        with tempfile.TemporaryDirectory() as tmpdir:
+            tracker_file_path = os.path.join(tmpdir, tracker_file)
+            strategy = KeepStepIntervalStrategy(
+                keep_interval=4, checkpoint_dir=tmpdir
+            )
+            storage = get_checkpoint_storage(strategy)
+            for step in range(1, 9):
+                storage.write(str(step), tracker_file_path)
+                os.makedirs(os.path.join(tmpdir, str(step)))
+                storage.commit(step, True)
+
+            files = os.listdir(tmpdir)
+            files.remove(tracker_file)
+            self.assertListEqual(sorted(files), ["4", "8"])
+
+            storage = get_checkpoint_storage(None)
+            self.assertTrue(isinstance(storage, PosixDiskStorage))
+
 
 if __name__ == "__main__":
     unittest.main()
```

## dlrover/python/tests/test_utils.py

```diff
@@ -13,14 +13,15 @@
 
 import datetime
 from unittest import mock
 
 import yaml
 from kubernetes import client
 
+import dlrover.python.util.k8s_util as ku
 from dlrover.proto import elastic_training_pb2
 from dlrover.python.common.constants import (
     DistributionStrategy,
     ElasticJobLabel,
     NodeStatus,
     NodeType,
     PlatformType,
@@ -179,44 +180,60 @@
     pod = client.V1Pod(
         api_version="v1",
         kind="Pod",
         spec=spec,
         metadata=client.V1ObjectMeta(
             name="test-worker-0",
             labels=labels,
+            creation_timestamp=datetime.datetime.now(),
             annotations={},
         ),
         status=status,
     )
     return pod
 
 
 def mock_list_namespaced_pod(label_selector):
     pods = []
-    for i in range(2):
-        labels = {
-            ElasticJobLabel.APP_NAME: "test",
-            ElasticJobLabel.REPLICA_TYPE_KEY: NodeType.PS,
-            ElasticJobLabel.REPLICA_INDEX_KEY: str(i),
-            ElasticJobLabel.RANK_INDEX_KEY: str(i),
-            ElasticJobLabel.RELAUNCH_COUNT: "0",
-        }
-        pod = create_pod(labels)
-        pods.append(pod)
-
-    for i in range(3):
-        labels = {
-            ElasticJobLabel.APP_NAME: "test",
-            ElasticJobLabel.REPLICA_TYPE_KEY: NodeType.WORKER,
-            ElasticJobLabel.REPLICA_INDEX_KEY: str(i),
-            ElasticJobLabel.RANK_INDEX_KEY: str(i),
-            ElasticJobLabel.RELAUNCH_COUNT: "0",
-        }
-        pod = create_pod(labels)
-        pods.append(pod)
+    if "master" in label_selector:
+        job_name = ku.gen_dict_from_k8s_label_selector(label_selector).get(
+            ElasticJobLabel.JOB_KEY
+        )
+        for i in range(2):
+            labels = {
+                ElasticJobLabel.APP_NAME: "test",
+                ElasticJobLabel.JOB_KEY: job_name,
+                ElasticJobLabel.REPLICA_TYPE_KEY: NodeType.DLROVER_MASTER,
+                ElasticJobLabel.REPLICA_INDEX_KEY: str(i),
+            }
+            pod = create_pod(labels)
+            pods.append(pod)
+    else:
+        for i in range(2):
+            labels = {
+                ElasticJobLabel.APP_NAME: "test",
+                ElasticJobLabel.REPLICA_TYPE_KEY: NodeType.PS,
+                ElasticJobLabel.REPLICA_INDEX_KEY: str(i),
+                ElasticJobLabel.RANK_INDEX_KEY: str(i),
+                ElasticJobLabel.RELAUNCH_COUNT: "0",
+            }
+            pod = create_pod(labels)
+            pods.append(pod)
+
+        for i in range(3):
+            labels = {
+                ElasticJobLabel.APP_NAME: "test",
+                ElasticJobLabel.REPLICA_TYPE_KEY: NodeType.WORKER,
+                ElasticJobLabel.REPLICA_INDEX_KEY: str(i),
+                ElasticJobLabel.RANK_INDEX_KEY: str(i),
+                ElasticJobLabel.RELAUNCH_COUNT: "0",
+            }
+            pod = create_pod(labels)
+            pods.append(pod)
+
     return client.V1PodList(
         items=pods, metadata=client.V1ListMeta(resource_version="12345678")
     )
 
 
 def create_test_dataset_splitter(dataset_name="test"):
     splitter = new_dataset_splitter(
```

## dlrover/trainer/torch/elastic_run.py

```diff
@@ -296,14 +296,18 @@
         args, "exclude_straggler", False
     )
     elastic_config.set_node_unit(getattr(args, "node_unit", 1))
     elastic_config.save_at_breakpoint = getattr(
         args, "save_at_breakpoint", False
     )
     elastic_config.auto_configure_params()
+    elastic_config.rdzv_backend = "dlrover-master"
+    elastic_config.rdzv_endpoint = ""
+    join_timeout = elastic_config.rdzv_configs.get("join_timeout", 600)
+    elastic_config.rdzv_configs["timeout"] = join_timeout
     return elastic_config, cmd, cmd_args
 
 
 def _check_to_use_dlrover_run(master_addr, max_nodes, timeout=120):
     if _check_dlrover_master_available(master_addr, timeout):
         return True
     elif max_nodes == 1:
```

## dlrover/trainer/torch/flash_checkpoint/ddp.py

```diff
@@ -12,38 +12,45 @@
 # limitations under the License.
 
 import os
 
 import torch.distributed as dist
 
 from dlrover.python.common.constants import CheckpointConstant
-from dlrover.python.common.storage import PosixDiskStorage
+from dlrover.python.common.storage import get_checkpoint_storage
 
 from .checkpointer import Checkpointer, StorageType
 from .full_ckpt_engine import FullCheckpointEngine
 
 
 class DdpCheckpointer(Checkpointer):
     """
     Flash checkpointer to save and load a DDP model or a model state
     dict with full weights.
 
     Args:
         checkpoint_dir: the directory to save the checkpoint.
-        storage: A CheckpointStorage instance. The checkpointer will
-            use a PosixStorage instance if the storage is not defined.
         local_shard_num (int): the number of shards on a node,
             The default is 1. If the model is partitioned on all ranks,
             you should set the local_shard_num as the number of ranks
             on a node.
         global_shard_num (int): the number of shards across all ranks.
             The default is 1.If the model is partitioned on all ranks,
             you should set the local_shard_num as the number of all ranks.
         comm_backend (str): the communcation backend to create a process group,
             The default is the backend of general main process group.
+        deletion_strategy: A `CheckpointDeletionStrategy` instance. The default
+            value is None and all checkpoint files will be retained. Now, the
+            strategy can be `KeepLatestStepStrategy`
+            or `KeepStepIntervalStrategy`. Users also can define a strategy
+            to manage the checkpoint files.
+        save_timeout (int): the seconds for node rank 0 to wait all
+            ranks save checkpoints. The node rank 0 will skip the checkpoint
+            if some ranks do not finish saving checkpoint in the save_timeout
+            after the node rank 0 finishes saving checkpoint.
 
     Examples::
         >>> checkpointer = DdpCheckpointer(
         >>>     checkpoint_dir="/tmp/checkpoint/"
         >>> )
         >>> for step, data in enumerate(dataloader):
         >>>     ...
@@ -59,31 +66,33 @@
         >>>         )
         >>> sate_dict = checkpointer.load_checkpoint()
     """
 
     def __init__(
         self,
         checkpoint_dir: str,
-        storage=None,
         local_shard_num=1,
         global_shard_num=1,
         comm_backend="",
+        deletion_strategy=None,
+        save_timeout=CheckpointConstant.SAVE_TIMEOUT,
     ):
         self.checkpoint_dir = checkpoint_dir
         if dist.is_initialized():
             self._rank = dist.get_rank()
         else:
             self._rank = 0
-        self.storage = PosixDiskStorage() if not storage else storage
+        self.storage = get_checkpoint_storage(deletion_strategy)
         self._engine = FullCheckpointEngine(
             checkpoint_dir=checkpoint_dir,
             storage=self.storage,
             local_shard_num=local_shard_num,
             global_shard_num=global_shard_num,
             comm_backend=comm_backend,
+            save_timeout=save_timeout,
         )
 
     def save_checkpoint(
         self, step, state_dict, path="", storage_type=StorageType.DISK
     ):
         if path == "":
             ckpt_name = f"{step}/rank_{self._rank}.pt"
```

## dlrover/trainer/torch/flash_checkpoint/deepspeed.py

```diff
@@ -20,15 +20,18 @@
     CheckpointEngine,
 )
 from deepspeed.runtime.engine import DeepSpeedEngine
 from deepspeed.runtime.zero.config import ZeroStageEnum
 
 from dlrover.python.common import env_utils
 from dlrover.python.common.constants import CheckpointConstant
-from dlrover.python.common.storage import CheckpointStorage, PosixDiskStorage
+from dlrover.python.common.storage import (
+    CheckpointStorage,
+    get_checkpoint_storage,
+)
 from dlrover.python.elastic_agent.torch.ckpt_saver import (
     DeepSpeedCheckpointSaver,
 )
 
 from .checkpointer import Checkpointer, StorageType
 from .deepspeed_engine import DeepSpeedCheckpointEngine
 
@@ -94,18 +97,25 @@
 
 class DeepSpeedCheckpointer(Checkpointer):
     """
     Flash checkpointer saves and loads a DeepSpeedEngine module.
 
     Args:
         checkpoint_dir: the directory to save the checkpoint.
-        storage: A CheckpointStorage instance. The checkpointer will
-            use a PosixStorage instance if the storage is not defined.
         comm_backend (str): the backend to synchronize when saving the
             checkpoint to the memory.
+        deletion_strategy: A `CheckpointDeletionStrategy` instance. The default
+            value is None and all checkpoint files will be retained. Now, the
+            strategy can be `KeepLatestStepStrategy`
+            or `KeepStepIntervalStrategy`. Users also can define a strategy
+            to manage the checkpoint files.
+        save_timeout (int): the seconds for node rank 0 to wait all
+            ranks save checkpoints. The node rank 0 will skip the checkpoint
+            if some ranks do not finish saving checkpoint in the save_timeout
+            after the node rank 0 finishes saving checkpoint.
 
     Examples::
         >>> engine = deepspeed.initialize(...)
         >>> checkpointer = DeepSpeedCheckpointer(engine, save_dir)
         >>> if step % 10 == 0:
         >>>     checkpointer.save_checkpoint(
         >>>         save_dir, tag, storage_type=StorageType.MEMORY
@@ -116,32 +126,34 @@
         >>>     )
     """
 
     def __init__(
         self,
         engine: DeepSpeedEngine,
         checkpoint_dir,
-        storage=None,
         comm_backend="",
+        deletion_strategy=None,
+        save_timeout=CheckpointConstant.SAVE_TIMEOUT,
     ):
         self.engine = engine
         self.checkpoint_dir = checkpoint_dir
         global_shard_num = 1
         if self.engine.zero_optimization():
             global_shard_num = dist.get_world_size(
                 self.engine.optimizer.dp_process_group
             )
         zero_stage = self.engine.zero_optimization_stage()
-        self.storage = PosixDiskStorage() if not storage else storage
+        self.storage = get_checkpoint_storage(deletion_strategy)
         self._async_save_engine = DeepSpeedCheckpointEngine(
             checkpoint_dir,
             storage=self.storage,
             global_shard_num=global_shard_num,
             zero_stage=zero_stage,
             comm_backend=comm_backend,
+            save_timeout=save_timeout,
         )
         self._ckpt_agent = AsyncCheckpointAgent(
             self._async_save_engine.storage
         )
         self._local_rank = env_utils.get_local_rank()
         self._ds_tracer_file = os.path.join(
             self.checkpoint_dir, DeepSpeedCheckpointSaver.TRACER_FILE
```

## dlrover/trainer/torch/flash_checkpoint/deepspeed_engine.py

```diff
@@ -48,18 +48,19 @@
     def __init__(
         self,
         checkpoint_dir,
         storage,
         global_shard_num=1,
         zero_stage=0,
         comm_backend="",
+        save_timeout=CheckpointConstant.SAVE_TIMEOUT,
     ):
         self.global_shard_num = global_shard_num
         self.zero_stage = zero_stage
-        super().__init__(checkpoint_dir, storage, comm_backend)
+        super().__init__(checkpoint_dir, storage, comm_backend, save_timeout)
 
     def get_saving_ranks(self):
         """
         Get the ranks which need to save the sharding state dict into
         the memory.
         """
         world_size = dist.get_world_size()
@@ -85,20 +86,15 @@
             step (int): the global iteration step.
             state_dict (dict): the state dict of model and optimizer to save.
             paths (dict): the key is a category in
                 ["model_states", "optim_states"] of the state dict and
                 the value is the path of storage to save.
         """
         conf = CheckpointConfig(step=step, paths=paths)
-        import time
-
-        start = time.time()
         success = self.save_state_dict_to_memory(state_dict, conf)
-        t = round(time.time() - start, 2)
-        print(f"Save Time is {t}s")
         return success
 
     @timer
     def save_to_storage(self, step, state_dict, paths):
         """
         Asynchonously saves the state dict into the storage. It synchonously
         saves the state dict into the shared memory and put the path
```

## dlrover/trainer/torch/flash_checkpoint/engine.py

```diff
@@ -18,14 +18,15 @@
 from multiprocessing import Process
 from typing import Dict, List, Optional
 
 import torch
 import torch.distributed as dist
 
 from dlrover.python.common import env_utils
+from dlrover.python.common.constants import CheckpointConstant
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.multi_process import SharedLock, SharedQueue
 from dlrover.python.common.singleton import Singleton
 from dlrover.python.common.storage import CheckpointStorage
 from dlrover.python.elastic_agent.torch.ckpt_saver import (
     DLROVER_CKPT_CONFIG_KEY,
     AsyncCheckpointSaver,
@@ -154,20 +155,22 @@
     saver_proc = None
 
     def __init__(
         self,
         checkpoint_dir: str,
         storage: CheckpointStorage,
         comm_backend: str = "",
+        save_timeout: int = CheckpointConstant.SAVE_TIMEOUT,
     ):
         if not self.saver_proc:
             self.saver_proc = start_saver_process()
 
         self.checkpoint_dir = checkpoint_dir
         self.storage = storage
+        self._save_timeout = save_timeout
         self._local_rank = int(os.getenv("LOCAL_RANK", 0))
         self._cached_step = 0
         self._restart_count = env_utils.get_torch_restart_count()
         # queue for agent to save to storage, only lock rank 0 needs the queue.
         if self._local_rank == 0:
             self._event_queue = SharedQueue(
                 name=CheckpointSharedObjPrefix.SAVE_STEP_QNAME + str(0),
@@ -261,14 +264,15 @@
             module_path=clazz.__module__,
             class_name=clazz.__name__,
             kwargs={
                 "checkpoint_dir": self.checkpoint_dir,
                 "storage_meta": self.storage.get_class_meta(),
                 "local_shard_num": local_shard_num,
                 "global_shard_num": global_shard_num,
+                "save_timeout": self._save_timeout,
             },
         )
 
         queue.put(class_meta)
 
     def _update_saver_config(self):
         """Update the sharding configuration to the saver."""
```

## dlrover/trainer/torch/flash_checkpoint/fsdp.py

```diff
@@ -20,51 +20,60 @@
 )
 from torch.distributed.fsdp import FullStateDictConfig
 from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
 from torch.distributed.fsdp import StateDictType
 from torch.distributed.fsdp.api import FullOptimStateDictConfig
 
 from dlrover.python.common.constants import CheckpointConstant
-from dlrover.python.common.storage import PosixDiskStorage
+from dlrover.python.common.storage import get_checkpoint_storage
 from dlrover.trainer.torch.flash_checkpoint.full_ckpt_engine import (
     FullCheckpointEngine,
 )
 
 from .checkpointer import Checkpointer, StorageType
 from .fsdp_engine import FsdpCheckpointEngine
 
 
 class FsdpShardCheckpointer(Checkpointer):
     """
     Flash checkpointer saves and loads a FSDP module.
 
     Args:
         checkpoint_dir: the directory to save the checkpoint.
-        storage: A CheckpointStorage instance. The checkpointer will
-            use a PosixStorage instance if the storage is not defined.
         comm_backend (str): the backend to synchronize when saving the
             checkpoint to the memory.
+        deletion_strategy: A `CheckpointDeletionStrategy` instance. The default
+            value is None and all checkpoint files will be retained. Now, the
+            strategy can be `KeepLatestStepStrategy`
+            or `KeepStepIntervalStrategy`. Users also can define a strategy
+            to manage the checkpoint files.
 
     Examples::
         >>> checkpointer = FsdpShardCheckpointer(checkpoint_dir)
         >>> # Save checkpoint
         >>> extra_sd = {"step": step, "epoch": epoch}
         >>> if step % save_storage_interval == 0:
         >>>     checkpointer.save_checkpoint(
         >>>         step, state_dict, ckpt_dir
         >>>     )
         >>> # Load checkpoint
         >>> checkpointer.load_checkpoint(model, optimzier)
     """
 
-    def __init__(self, checkpoint_dir: str, storage=None, comm_backend=""):
+    def __init__(
+        self,
+        checkpoint_dir: str,
+        comm_backend="",
+        deletion_strategy=None,
+        save_timeout=CheckpointConstant.SAVE_TIMEOUT,
+    ):
         self.checkpoint_dir = checkpoint_dir
-        self.storage = PosixDiskStorage() if not storage else storage
+        self.storage = get_checkpoint_storage(deletion_strategy)
         self._engine = FsdpCheckpointEngine(
-            checkpoint_dir, self.storage, comm_backend
+            checkpoint_dir, self.storage, comm_backend, save_timeout
         )
 
     def save_checkpoint(
         self,
         step,
         model,
         optimizer,
@@ -142,25 +151,28 @@
 
 class FsdpFullCheckpointer(Checkpointer):
     """
     Flash checkpointer to save and load a FSDP full model.
 
     Args:
         checkpoint_dir: the directory to save the checkpoint.
-        storage: A CheckpointStorage instance. The checkpointer will
-            use a PosixStorage instance if the storage is not defined.
         local_shard_num (int): the number of shards on a node,
             The default is 1. If the model is partitioned on all ranks,
             you should set the local_shard_num as the number of ranks
             on a node.
         global_shard_num (int): the number of shards across all ranks.
             The default is 1.If the model is partitioned on all ranks,
             you should set the local_shard_num as the number of all ranks.
         comm_backend (str): the communcation backend to create a process group,
             The default is the backend of general main process group.
+        deletion_strategy: A `CheckpointDeletionStrategy` instance. The default
+            value is None and all checkpoint files will be retained. Now, the
+            strategy can be `KeepLatestStepStrategy`
+            or `KeepStepIntervalStrategy`. Users also can define a strategy
+            to manage the checkpoint files.
 
     Examples::
         >>> checkpointer = FsdpFullCheckpointer(
         >>>     checkpoint_dir="/tmp/checkpoint/"
         >>> )
         >>> for step, data in enumerate(dataloader):
         >>>     ...
@@ -172,23 +184,23 @@
         >>>         )
         >>> sate_dict = checkpointer.load_checkpoint(model, optimizer)
     """
 
     def __init__(
         self,
         checkpoint_dir: str,
-        storage=None,
         comm_backend="",
+        deletion_strategy=None,
     ):
         self.checkpoint_dir = checkpoint_dir
         if dist.is_initialized():
             self._rank = dist.get_rank()
         else:
             self._rank = 0
-        self.storage = PosixDiskStorage() if not storage else storage
+        self.storage = get_checkpoint_storage(deletion_strategy)
         self._engine = FullCheckpointEngine(
             checkpoint_dir=checkpoint_dir,
             storage=self.storage,
             local_shard_num=1,
             global_shard_num=1,
             comm_backend=comm_backend,
         )
```

## dlrover/trainer/torch/flash_checkpoint/fsdp_engine.py

```diff
@@ -415,16 +415,22 @@
 
 class FsdpCheckpointEngine(CheckpointEngine):
     """
     A engine to save FSDP distributed checkpoint into the memory
     and storage.
     """
 
-    def __init__(self, checkpoint_dir: str, storage, comm_backend=""):
-        super().__init__(checkpoint_dir, storage, comm_backend)
+    def __init__(
+        self,
+        checkpoint_dir: str,
+        storage,
+        comm_backend="",
+        save_timeout=CheckpointConstant.SAVE_TIMEOUT,
+    ):
+        super().__init__(checkpoint_dir, storage, comm_backend, save_timeout)
         self._shm_writer = SharedMemoryWriter(shm_handler=self._shm_handler)
         self._shm_reader = SharedMemoryReader(self._shm_handler)
 
     def get_saving_ranks(self):
         """
         Only the local rank 0 in each node saves the state dict into the
         memory. They need to synchronize the saving status.
```

## dlrover/trainer/torch/flash_checkpoint/full_ckpt_engine.py

```diff
@@ -52,21 +52,22 @@
     def __init__(
         self,
         checkpoint_dir,
         storage,
         local_shard_num=1,
         global_shard_num=1,
         comm_backend="",
+        save_timeout=CheckpointConstant.SAVE_TIMEOUT,
     ):
         if global_shard_num < local_shard_num:
             global_shard_num = local_shard_num
             logger.info(f"Set global_shard_num to {local_shard_num}.")
         self._local_shard_num = local_shard_num
         self._global_shard_num = global_shard_num
-        super().__init__(checkpoint_dir, storage, comm_backend)
+        super().__init__(checkpoint_dir, storage, comm_backend, save_timeout)
 
     def get_saving_ranks(self):
         """
         Only the local rank 0 in each node saves the state dict into the
         memory. They need to synchronize the saving status.
         """
         group_size = env_utils.get_group_world_size()
```

## dlrover/trainer/torch/flash_checkpoint/megatron.py

```diff
@@ -48,23 +48,30 @@
 def _get_rank():
     if dist.is_initialized():
         return dist.get_rank()
     return 0
 
 
 class MegatronCheckpointer(Singleton):
-    def __init__(self, checkpoint_dir, storage=None, comm_backend=""):
+    def __init__(
+        self,
+        checkpoint_dir,
+        storage=None,
+        comm_backend="",
+        save_timeout=CheckpointConstant.SAVE_TIMEOUT,
+    ):
         self.state_dict = {}
         self.paths = {}
         self.checkpoint_dir = checkpoint_dir
         self.storage = PosixDiskStorage() if not storage else storage
         self.engine = MegatronCheckpointEngine(
             checkpoint_dir=checkpoint_dir,
             storage=self.storage,
             comm_backend=comm_backend,
+            save_timeout=save_timeout,
         )
 
     def save(self, state_dict, path: str):
         if not isinstance(path, str):
             torch_native_save(state_dict, path)
             return
         if path.endswith(_MODEL_SD_NAME):
@@ -132,28 +139,32 @@
     model,
     optimizer,
     opt_param_scheduler,
     num_floating_point_operations_so_far=0,
     storage_type=StorageType.DISK,
     storage=None,
     comm_backend="",
+    save_timeout=CheckpointConstant.SAVE_TIMEOUT,
 ):
     """
     Synchronously save the the checkpointing state dict into the CPU memory.
 
     Args:
         same as the `megatron.checkpointing.load_checkpoint`
         storage: A CheckpointStorage instance. The checkpointer will
             use a PosixStorage instance if the storage is not defined.
         comm_backend (str): the backend to synchronize when saving the
             checkpoint to the memory.
     """
     args = get_args()
     saver = MegatronCheckpointer.singleton_instance(
-        args.save, storage=storage, comm_backend=comm_backend
+        args.save,
+        storage=storage,
+        comm_backend=comm_backend,
+        save_timeout=save_timeout,
     )
     sig = inspect.signature(megatron_save)
     if storage_type == StorageType.MEMORY:
         torch.save = saver.save
         try:
             if "num_floating_point_operations_so_far" in sig.parameters:
                 megatron_save(
@@ -203,23 +214,27 @@
     model,
     optimizer,
     opt_param_scheduler,
     load_arg="load",
     strict=True,
     storage=None,
     comm_backend="",
+    save_timeout=CheckpointConstant.SAVE_TIMEOUT,
 ):
     """Load the checkpointing state dict. The method firstly
     load the state dict from the CPU memory and then from the storage.
     Args:
         same as the `megatron.checkpointing.load_checkpoint`
     """
     args = get_args()
     checkpointer = MegatronCheckpointer.singleton_instance(
-        args.save, storge=storage, comm_backend=comm_backend
+        args.save,
+        storge=storage,
+        comm_backend=comm_backend,
+        save_timeout=save_timeout,
     )
     torch.load = checkpointer.load
     iteration = megatron_load(
         model, optimizer, opt_param_scheduler, load_arg, strict
     )
     torch.load = torch_native_load
     return iteration
```

## dlrover/trainer/torch/flash_checkpoint/megatron_dist_ckpt.py

```diff
@@ -11,14 +11,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Input/output checkpointing."""
 import os
 import random
 import sys
+from typing import List
 
 import numpy as np
 import torch
 import torch.distributed as dist
 
 from dlrover.python.common.log import default_logger as logger
 
@@ -40,63 +41,157 @@
     from megatron.optimizer.optimizer import ChainedOptimizer
     from megatron.utils import print_rank_0, unwrap_model
 except ImportError:
     logger.warning("Please check the magatron.checkpointing exists.")
 
 from dlrover.python.common.constants import CheckpointConstant
 from dlrover.python.common.singleton import Singleton
-from dlrover.python.common.storage import PosixDiskStorage
+from dlrover.python.common.storage import (
+    CheckpointDeletionStrategy,
+    PosixDiskStorage,
+    PosixStorageWithDeletion,
+)
 from dlrover.trainer.torch.flash_checkpoint.checkpointer import StorageType
 from dlrover.trainer.torch.flash_checkpoint.megatron_engine import (
     MegatronCheckpointEngine,
     MegatronDistCheckpointEngine,
 )
 
 
+class KeepStepIntervalStrategy(CheckpointDeletionStrategy):
+    """
+    The strategy only keeps the step which is a multiple of the keep_interval
+    and clean the other previous step after saving a new step checkpoint.
+
+    Arguments:
+        keep_interval (int): The step interval to keep. If the step is not
+            a multiple of it, the strategy will clean up the step checkpoint
+            after saving a new step checkpoint. For example, when
+            keep_interval=400, the checkpoint of step 200 will be removed
+            if the checkpoint of step 400 is saved.
+        checkpoint_dir (str): The common folder directory of checkpoint of
+            all steps.
+
+    example:
+        keep_strategy = KeepStepIntervalStrategy(
+            keep_interval=400,
+            checkpoint_dir=args.save,
+        )
+        storage = PosixStorageWithDeletion(keep_strategy)
+        iteration, num_floating_point_operations_so_far = load_checkpoint(
+            model, optimizer, opt_param_scheduler, storage=storage
+        )
+        save_checkpoint(iteration, model, optimizer, opt_param_scheduler,
+                        num_floating_point_operations_so_far, storage=storage)
+
+    """
+
+    def __init__(self, keep_interval: int, checkpoint_dir: str):
+        self._keep_interval = keep_interval
+        self._checkpoint_dir = checkpoint_dir
+
+    def clean_up(self, step, delete_func):
+        if step % self._keep_interval == 0:
+            return
+        directory = "iter_{:07d}".format(step)
+        rm_dir = os.path.join(self._checkpoint_dir, str(directory))
+        try:
+            delete_func(rm_dir)
+            logger.info(f"Clean path {rm_dir}")
+        except Exception:
+            logger.warning(f"Fail to clean path {rm_dir}!")
+
+
+class KeepLatestStepStrategy(CheckpointDeletionStrategy):
+    """
+    The strategy only remains the latest steps and delete the outdated
+    checkpoints.
+    Arguments:
+        max_to_keep (int): An integer, the number of checkpoints to keep.
+        checkpoint_dir (str): The common folder directory of checkpoint of
+            all steps.
+    """
+
+    def __init__(self, max_to_keep: int, checkpoint_dir: str):
+        self._max_to_keep = max(max_to_keep, 1)
+        self._checkpoint_dir = checkpoint_dir
+        self._steps: List[int] = []
+
+    def clean_up(self, step, delete_func):
+        self._steps.append(step)
+        if len(self._steps) == self._max_to_keep:
+            rm_step = self._steps.pop(0)
+            directory = "iter_{:07d}".format(rm_step)
+            rm_dir = os.path.join(self._checkpoint_dir, directory)
+            try:
+                delete_func(rm_dir)
+                logger.info(f"Clean path {rm_dir}")
+            except Exception:
+                logger.warning(f"Fail to clean path {rm_dir}!")
+
+
 class MegatronDistCheckpointer(Singleton):
     def __init__(
         self,
         checkpoint_dir,
         storage=None,
         comm_backend="",
         use_distributed_optimizer=False,
+        save_timeout=CheckpointConstant.SAVE_TIMEOUT,
     ):
         self.storage = PosixDiskStorage() if not storage else storage
         if use_distributed_optimizer:
             self.engine = MegatronDistCheckpointEngine(
                 checkpoint_dir=checkpoint_dir,
                 storage=self.storage,
                 comm_backend=comm_backend,
+                save_timeout=save_timeout,
             )
         else:
             self.engine = MegatronCheckpointEngine(
                 checkpoint_dir=checkpoint_dir,
                 storage=self.storage,
                 comm_backend=comm_backend,
+                save_timeout=save_timeout,
             )
 
 
 def save_checkpoint(
     iteration,
     model,
     optimizer,
     opt_param_scheduler,
     num_floating_point_operations_so_far,
     storage_type=StorageType.DISK,
-    storage=None,
     comm_backend="",
+    deletion_strategy=None,
+    save_timeout=CheckpointConstant.SAVE_TIMEOUT,
 ):
-    """Save a model checkpoint."""
+    """
+    Save a model checkpoint.
+    deletion_strategy: A `CheckpointDeletionStrategy` instance. The default
+        value is None and all checkpoint files will be retained. Now, the
+        strategy can be `KeepLatestStepStrategy`
+        or `KeepStepIntervalStrategy`. Users also can define a strategy
+        to manage the checkpoint files.
+    save_timeout (int): the seconds for node rank 0 to wait all
+            ranks save checkpoints. The node rank 0 will skip the checkpoint
+            if some ranks do not finish saving checkpoint in the save_timeout
+            after the node rank 0 finishes saving checkpoint.
+    """
     args = get_args()
 
+    storage = get_checkpoint_storage(deletion_strategy)
+
     checkpointer = MegatronDistCheckpointer.singleton_instance(
         args.save,
         storage=storage,
         comm_backend=comm_backend,
         use_distributed_optimizer=args.use_distributed_optimizer,
+        save_timeout=save_timeout,
     )
 
     # Only rank zero of the data parallel writes to the disk.
     model = unwrap_model(model)
 
     print_rank_0(
         "saving checkpoint at iteration {:7d} to {}".format(
@@ -148,15 +243,15 @@
                 mpu.set_virtual_pipeline_model_parallel_rank(i)
                 model_state_dict["model%d" % i] = model[
                     i
                 ].state_dict_for_save_checkpoint()
 
         # Optimizer stuff.
         if not args.no_save_optim:
-            if optimizer is not None and not args.use_distributed_optimizer:
+            if optimizer is not None:
                 model_state_dict["optimizer"] = optimizer.state_dict()
             if opt_param_scheduler is not None:
                 model_state_dict[
                     "opt_param_scheduler"
                 ] = opt_param_scheduler.state_dict()
 
         # RNG states.
@@ -258,30 +353,41 @@
 
 def load_checkpoint(
     model,
     optimizer,
     opt_param_scheduler,
     load_arg="load",
     strict=True,
-    storage=None,
     comm_backend="",
+    deletion_strategy=None,
+    save_timeout=CheckpointConstant.SAVE_TIMEOUT,
 ):
     """Load a model checkpoint and return the iteration.
     strict (bool): whether to strictly enforce that the keys in
         :attr:`state_dict` of the checkpoint match the names of
         parameters and buffers in model.
+    deletion_strategy: A `CheckpointDeletionStrategy` instance. The default
+        value is None and all checkpoint files will be retained. Now, the
+        strategy can be `KeepLatestStepStrategy`
+        or `KeepStepIntervalStrategy`. Users also can define a strategy
+        to manage the checkpoint files.
+    save_timeout (int): the seconds for node rank 0 to wait all
+            ranks save checkpoints. The node rank 0 will skip the checkpoint
+            if some ranks do not finish saving checkpoint in the save_timeout
+            after the node rank 0 finishes saving checkpoint.
     """
     args = get_args()
     load_dir = getattr(args, load_arg)
-
+    storage = get_checkpoint_storage(deletion_strategy)
     checkpointer = MegatronDistCheckpointer.singleton_instance(
         args.save,
         storage=storage,
         comm_backend=comm_backend,
         use_distributed_optimizer=args.use_distributed_optimizer,
+        save_timeout=save_timeout,
     )
 
     model = unwrap_model(model)
     (
         model_state_dict,
         opt_state_dict,
         checkpoint_name,
@@ -372,17 +478,17 @@
     fix_query_key_value_ordering(model, checkpoint_version)
 
     # Optimizer.
     if not release and not args.finetune and not args.no_load_optim:
         try:
             # Load state dict.
             if optimizer is not None:
-                if not args.use_distributed_optimizer:
-                    optimizer.load_state_dict(model_state_dict["optimizer"])
-                elif isinstance(optimizer, ChainedOptimizer):
+                optimizer.load_state_dict(model_state_dict["optimizer"])
+            if args.use_distributed_optimizer:
+                if isinstance(optimizer, ChainedOptimizer):
                     load_chained_optimizer_parameter_state(
                         optimizer, opt_state_dict
                     )
                 else:
                     load_parameter_state_from_state_dict(
                         optimizer, opt_state_dict
                     )
@@ -568,7 +674,18 @@
     """
     for idx, optimizer in enumerate(chained_optimizer.chained_optimizers):
         if not hasattr(optimizer, "load_parameter_state_from_state_dict"):
             continue
 
         state_dict = states[idx] if states else None
         load_parameter_state_from_state_dict(optimizer, state_dict)
+
+
+def get_checkpoint_storage(deletion_strategy=None):
+    if deletion_strategy:
+        storage = PosixStorageWithDeletion(
+            tracker_file=CheckpointConstant.TRACER_FILE_NAME,
+            deletion_strategy=deletion_strategy,
+        )
+    else:
+        storage = PosixDiskStorage()
+    return storage
```

## dlrover/trainer/torch/flash_checkpoint/megatron_engine.py

```diff
@@ -10,14 +10,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch.distributed as dist
 
 from dlrover.python.common import env_utils
+from dlrover.python.common.constants import CheckpointConstant
 from dlrover.python.elastic_agent.torch.ckpt_saver import (
     CheckpointConfig,
     CheckpointEvent,
     CheckpointEventType,
     MegatronCheckpointSaver,
 )
 
@@ -29,15 +30,21 @@
     The checkpoint engine synchronously writes the state dict of
     Megatron-LM model and optimizer into
     the shared memory and notify the agent in main process to
     asynchronously save the state dict from the shared memory into
     the storage.
     """
 
-    def __init__(self, checkpoint_dir, storage, comm_backend=""):
+    def __init__(
+        self,
+        checkpoint_dir,
+        storage,
+        comm_backend="",
+        save_timeout=CheckpointConstant.SAVE_TIMEOUT,
+    ):
         if dist.is_initialized():
             try:
                 from megatron.core import mpu
             except ImportError:
                 #  Keep back compatibility.
                 from megatron import mpu
 
@@ -49,15 +56,15 @@
         else:
             self._tp_rank = 0
             self._pp_rank = 0
             self._dp_rank = 0
             self._pp_world_size = 1
             self._tp_world_size = 1
 
-        super().__init__(checkpoint_dir, storage, comm_backend)
+        super().__init__(checkpoint_dir, storage, comm_backend, save_timeout)
 
     def get_saving_ranks(self):
         """
         Get the ranks which need to save the sharding state dict into
         the memory.
         """
         world_size = dist.get_world_size()
@@ -148,15 +155,21 @@
     The checkpoint engine synchronously writes the state dict of
     Megatron-LM model and optimizer into
     the shared memory and notify the agent in main process to
     asynchronously save the state dict from the shared memory into
     the storage.
     """
 
-    def __init__(self, checkpoint_dir, storage, comm_backend=""):
+    def __init__(
+        self,
+        checkpoint_dir,
+        storage,
+        comm_backend="",
+        save_timeout=CheckpointConstant.SAVE_TIMEOUT,
+    ):
         if dist.is_initialized():
             try:
                 from megatron.core import mpu
             except ImportError:
                 #  Keep back compatibility.
                 from megatron import mpu
 
@@ -168,15 +181,15 @@
         else:
             self._tp_rank = 0
             self._pp_rank = 0
             self._dp_rank = 0
             self._pp_world_size = 1
             self._tp_world_size = 1
 
-        super().__init__(checkpoint_dir, storage, comm_backend)
+        super().__init__(checkpoint_dir, storage, comm_backend, save_timeout)
 
     def get_saving_ranks(self):
         """
         Get the ranks which need to save the sharding state dict into
         the memory.
         """
         # All ranks
```

## dlrover/trainer/torch/node_check/utils.py

```diff
@@ -36,16 +36,17 @@
 
 def log_execution_time(func):
     def wrapper(*args, **kwargs):
         start = time.time()
         func(*args, **kwargs)
         t = round(time.time() - start, 2)
         local_rank = int(os.environ["LOCAL_RANK"])
+        func_name = func.__name__
         logger.info(
-            f"Time to execute {func} on local rank {local_rank} is {t}."
+            f"Time to execute {func_name} on local rank {local_rank} is {t}s."
         )
 
     return wrapper
 
 
 def mock_error():
     if os.environ.get("MOCK_ERR_RANK"):
```

## Comparing `dlrover-0.3.6.dist-info/LICENSE` & `dlrover-0.3.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dlrover-0.3.6.dist-info/METADATA` & `dlrover-0.3.7.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlrover
-Version: 0.3.6
+Version: 0.3.7
 Summary: An Automatic Distributed Deep Learning Framework
 Home-page: https://github.com/intelligent-machine-learning/dlrover
 Author: Ant Group
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

## Comparing `dlrover-0.3.6.dist-info/RECORD` & `dlrover-0.3.7.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,72 +1,89 @@
 dlrover/Makefile,sha256=gWX_j-z6M1UP3-h331dG--ZiwVIfLORm69qwof9Ke84,411
 dlrover/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/proto/brain.proto,sha256=HGeQp7U1BzaosYfGKjqviFhUAXIqTx9_mWET-kpi1aQ,4439
 dlrover/proto/brain_pb2.py,sha256=HhTGQ1z1CYyPtDSUnZHk3VhqNCaLP4aNWBjvqtNxBek,12755
 dlrover/proto/brain_pb2_grpc.py,sha256=uuc2uMH2lIv4J2RTkTuPPHBUg0xBdm9knKcWLVV7JlI,5867
-dlrover/proto/elastic_training.proto,sha256=iMN4UYjm_IQUubFfT49haACLnqAn1uu6Mi9ij0aeIbc,463
-dlrover/proto/elastic_training_pb2.py,sha256=R30_12ki-n8zEpt4Kn117eYJMZ1-qajQT1SKYUdl63Q,1951
+dlrover/proto/elastic_training.proto,sha256=FsWapiM07CgzK79dzsVJPdIJFzUMCeCPnOwyOOHQVHI,424
+dlrover/proto/elastic_training_pb2.py,sha256=TSxMwUYw95OKU09ss2GeTSa28k3qnsuieHC3GY4ncYo,1838
 dlrover/proto/elastic_training_pb2_grpc.py,sha256=tBlVuVvwEkT28H8GafyXTRDmgD-nnLhHtOpHg875Lvg,4164
 dlrover/python/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/brain/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/brain/client.py,sha256=YntlTJz5_WnkeiSfPY6kRY15z5D5G8uNbbOAAyZTrvI,11103
 dlrover/python/common/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/common/constants.py,sha256=X9HzV8-tGB8uwsdtQOITe7FAbrIbMs86VUtEHtm1AcE,7036
-dlrover/python/common/env_utils.py,sha256=8IQ_d8X1Z23CAUdc2XutLVMp1s_hkjXW1khIWnCsrVI,1715
+dlrover/python/common/constants.py,sha256=WFtlCSKcSkHANJ8wXQsFcKoO1DgcHr7gIpyZKdMQsKk,7195
+dlrover/python/common/diagnosis.py,sha256=XBHYyTtE7NIUlYWbQ1fGZlsoCvsOtu3iOcDbI6wAVYY,2102
+dlrover/python/common/env_utils.py,sha256=mG2a4CSb-LrWAN_XzoDRy5gZgzvToEr4rnntE8uzZiU,1851
 dlrover/python/common/global_context.py,sha256=X7YTAAC1Pd6cxleei3-H_QLFLWjUBQiyGSTwXejkF5A,7547
-dlrover/python/common/grpc.py,sha256=hZpSINdrmaj7YVXdUKglUN_dPAPfxiuSdMro1PAphSo,9966
+dlrover/python/common/grpc.py,sha256=XBpu-6LHrkhXI4Z_gk2OfIbRJ7TFk9apfABD_Uy8H5Q,10181
 dlrover/python/common/log.py,sha256=s1m9hiuvEmUBC7MxSbSlMSJ-XzzHjt3A3BZXz9qtzM8,1377
 dlrover/python/common/multi_process.py,sha256=wy-hsjfWyuJkGQaCbeO-5KXxPWXF1Bq9ffPZuq-oflU,18440
 dlrover/python/common/node.py,sha256=d6Z25RRyptkErW57ENQASygRIAtTHI6sD6eZdCjELBU,11858
 dlrover/python/common/serialize.py,sha256=B2PLB4ROeasn8HiW0eOmUhMNmnFnZNg6Gsl-rhh1L9A,1186
 dlrover/python/common/singleton.py,sha256=TZp-_IcOFUDJ2l5AqYIkC0Ov0kqF3s_i3jDwkyQiHf8,1489
-dlrover/python/common/storage.py,sha256=5oywNBkDzop0_bNY0P5eu1QcQhMmntXrYwLXRkMb5Nw,8635
+dlrover/python/common/storage.py,sha256=HPDHT7c51MHVLiCrFk8jo8ooYrw_ujFZGHLef1Ga_Go,9636
 dlrover/python/elastic_agent/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/elastic_agent/master_client.py,sha256=n3_iZGmPP-H537c7YDJy9hUdkr-V2-6wcQtBzP3fH4k,14237
+dlrover/python/elastic_agent/master_client.py,sha256=83IoAJEBRbg5NIYD7KzMOjbrWVrTcbeByhhR6rgC400,14808
 dlrover/python/elastic_agent/config/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/elastic_agent/config/paral_config_tuner.py,sha256=UwA_nOQspFd920JZQrO2OIlcQLyHL9MW4e_f2J61eF0,3717
+dlrover/python/elastic_agent/datacollector/__init__.py,sha256=wfC0_tw9vplJaggtrT0BB0RM7a2NmB4sfZVnI-sV58E,599
+dlrover/python/elastic_agent/datacollector/cuda_log_collector.py,sha256=Le_HoG2OfXqXAT4RS3LvlhK8A_mHWS_oMSxzpitCMlI,983
+dlrover/python/elastic_agent/datacollector/data_collector.py,sha256=MqD0Qcr0ZgQ57hDtCqzdWrAmtUF3HG1dm5cFp2y7sEo,1124
+dlrover/python/elastic_agent/datacollector/log_collector.py,sha256=a4LSDz3-j2v0fmoCK1cXCrI7zIIuC2Dmcrhofg3_iC4,987
+dlrover/python/elastic_agent/datacollector/metrics_collector.py,sha256=AYYNtYtWVPBv2yHfqNa1u_EqmIbFn5kth25pP20Jehg,1009
 dlrover/python/elastic_agent/monitor/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
+dlrover/python/elastic_agent/monitor/diagnosis.py,sha256=9b1Eg6r1pqKSrw2vSV_0OUjR7bHCaytK9cSj83GONAE,3768
 dlrover/python/elastic_agent/monitor/resource.py,sha256=SmcQU3HwV-UsrxJqil1W-fcUJY8Cc4YxRjAc9sonSsQ,5980
 dlrover/python/elastic_agent/monitor/training.py,sha256=G5MmNLxS26mTlzaN28KNhKmam1ND2-AuSfBo-XOjKHM,4659
 dlrover/python/elastic_agent/sharding/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/elastic_agent/sharding/client.py,sha256=tXZwnb5gkTnKiPBkW29v0E5XtJU0aBrBLG8LEL7RqRU,11734
 dlrover/python/elastic_agent/sychronization/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/elastic_agent/sychronization/sync_client.py,sha256=KpZqNRc9B73jFgeEzDFlyDqbrYoFu2qcVHUIj4ozd-Y,2686
 dlrover/python/elastic_agent/tensorflow/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/elastic_agent/tensorflow/elastic_ps.py,sha256=WcQ4aRYZD1WlkcYvqi5gifAzcSGFjATN7OinqHtSMBQ,3424
 dlrover/python/elastic_agent/tensorflow/hooks.py,sha256=TYelsg4pY0liS5Wfol3oPSqg23GEoKk-uOeWejb-e_8,4226
 dlrover/python/elastic_agent/tensorflow/profile_extractor.py,sha256=N7MsELFbfraXR9SY70XsE7v1T58CQUXbdCebRvyp6UQ,4556
 dlrover/python/elastic_agent/torch/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
-dlrover/python/elastic_agent/torch/ckpt_saver.py,sha256=t3IJyo0LDylKa6kkv_jI_dHKaktFbzuPpvDJY862YRU,40769
+dlrover/python/elastic_agent/torch/ckpt_saver.py,sha256=rfHHTeyj__UW7euW1VBvc835KrGoZUlAR4ahnCUa2Gw,40977
 dlrover/python/elastic_agent/torch/master_kv_store.py,sha256=-nN5erhZNAnpvLtusnDwTGoyOYVvk9DQlvAXFKWhjzE,4594
-dlrover/python/elastic_agent/torch/training.py,sha256=l7M9s2JLLjvSFdQ4MGR1T61CZFgahL6n9D2GS8NCV44,39591
+dlrover/python/elastic_agent/torch/training.py,sha256=M_p8yeFyXb9TF3aNgm7BpQn28xrF22gCakLyjOPDMb0,40001
 dlrover/python/master/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/args.py,sha256=CxR4Pr9j7l5Ta19ILv7qNH5NuOfGtm682qhV_vR_iO4,3044
 dlrover/python/master/dist_master.py,sha256=3iEuSFOEmGUQNOM36HXQCG7XPXskT3w98bdjK_vngEA,11296
 dlrover/python/master/local_master.py,sha256=BvgwihVOSU--F-W59nFLGwv2TnS7IRUUkg5tnVkLRlQ,4416
 dlrover/python/master/main.py,sha256=dCMtDSu1PN8zTd2H6gACy6KyMmcdkOPA9rYVMg--LS8,2550
 dlrover/python/master/master.py,sha256=vE3WebhpEB8alBXUZku-jUXNGkLalK6JMYnEafGfKRs,928
-dlrover/python/master/servicer.py,sha256=pDF1ul92Vmr0FUr2pkvZ0omVInOKVpFEnmofpSZBLzg,23356
+dlrover/python/master/servicer.py,sha256=WVc8ymAeT4qrIAn_gHI6Jozfo8VrrWdrSKFuEZeZPyU,25426
 dlrover/python/master/cluster/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/master/cluster/quota.py,sha256=Kfzb8B1gV7xZXkwsGaiIjISDH9Q0mh1DqNLSBZzTWnw,1124
+dlrover/python/master/diagnosis/__init__.py,sha256=wfC0_tw9vplJaggtrT0BB0RM7a2NmB4sfZVnI-sV58E,599
+dlrover/python/master/diagnosis/diagnosis.py,sha256=ceUVMPE3GkKfWhMyiiT4QsvUkrSpFjumKuz31ZMu6Hc,2665
+dlrover/python/master/diagnosis/diagnosis_data.py,sha256=6p-SRRAU6VWhwBFy3KWChJe2QCT1zfstulfFt08Ku7Q,2068
+dlrover/python/master/diagnosis/diagnostician.py,sha256=zrM4-wGLh7nNl7kXCgnMHl-MMIOgs9h9l_u2kVvtpXc,1369
+dlrover/python/master/diagnosis/inferencechain/__init__.py,sha256=wfC0_tw9vplJaggtrT0BB0RM7a2NmB4sfZVnI-sV58E,599
+dlrover/python/master/diagnosis/inferencechain/common.py,sha256=QN36sEnlpWEof_kg6ifKiUeT5aXzJAlM095J18NdVQo,2313
+dlrover/python/master/diagnosis/inferencechain/inference_chain.py,sha256=L1M_Hb1wUG5hZ8xxdpNZvFUyJzw7pEAcCG-RGnNWKBc,2398
+dlrover/python/master/diagnosis/operator/__init__.py,sha256=wfC0_tw9vplJaggtrT0BB0RM7a2NmB4sfZVnI-sV58E,599
+dlrover/python/master/diagnosis/operator/check_training_hang_operator.py,sha256=bUmUjB10i3-lt21LRoEj4VbwjsdBR5aW3niBtOlFXog,1592
+dlrover/python/master/diagnosis/operator/operator.py,sha256=P8djtXG-pt8v6FZzJ6dGsJ8bCQ0xrAAvCa5fXX-eqwY,1053
 dlrover/python/master/elastic_training/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/elastic_training/elastic_ps.py,sha256=rhplRZ7sfT6hUDD1mPvI8Gpqy8M2RgaFqCI874pQ56Y,3494
 dlrover/python/master/elastic_training/kv_store_service.py,sha256=TTSz8pCc2wifmG_ecUREPDYFwcBgBm97H0G4n8Ta4xA,1017
 dlrover/python/master/elastic_training/net_topology.py,sha256=5Z8QudeA2x00Iu7WrlsHIpvGNiw3AKnQY19ajSOGHk0,2852
 dlrover/python/master/elastic_training/rdzv_manager.py,sha256=r0S0TpNX1nus_YvvjuOzftEawHZzfdeDAZgqosavj-o,22102
 dlrover/python/master/elastic_training/sync_service.py,sha256=EXlW9UlRrn4nO8DNh4WceRJYbNYAC0Z_u_-PSP8caX4,4971
 dlrover/python/master/hyperparams/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/master/hyperparams/simple_strategy_generator.py,sha256=dLAelo1uYfZUzpNwQV9JcP8JV8WAn9HbhGL_hxewJG0,6818
 dlrover/python/master/hyperparams/strategy_generator.py,sha256=PmrcEvdYWTEd3YK2tJySHlyWLLEcn9WBgWTRIJRwfZo,1000
 dlrover/python/master/monitor/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/monitor/error_monitor.py,sha256=tuK57cWuD5WaRcQKVoV9dTTHOiaVW1Aa5PuxmM7ysHw,4490
 dlrover/python/master/monitor/speed_monitor.py,sha256=D3l6fWDarLrwiFlFMqJHfVG-re8WRSLopGBKbMBeXho,7384
 dlrover/python/master/node/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/node/dist_job_manager.py,sha256=4YIDDY_1r_et2gu12sl0fTt08hOs1mNldOEiWrQ99S4,34327
-dlrover/python/master/node/event_callback.py,sha256=bbFSeouRx7f5Fiq_XwG-b8_LFQk9BcBDyQUhzhNzviE,13001
+dlrover/python/master/node/event_callback.py,sha256=YDQt6nNXDIqjtHZagj_BgFcaLTWhyBH1Z1ZLBHSpdPE,13075
 dlrover/python/master/node/job_auto_scaler.py,sha256=ppWqLUwdgcnY8Q3p-JFGaLOrKgzBfazOVsKnBf49lYo,12665
 dlrover/python/master/node/job_manager.py,sha256=AKnVtldVeCZWmhtVWaiKuNpva0m9VBcEu9sImLC71BI,3661
 dlrover/python/master/node/local_job_manager.py,sha256=qFq-R6Eokn3WpKy4BRWRM4YOYf9AqvGOjWpGXqIPry0,5342
 dlrover/python/master/node/ps.py,sha256=eN2FqehCvCd9SfR44M6SYMpISgCWK55_v_voB4YNPag,14448
 dlrover/python/master/node/status_flow.py,sha256=vtZgVEnCmqTdZuRnV17iIVnwumRW2mj6GwUeDiEHqU8,4094
 dlrover/python/master/node/training_node.py,sha256=_6V3mpXtHPo5yiWDyprhLdbSZC5KcStbvuaJ51gKj7Q,13398
 dlrover/python/master/node/worker.py,sha256=OcvkJeS5KMenPUpSEfyO5puloOdHztSELNruajIcZgo,11300
@@ -75,24 +92,24 @@
 dlrover/python/master/resource/job.py,sha256=JqnruLKjJFXRsTROqHeZPkZxCw5PCFnf1avYVb-7y9A,21672
 dlrover/python/master/resource/local_optimizer.py,sha256=Qr4oGr7lDbDjcQIjx9ywEBjBvDCI-NoYW_nxvcIfDVY,15828
 dlrover/python/master/resource/optimizer.py,sha256=E5mGrzoSGbt23fK3k82uYniwazGdtCMpzV8D1a1P8fI,6187
 dlrover/python/master/scaler/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/scaler/base_scaler.py,sha256=CgFgYPyJDgxRoV22dMfQTlVH5f7Sk_gaMgsW5oZuZtQ,2202
 dlrover/python/master/scaler/elasticjob_scaler.py,sha256=O3UuDaL68TS81FoTkahQ-smH_zGmWgwvmr9NFSzet7U,8541
 dlrover/python/master/scaler/factory.py,sha256=NcuKpxoAjrEMqzIsTZEnHOFEmY8LZtRBmFQrKucC04U,1370
-dlrover/python/master/scaler/pod_scaler.py,sha256=ISefeQUwGgJbMP-rLIJzf_xNckePgjtZFxx1yvDy1OA,24649
+dlrover/python/master/scaler/pod_scaler.py,sha256=lw-fCusuURUgp26xd9xP8usobtq962s3576rUKNwbiM,25968
 dlrover/python/master/scaler/ray_scaler.py,sha256=QVL8AWBQec9up0SFJjikURX529lJ4m0eYMSF2OGy_wA,4659
 dlrover/python/master/shard/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/shard/base_dataset_manager.py,sha256=3jQ-kWrffGsGiCUE6_iLh9aug4GXVja-iWjM4lWcZaQ,4574
 dlrover/python/master/shard/batch_dataset_manager.py,sha256=mD8TEi-yww-4G7cTwL-9irEul49twD2HdRk-Y-_4KEw,6964
 dlrover/python/master/shard/dataset_splitter.py,sha256=HqYEgzZ2YwrschCFeXuAjOc8wpkvZsHwtNdEAnIx3m0,16305
 dlrover/python/master/shard/streaming_dataset_manager.py,sha256=vr_-JNbzwR0BkK2g1WIAuIwZXWaJCU6EtYI6EDVm1ZM,7064
 dlrover/python/master/shard/task_manager.py,sha256=dus4fccMWnqFx5kIs1Gc6jwvhBLeEBg8HidyFc-y2Ww,11152
 dlrover/python/master/stats/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/master/stats/job_collector.py,sha256=mUCl-ZH1maL5qWwaYGx5MXD8nQDfN0h3-IV7gxyCbM4,6444
+dlrover/python/master/stats/job_collector.py,sha256=4gxtPDK7dYRTxJL8gZyxafYEuJCYYJAcy3oNiBAjY8k,6683
 dlrover/python/master/stats/reporter.py,sha256=8xDz_C6lBFsiPu647Hqa7iE74xiJGorwaFWxph1a_5Q,8776
 dlrover/python/master/stats/stats_backend.py,sha256=iJGkngsGLkXEWdN_2jv9xSfELrzpA2ow4Nle93WE4cQ,1567
 dlrover/python/master/stats/training_metrics.py,sha256=gaio2HHKCDSpd00JkyKY6y4uW-Y7Yry4Qmyj1svVhls,4820
 dlrover/python/master/watcher/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/watcher/base_watcher.py,sha256=OZkgRItgEMNC53hv59ciNKNc8fSKzX016zRIrINF0vQ,1241
 dlrover/python/master/watcher/factory.py,sha256=lqH-xRNHnzK2yzlLaGntG06j3FuNW_QhIWVwNhzGzLs,1906
 dlrover/python/master/watcher/k8s_watcher.py,sha256=wBQ357qsmmTt0gDF3efljCT2UA-YHmB34jRqJH8-Z3o,11775
@@ -100,57 +117,60 @@
 dlrover/python/scheduler/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/scheduler/factory.py,sha256=yj8B7L6nJC0Kqn_CMdYJ_AkX_HW7wU6rzD7mBZXQ4Oc,1924
 dlrover/python/scheduler/job.py,sha256=EQs2up1YqcRFzaDgQ709PCjVj_pgezIGsNOkz9hjf3E,4285
 dlrover/python/scheduler/kubernetes.py,sha256=ydID-miTeUmJX-_oodr01Di1uSmfETT-LHaD2FoOPx0,18558
 dlrover/python/scheduler/ray.py,sha256=3XOrX-6faq-PSzbKQ5ml3IuVqk82zIwWyptxD3ctYOk,7397
 dlrover/python/tests/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/tests/test_agent_config_tuner.py,sha256=6JGa3UJs2JbC8wo3WIPdwrXrqCZ0jUyfAcIe9xFv9ew,2799
-dlrover/python/tests/test_agent_monitor.py,sha256=HJuwwkDmZ8ncGn98uBftBM1ewPXS8ZwxiflbUWedqI8,3405
+dlrover/python/tests/test_agent_monitor.py,sha256=Ho5eak9bacT-EaePHwrVxcrM5zB1nLAQTplv1LByaFQ,4236
 dlrover/python/tests/test_args.py,sha256=xq0ZkOq0wXdyvjuQppwj8GPR0XmjAUFFcb8GmPe2l4I,1049
 dlrover/python/tests/test_ckpt_saver.py,sha256=rOH_FLL3U_gbnEfgOnIGmhpoEGCRPophe-ZcxkOKS1o,10521
 dlrover/python/tests/test_dataset_splitter.py,sha256=8y2Y1wXThIlZ4f4atVqIxbrWNmUb6fJfyr3t-Xbr58E,4583
 dlrover/python/tests/test_dataset_task_manager.py,sha256=dStylhcl1DIDG6xWTkxXrMXKsvthVos2zu0ZlC5ewag,4905
-dlrover/python/tests/test_elastic_training_agent.py,sha256=djm8z06xAU1q3pjHbz6ETD4Gj6SX8L88W3woRfp-4Jo,14928
+dlrover/python/tests/test_diagnosis.py,sha256=cUoqYxLXhouCLOdeX1VNHkqpuLEuqj0zw3awf3CLCKM,2128
+dlrover/python/tests/test_elastic_training_agent.py,sha256=ESjXEAupwrnp-6mao7lWXKIbwKfVIFKLFCb2Z3f7cvs,14958
 dlrover/python/tests/test_elasticjob_scaler.py,sha256=HB7255Ytru9VltWZkp9Wa3zgaHi4yHMffgLSmF6DrrY,3383
 dlrover/python/tests/test_env_utils.py,sha256=ZomqS03hXAfXYePP5rga9iOnN2Dsq6-0el6n84RLnao,1873
 dlrover/python/tests/test_error_monitor.py,sha256=ScPG7mArYtMGnDWA0ApcsMqdb3sWe3P-SuR0r0d975M,1527
 dlrover/python/tests/test_event_callback.py,sha256=ti3LClbn6yQQ4gN-svxWW5WGk4Hwsd35RdRkLu5OW_s,3635
 dlrover/python/tests/test_global_context.py,sha256=nUQflu6UPsbr5_o3OOZRYbyS7L674QMLazjo2f_OKS4,1268
 dlrover/python/tests/test_grpc_utils.py,sha256=NKe_hTlT3G3CpfZTY3TKImYkx5pgS3Q3RfbkLfVSZYU,2158
 dlrover/python/tests/test_job_auto_scaler.py,sha256=uVhD_zOqUEWI5rorGBra_W0jrancyHijhW4FXmfvMyM,5292
 dlrover/python/tests/test_job_manager.py,sha256=fizGmAhat8ccfojvBjr2GdT6xbllLT0cBl4tqziOn0w,21350
 dlrover/python/tests/test_job_params.py,sha256=WxvoIFzf5qW658Mehru5pwVBlfmjwyTt3oY4yeXD1uM,2183
+dlrover/python/tests/test_k8s_util.py,sha256=VP-5w4i155U-qFAyz_CMUQQhMy-OjuSDvSvlKwV_G0c,1391
 dlrover/python/tests/test_k8s_utils.py,sha256=VcgxfuYZl6hu6E-zhrLJmB-43ykaeoi3tNy7T4FxwQ8,3188
 dlrover/python/tests/test_k8s_watcher.py,sha256=dC5g7jxwuCoVTdbSRYEqYmhH_KpCRoTcXqU3wpqU6kU,5920
 dlrover/python/tests/test_local_optimizer.py,sha256=ngdzP_r2yNntECv1SnsabnCdVgtO4QRjCNy7JNHWAVg,9142
 dlrover/python/tests/test_master.py,sha256=MqkueLGrY05f11ude_omP-SKxPX5m2396KPzqWw9cVE,5449
 dlrover/python/tests/test_master_client.py,sha256=bVfAID_KfMTSxR8-HSmCaGqVJbQAg_Ep_-2ke9b4Tkg,5455
 dlrover/python/tests/test_multi_process.py,sha256=shThZ-ZTB0cQTbbY3TDGMjw0FR6QCea3pFZO4olDx-4,3773
 dlrover/python/tests/test_net_topology.py,sha256=BHuEvjSy9zLmm_oB9SIz4TbqA4aGjoyP2KhuMcLwVjE,1816
 dlrover/python/tests/test_node.py,sha256=JfwSa_xHW8oChUyCKSmB5PTohF6gxxoCQEHxMe8pbXE,1943
-dlrover/python/tests/test_pod_scaler.py,sha256=O_NHV1neCRuUOebd-ECmb9z1PhJ2OVDHOWlabOyhHnY,9506
+dlrover/python/tests/test_pod_scaler.py,sha256=soC0Qvpt9B0uhTcBWakVnEwGpPgaM3VDk6Zd1CSaShc,10099
 dlrover/python/tests/test_ps_manager.py,sha256=mZZYUUZT-apGUq3qH2pwe-1ObnG6F72XIl6gOtmMLe4,7411
 dlrover/python/tests/test_ray_client.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/tests/test_ray_job_args.py,sha256=0gSfBb3u-_GFCj9dOpRdvCJ6g0QFEbi3dudYFt6Pqdo,1976
 dlrover/python/tests/test_ray_scaler.py,sha256=xN4dPhtrMCzKdzckTwELdBbOtzdGbJQtODegm5Ku_KI,971
 dlrover/python/tests/test_ray_watcher.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/tests/test_rdzv_manager.py,sha256=aTcoTMDvA6U7Kd-I6NwQnip0I0YQavq6v-psFTMatI4,12564
 dlrover/python/tests/test_resource_optimizer.py,sha256=R63qFU1nJ9gyMd675ft98IVGCjyWQmVC76uX0eBw-Bo,11635
 dlrover/python/tests/test_servicer.py,sha256=zdZqm9tSC0XvdfxPix6h4TrF77dgNhAxaP89DIZq4X4,18420
 dlrover/python/tests/test_sharding_client.py,sha256=9fsp41zGpwo4tAmVtAg1OOynBteQ639Z6b7UT_40-ko,3687
 dlrover/python/tests/test_speed_monitor.py,sha256=5XBMjXWqyz2x3Ywn4G3f_E9njOOAknnYwyK1M9-U9ew,1783
 dlrover/python/tests/test_state_backend.py,sha256=uocRJZWt1RjcTshOYfseUUiT9Bl9x_7dSNI3cvExJPs,1344
-dlrover/python/tests/test_stats_collector.py,sha256=YZntX9yYoONRuGwaSzZiy5OUAmVy97SGSNAXd-pSkVs,3287
-dlrover/python/tests/test_storage.py,sha256=D_mfwnU5PaQ_3lV9myC1-qoUHZ71mgeZFpPlcqhhb9g,2703
+dlrover/python/tests/test_stats_collector.py,sha256=WjAMI6iGPiYkEa13faV0Di2wbnj5Q545WUluLnjioD0,3535
+dlrover/python/tests/test_storage.py,sha256=v6moOj5xsOeb1kRo8qQBVekOSzYF9_m45Xmij5f9IcA,3497
 dlrover/python/tests/test_strategy_generator.py,sha256=onw1BfpQD9rfU9YbFB0LIHPFB54IlB9A0aS2eu6D0gw,3303
 dlrover/python/tests/test_sync_service.py,sha256=VAIi61kx7BLZKJI5qk-BHk-IC9lEoiD4OqLvPBIV5vk,2460
 dlrover/python/tests/test_task_manager.py,sha256=UE0fFwQrBFEM-LuLZl-vJYCaSM6q7OHI5MjtYdICYPo,5425
-dlrover/python/tests/test_utils.py,sha256=laEXPiPmbHANWcEOAQTkvrvOHqfuZbD010Q3c18OcwM,8599
+dlrover/python/tests/test_utils.py,sha256=_gqdn0yDOvt766v9FKgzcPJphyOlK1A6ShI_gB9tXZM,9310
 dlrover/python/tests/test_worker_manager.py,sha256=-kST3cXREaz8me9PqDBtNz7wA6fsJuX0boTifIMVPPA,7354
 dlrover/python/util/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/python/util/k8s_util.py,sha256=Nb6-5AGLM4kJ-bS1WpdwCuy7djWGHVDEkUTyXzG_zXw,1169
 dlrover/python/util/reflect_util.py,sha256=6d__Wupk46-s5gwg5ChlZSJF5um4GDLhrZN-bz_oTnY,3856
 dlrover/python/util/actor_util/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/util/actor_util/parse_actor.py,sha256=QWQiECvoj4FVX1MnL_BtmCaZ3JHvcCvI-FWc8MVC2nA,1552
 dlrover/python/util/queue/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/util/queue/queue.py,sha256=aVR_a5vk6y5n5BAtMxBMA7XUhV04NUZfpDq7A1TKi8k,2834
 dlrover/python/util/state/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/util/state/memory_store.py,sha256=G9YoCClRxMqW038eIXNXt5K2uQxptEiA5_ZUy28FSj0,2322
@@ -192,45 +212,45 @@
 dlrover/trainer/tensorflow/util/dataset_util.py,sha256=qjz-NlmqBBwp-ztZrhegfJcvDYntjW2pFFzBLFuuPoM,5429
 dlrover/trainer/tensorflow/util/estimator_util.py,sha256=-ULYmgVFALFCd4oLGSbjZc3OQBl0dI26HUC9Uy2tnQc,8506
 dlrover/trainer/tensorflow/util/path_util.py,sha256=LQCCluOm2zR492dVuwW_z_hVtArgXVTkc1mnEjidHms,1122
 dlrover/trainer/tensorflow/util/tf_env_util.py,sha256=Zi0GaRhfHYytKVKcYNbTfh9E89hpRuADYzC0EyE3bjk,1598
 dlrover/trainer/tensorflow/util/tf_patch_util.py,sha256=8LjI9NclFCNPnZ63GIon0qgV7x5XqVUdDMFLkqugy-s,15226
 dlrover/trainer/tensorflow/util/tf_version_util.py,sha256=4zoYq-yImVA_6ymQCBdxwMCNMi8cT7_EQbe78uqq140,1104
 dlrover/trainer/torch/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
-dlrover/trainer/torch/elastic_run.py,sha256=oH5vVMLqHznj6AziPENFUg5d-dI1ZN__yOiz0Errloc,11832
+dlrover/trainer/torch/elastic_run.py,sha256=PUKf3IFoQjfAOh18du4KO8-FqUO77IOZeuIVn2bVVAs,12051
 dlrover/trainer/torch/main.py,sha256=2lZr2YcXAFjKxYn4M4okmbThfnqd88BHUnMHh9jgYQk,690
 dlrover/trainer/torch/elastic/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/trainer/torch/elastic/dataloader.py,sha256=73-mMJyIEi0dOtHsyrYlOhD9vY00glRLP7USkPDfIOc,5422
 dlrover/trainer/torch/elastic/sampler.py,sha256=BLq3BUNiFQOMEAZn5LFdCoGzrptqoWpoApnuhd8RrPU,5981
 dlrover/trainer/torch/elastic/trainer.py,sha256=F_OclqqnTnMcc3fjTXQb5d0ZcG0rXM-GJ9RLrpH1wm8,11244
 dlrover/trainer/torch/flash_checkpoint/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/trainer/torch/flash_checkpoint/checkpointer.py,sha256=uh5SQgZZc_VH2PCGXlaJWhRtBDntq4oOX1nhTbuXyIU,2534
-dlrover/trainer/torch/flash_checkpoint/ddp.py,sha256=jyZtTcEbjHluGkSHYq9DdUs9C_tQXrrwhGcHdlj4P8I,4247
-dlrover/trainer/torch/flash_checkpoint/deepspeed.py,sha256=VnEWkFviXaerkhLeh1Mstlatot5NCcEUygMmQMerL24,8646
-dlrover/trainer/torch/flash_checkpoint/deepspeed_engine.py,sha256=OA-yFN8bit-KgzEpx7cuXiebowuU0z7tO2DX073TC60,6280
-dlrover/trainer/torch/flash_checkpoint/engine.py,sha256=SZJVB53sy7zvR77bxAId4AxuoNyaZJMSOmJ7DbzKUII,14280
-dlrover/trainer/torch/flash_checkpoint/fsdp.py,sha256=Cj5oEe_cHDOW2-QitPfQFduGS2Ym2QrQYKBI01KnhCo,10397
-dlrover/trainer/torch/flash_checkpoint/fsdp_engine.py,sha256=B90iLS8CaNsVzp7JOTmDNIuxFZp9lGfhoiGn7hYgabQ,19976
-dlrover/trainer/torch/flash_checkpoint/full_ckpt_engine.py,sha256=OmQ5ZmCqRh3OvWFj3uYWZbKumPhB7j9kYTFv1lp6quk,7885
+dlrover/trainer/torch/flash_checkpoint/ddp.py,sha256=I5p_tqhaJDpl-F2zM2CyE5vcDLajoA4vq5YFIlCWk2o,4827
+dlrover/trainer/torch/flash_checkpoint/deepspeed.py,sha256=LnFiA2LdHtNVP_OZ4lK0l32fSyelcRmVCFLXENzFawU,9239
+dlrover/trainer/torch/flash_checkpoint/deepspeed_engine.py,sha256=PNiD71kXdZNgk5ZV2jR6PcmKzUS0DlFD5EGqJ7__ZV0,6221
+dlrover/trainer/torch/flash_checkpoint/engine.py,sha256=3ikoVGRgf1qaL5MphnC8-zKRalGe20HVftRmU59tVmg,14498
+dlrover/trainer/torch/flash_checkpoint/fsdp.py,sha256=Sd3um_8V8Zfzpcbg0oC2yfBt4AZnWEsH0iILRIV_7go,10902
+dlrover/trainer/torch/flash_checkpoint/fsdp_engine.py,sha256=5HgY_eojEwvoMvNLWhzuqejHostYq7AzUxJJWyV8f_I,20083
+dlrover/trainer/torch/flash_checkpoint/full_ckpt_engine.py,sha256=uXRIFEUt_jFkIkpFACYNG7TSWh7onSEY3oFL95N-51s,7953
 dlrover/trainer/torch/flash_checkpoint/hf_trainer.py,sha256=_ehKQc_8GPK30lE-mJUpVHMq21ySuvAjOsQ4K0u6eQM,14246
-dlrover/trainer/torch/flash_checkpoint/megatron.py,sha256=5V86EwbyawfT7nRlJqOBdml5M0BwDSnKAALpN38Cqds,7823
-dlrover/trainer/torch/flash_checkpoint/megatron_dist_ckpt.py,sha256=gp-rKa1_6nQalgitl2QNLH-fkFwAL4Ns25ZOx5RZuGY,20464
-dlrover/trainer/torch/flash_checkpoint/megatron_engine.py,sha256=uBcHmHqNDe7Sr0nzfQBE2yaNdraV2SeE2JGW4_5pEvo,9626
+dlrover/trainer/torch/flash_checkpoint/megatron.py,sha256=2ARQfuMRCDt15j6vG6OSzd_qXmHAHYpKI1rDQlpKSUY,8159
+dlrover/trainer/torch/flash_checkpoint/megatron_dist_ckpt.py,sha256=O1FnGW6rI_zUy_uSeLNDQKdUPKRsxb7u4F0iwmCw81w,25238
+dlrover/trainer/torch/flash_checkpoint/megatron_engine.py,sha256=ipZWeo-iRg2tdjNxNMUpBBqZ4Z9Q9K4To_oMdxf8b18,9903
 dlrover/trainer/torch/node_check/__init__.py,sha256=wfC0_tw9vplJaggtrT0BB0RM7a2NmB4sfZVnI-sV58E,599
 dlrover/trainer/torch/node_check/ascend_npu.py,sha256=9mRCvnoUncLqxrPywlAPeKqdY9lBSSmn_YTU3q8PG50,1645
 dlrover/trainer/torch/node_check/nvidia_gpu.py,sha256=ZUvLHUEtRJSVXgNcvhHIrKaRRw5hD3-vSq4q-ewg9h4,1373
-dlrover/trainer/torch/node_check/utils.py,sha256=bnGua0UmYaWIh2P62ggC8y5zHmEgw9klcg2jKAj4pxw,2890
+dlrover/trainer/torch/node_check/utils.py,sha256=LQwI3ULSWLhD203hzg4O079aNJvJWS1bCrJnJjFVgq0,2930
 dlrover/trainer/util/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/trainer/util/args_util.py,sha256=cWIf8seZuB-CZDDj2451M93RhedlZOoiK7Wje_61RJ8,2031
 dlrover/trainer/util/conf_util.py,sha256=0Qzx2glA0nwYe335RRq8zV9Rx-i9tLVKz6Pzz5NO5fs,6436
 dlrover/trainer/util/log_util.py,sha256=v0sxOgR0IWQl6odSXFc1h-GTHyeeCb7-MlQuLjiTfrA,2863
 dlrover/trainer/util/net_util.py,sha256=RLWB5efGRUgaXMbJk0uzdLuyboNEcOVhbFJb-VXG2tI,736
 dlrover/trainer/util/reflect_util.py,sha256=6MSIuzdcKqODcrH35oWINzE-oQa-Y58XIxi3QPkJWGM,3860
 dlrover/trainer/worker/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/trainer/worker/tf_kubernetes_worker.py,sha256=ItXRn7H6ts1XD12dIJD7me5L061dUXIBKHF5lpCAFqI,3540
 dlrover/trainer/worker/tf_ray_worker.py,sha256=AXXhQqiRBAwy0jWrw69HBVR4Qq8qSTPr4ivTrJ7EoSo,6927
-dlrover-0.3.6.dist-info/LICENSE,sha256=9-m2Y33Gdwo-6MPmAHTXF3nBJ7_HBvL5b9_ttmjvKiY,13484
-dlrover-0.3.6.dist-info/METADATA,sha256=Emo-UT6HbOlYQSVSJpd3pvHsozKnqKi74IHPQ761wzI,1008
-dlrover-0.3.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dlrover-0.3.6.dist-info/entry_points.txt,sha256=Yov3tA1wyZ8xs5vw1f6YW7XgzeGtClcj62FfLU9l7wY,65
-dlrover-0.3.6.dist-info/top_level.txt,sha256=DBXgCrSsRqJf0F1cJOaCbBv9tmdt3d7C6qEOFPBhCgg,8
-dlrover-0.3.6.dist-info/RECORD,,
+dlrover-0.3.7.dist-info/LICENSE,sha256=9-m2Y33Gdwo-6MPmAHTXF3nBJ7_HBvL5b9_ttmjvKiY,13484
+dlrover-0.3.7.dist-info/METADATA,sha256=wC901rIBEmFGkRqzPiam430VApSN9ddRsU_SuaF4qyU,1008
+dlrover-0.3.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dlrover-0.3.7.dist-info/entry_points.txt,sha256=Yov3tA1wyZ8xs5vw1f6YW7XgzeGtClcj62FfLU9l7wY,65
+dlrover-0.3.7.dist-info/top_level.txt,sha256=DBXgCrSsRqJf0F1cJOaCbBv9tmdt3d7C6qEOFPBhCgg,8
+dlrover-0.3.7.dist-info/RECORD,,
```

