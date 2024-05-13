# Comparing `tmp/declearn-2.3.2.tar.gz` & `tmp/declearn-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "declearn-2.3.2.tar", last modified: Thu Oct  5 09:52:57 2023, max compression
+gzip compressed data, was "declearn-2.4.0.tar", last modified: Mon Mar 18 14:03:35 2024, max compression
```

## Comparing `declearn-2.3.2.tar` & `declearn-2.4.0.tar`

### file list

```diff
@@ -1,317 +1,339 @@
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.620774 declearn-2.3.2/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3842 2023-09-06 09:27:59.000000 declearn-2.3.2/.gitlab-ci.yml
--rw-r--r--   0 paandrey (670133) magnet   (208235)      566 2023-09-07 11:10:33.000000 declearn-2.3.2/AUTHORS
--rw-r--r--   0 paandrey (670133) magnet   (208235)    11357 2023-03-24 21:43:07.000000 declearn-2.3.2/LICENSE
--rw-r--r--   0 paandrey (670133) magnet   (208235)    20962 2023-10-05 09:52:57.620774 declearn-2.3.2/PKG-INFO
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4977 2023-09-01 10:00:51.000000 declearn-2.3.2/README.md
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.592774 declearn-2.3.2/declearn/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2496 2023-10-05 09:49:54.000000 declearn-2.3.2/declearn/__init__.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.592774 declearn-2.3.2/declearn/aggregator/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1705 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/aggregator/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5617 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/aggregator/_api.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4167 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/aggregator/_base.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4271 2023-03-24 21:43:07.000000 declearn-2.3.2/declearn/aggregator/_gma.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.592774 declearn-2.3.2/declearn/communication/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3086 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/communication/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8224 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/communication/_build.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.592774 declearn-2.3.2/declearn/communication/api/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1248 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/communication/api/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     9146 2023-08-31 09:31:39.000000 declearn-2.3.2/declearn/communication/api/_client.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    13310 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/communication/api/_server.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    16342 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/communication/api/_service.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.592774 declearn-2.3.2/declearn/communication/grpc/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1308 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/communication/grpc/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4811 2023-09-01 09:26:44.000000 declearn-2.3.2/declearn/communication/grpc/_client.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8877 2023-03-24 21:43:07.000000 declearn-2.3.2/declearn/communication/grpc/_server.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/communication/grpc/protobufs/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1398 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/communication/grpc/protobufs/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)      263 2023-08-02 12:54:57.000000 declearn-2.3.2/declearn/communication/grpc/protobufs/message.proto
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1841 2023-03-24 21:43:07.000000 declearn-2.3.2/declearn/communication/grpc/protobufs/message_pb2.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5239 2023-08-02 12:58:33.000000 declearn-2.3.2/declearn/communication/grpc/protobufs/message_pb2_grpc.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/communication/messaging/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2409 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/communication/messaging/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6999 2023-08-31 07:09:04.000000 declearn-2.3.2/declearn/communication/messaging/_messages.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1410 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/communication/messaging/flags.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/communication/websockets/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1143 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/communication/websockets/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5988 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/communication/websockets/_client.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6292 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/communication/websockets/_server.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3616 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/communication/websockets/_tools.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/data_info/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2948 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/data_info/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8345 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/data_info/_base.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     7353 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/data_info/_fields.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/dataset/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2665 2023-09-06 09:27:59.000000 declearn-2.3.2/declearn/dataset/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6139 2023-09-06 09:27:59.000000 declearn-2.3.2/declearn/dataset/_base.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    22330 2023-10-05 08:27:43.000000 declearn-2.3.2/declearn/dataset/_inmemory.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8307 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/dataset/_split_data.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/dataset/examples/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1053 2023-10-05 08:27:43.000000 declearn-2.3.2/declearn/dataset/examples/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5145 2023-10-05 08:18:19.000000 declearn-2.3.2/declearn/dataset/examples/_heart_uci.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3770 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/dataset/examples/_mnist.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/dataset/tensorflow/
--rw-r--r--   0 paandrey (670133) magnet   (208235)      910 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/dataset/tensorflow/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    13966 2023-09-06 09:27:59.000000 declearn-2.3.2/declearn/dataset/tensorflow/_tensorflow.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/dataset/torch/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1385 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/dataset/torch/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    10812 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/dataset/torch/_torch.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4779 2023-09-06 09:27:59.000000 declearn-2.3.2/declearn/dataset/torch/_utils.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/dataset/utils/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1693 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/dataset/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4866 2023-10-05 08:27:43.000000 declearn-2.3.2/declearn/dataset/utils/_save_load.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6022 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/dataset/utils/_sparse.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     7065 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/dataset/utils/_split_classif.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/main/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2160 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/main/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    17375 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/main/_client.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    28091 2023-09-01 10:00:47.000000 declearn-2.3.2/declearn/main/_server.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/main/config/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1739 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/main/config/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     7728 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/main/config/_dataclasses.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5589 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/main/config/_run_config.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     7888 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/main/config/_strategy.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/main/privacy/
--rw-r--r--   0 paandrey (670133) magnet   (208235)      904 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/main/privacy/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    10673 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/main/privacy/_dp_trainer.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.596774 declearn-2.3.2/declearn/main/utils/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2584 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/main/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    21365 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/main/utils/_checkpoint.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5064 2023-03-24 21:43:07.000000 declearn-2.3.2/declearn/main/utils/_constraints.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     7442 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/main/utils/_data_info.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4008 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/main/utils/_early_stop.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    14134 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/main/utils/_training.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/metrics/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2861 2023-09-01 10:00:47.000000 declearn-2.3.2/declearn/metrics/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    12850 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/metrics/_api.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8084 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/metrics/_classif.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5457 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/metrics/_mean.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    11953 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/metrics/_roc_auc.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5260 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/metrics/_rsquared.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1787 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/metrics/_utils.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8185 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/metrics/_wrapper.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/model/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2949 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/model/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1803 2023-09-01 10:00:47.000000 declearn-2.3.2/declearn/model/_utils.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/model/api/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1202 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/model/api/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    11185 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/model/api/_model.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    15983 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/model/api/_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/model/haiku/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1062 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/model/haiku/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    20958 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/model/haiku/_model.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6200 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/model/haiku/_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/model/haiku/utils/
--rw-r--r--   0 paandrey (670133) magnet   (208235)      857 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/model/haiku/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2751 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/model/haiku/utils/_gpu.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/model/sklearn/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1216 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/model/sklearn/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4254 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/model/sklearn/_np_vec.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    19254 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/model/sklearn/_sgd.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/model/tensorflow/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1552 2023-09-01 10:00:47.000000 declearn-2.3.2/declearn/model/tensorflow/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    15417 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/model/tensorflow/_model.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    10658 2023-09-01 10:00:47.000000 declearn-2.3.2/declearn/model/tensorflow/_optim.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    10955 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/model/tensorflow/_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/model/tensorflow/utils/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1881 2023-09-01 10:00:47.000000 declearn-2.3.2/declearn/model/tensorflow/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4455 2023-10-05 08:27:43.000000 declearn-2.3.2/declearn/model/tensorflow/utils/_gpu.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4530 2023-09-01 10:00:47.000000 declearn-2.3.2/declearn/model/tensorflow/utils/_loss.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5360 2023-09-01 10:00:47.000000 declearn-2.3.2/declearn/model/tensorflow/utils/_slices.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/model/torch/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1474 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/model/torch/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    16672 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/model/torch/_model.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    13026 2023-09-01 10:00:47.000000 declearn-2.3.2/declearn/model/torch/_optim.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/model/torch/_samplewise/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2438 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/model/torch/_samplewise/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2860 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/model/torch/_samplewise/functorch.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1677 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/model/torch/_samplewise/shared.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2813 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/model/torch/_samplewise/torchfunc.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     7326 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/model/torch/_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/model/torch/utils/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1094 2023-09-01 10:00:47.000000 declearn-2.3.2/declearn/model/torch/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4641 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/model/torch/utils/_gpu.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.600774 declearn-2.3.2/declearn/optimizer/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1711 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/optimizer/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    19710 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/optimizer/_base.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3130 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/optimizer/_utils.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.604774 declearn-2.3.2/declearn/optimizer/modules/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3002 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/optimizer/modules/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    11020 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/optimizer/modules/_adaptive.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    11323 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/optimizer/modules/_api.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4898 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/optimizer/modules/_clipping.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6600 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/optimizer/modules/_momentum.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6031 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/optimizer/modules/_noise.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    15038 2023-09-01 14:03:12.000000 declearn-2.3.2/declearn/optimizer/modules/_scaffold.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.604774 declearn-2.3.2/declearn/optimizer/regularizers/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1453 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/optimizer/regularizers/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6166 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/optimizer/regularizers/_api.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3405 2023-08-24 14:24:00.000000 declearn-2.3.2/declearn/optimizer/regularizers/_base.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)        0 2023-03-24 21:43:07.000000 declearn-2.3.2/declearn/py.typed
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.604774 declearn-2.3.2/declearn/quickrun/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1811 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/quickrun/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3938 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/quickrun/_config.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6673 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/quickrun/_parser.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     9676 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/quickrun/_run.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.604774 declearn-2.3.2/declearn/test_utils/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1671 2023-09-06 09:27:59.000000 declearn-2.3.2/declearn/test_utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4704 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/test_utils/_argparse.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8728 2023-09-06 09:27:59.000000 declearn-2.3.2/declearn/test_utils/_assertions.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1564 2023-09-06 09:27:59.000000 declearn-2.3.2/declearn/test_utils/_convert.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    11678 2023-09-07 11:10:33.000000 declearn-2.3.2/declearn/test_utils/_gen_ssl.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1772 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/test_utils/_imports.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5887 2023-09-06 09:27:59.000000 declearn-2.3.2/declearn/test_utils/_vectors.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2096 2023-10-05 08:27:43.000000 declearn-2.3.2/declearn/typing.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.604774 declearn-2.3.2/declearn/utils/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5008 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     7741 2023-10-05 08:27:51.000000 declearn-2.3.2/declearn/utils/_dataclass.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4174 2023-09-01 10:00:47.000000 declearn-2.3.2/declearn/utils/_device_policy.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     7056 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/utils/_json.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2968 2023-09-21 08:19:20.000000 declearn-2.3.2/declearn/utils/_logging.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6182 2023-10-05 09:48:56.000000 declearn-2.3.2/declearn/utils/_multiprocess.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1575 2023-03-24 21:43:07.000000 declearn-2.3.2/declearn/utils/_numpy.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    10530 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/utils/_register.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6342 2023-05-04 10:01:14.000000 declearn-2.3.2/declearn/utils/_serialize.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    15250 2023-09-01 10:00:51.000000 declearn-2.3.2/declearn/utils/_toml_config.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.592774 declearn-2.3.2/declearn.egg-info/
--rw-r--r--   0 paandrey (670133) magnet   (208235)    20962 2023-10-05 09:52:57.000000 declearn-2.3.2/declearn.egg-info/PKG-INFO
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8102 2023-10-05 09:52:57.000000 declearn-2.3.2/declearn.egg-info/SOURCES.txt
--rw-r--r--   0 paandrey (670133) magnet   (208235)        1 2023-10-05 09:52:57.000000 declearn-2.3.2/declearn.egg-info/dependency_links.txt
--rw-r--r--   0 paandrey (670133) magnet   (208235)      117 2023-10-05 09:52:57.000000 declearn-2.3.2/declearn.egg-info/entry_points.txt
--rw-r--r--   0 paandrey (670133) magnet   (208235)      691 2023-10-05 09:52:57.000000 declearn-2.3.2/declearn.egg-info/requires.txt
--rw-r--r--   0 paandrey (670133) magnet   (208235)        9 2023-10-05 09:52:57.000000 declearn-2.3.2/declearn.egg-info/top_level.txt
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.604774 declearn-2.3.2/docs/
--rw-r--r--   0 paandrey (670133) magnet   (208235)      215 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/SUMMARY.md
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.604774 declearn-2.3.2/docs/api-reference/
--rw-r--r--   0 paandrey (670133) magnet   (208235)      416 2023-09-21 08:32:24.000000 declearn-2.3.2/docs/api-reference/index.md
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.604774 declearn-2.3.2/docs/devs-guide/
--rw-r--r--   0 paandrey (670133) magnet   (208235)      207 2023-05-04 10:01:14.000000 declearn-2.3.2/docs/devs-guide/SUMMARY.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4762 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/devs-guide/contribute.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2930 2023-05-04 10:01:14.000000 declearn-2.3.2/docs/devs-guide/docs-build.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)    10370 2023-05-04 10:01:14.000000 declearn-2.3.2/docs/devs-guide/docs-style.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)      746 2023-05-04 10:01:14.000000 declearn-2.3.2/docs/devs-guide/index.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)    10125 2023-09-06 09:27:59.000000 declearn-2.3.2/docs/devs-guide/tests.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3884 2023-09-21 08:31:10.000000 declearn-2.3.2/docs/index.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)    12500 2023-09-01 10:00:51.000000 declearn-2.3.2/docs/quickstart.md
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.608774 declearn-2.3.2/docs/release-notes/
--rw-r--r--   0 paandrey (670133) magnet   (208235)      264 2023-10-05 09:49:16.000000 declearn-2.3.2/docs/release-notes/SUMMARY.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)      457 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/release-notes/v2.0.0.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)      380 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/release-notes/v2.0.1.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)      711 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/release-notes/v2.0.2.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1586 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/release-notes/v2.0.3.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4050 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/release-notes/v2.1.0.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1586 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/release-notes/v2.1.1.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8949 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/release-notes/v2.2.0.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1697 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/release-notes/v2.2.1.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)      724 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/release-notes/v2.2.2.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8510 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/release-notes/v2.3.0.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1493 2023-09-07 11:10:33.000000 declearn-2.3.2/docs/release-notes/v2.3.1.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)      877 2023-10-05 09:49:16.000000 declearn-2.3.2/docs/release-notes/v2.3.2.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4794 2023-09-06 09:27:59.000000 declearn-2.3.2/docs/setup.md
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.608774 declearn-2.3.2/docs/user-guide/
--rw-r--r--   0 paandrey (670133) magnet   (208235)      230 2023-09-07 09:42:09.000000 declearn-2.3.2/docs/user-guide/SUMMARY.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4626 2023-05-04 10:01:14.000000 declearn-2.3.2/docs/user-guide/fl_process.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)      799 2023-05-04 10:01:14.000000 declearn-2.3.2/docs/user-guide/index.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4989 2023-05-04 10:01:14.000000 declearn-2.3.2/docs/user-guide/local_dp.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5087 2023-05-04 10:01:14.000000 declearn-2.3.2/docs/user-guide/package.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     9739 2023-09-01 10:00:51.000000 declearn-2.3.2/docs/user-guide/usage.md
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.592774 declearn-2.3.2/examples/
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.608774 declearn-2.3.2/examples/adding_rmsprop/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4600 2023-03-24 21:43:07.000000 declearn-2.3.2/examples/adding_rmsprop/readme.md
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.608774 declearn-2.3.2/examples/heart-uci/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3698 2023-10-05 09:48:56.000000 declearn-2.3.2/examples/heart-uci/client.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1642 2023-09-01 10:00:51.000000 declearn-2.3.2/examples/heart-uci/data.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)      916 2023-03-24 21:43:07.000000 declearn-2.3.2/examples/heart-uci/gen_ssl.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4214 2023-09-01 10:00:51.000000 declearn-2.3.2/examples/heart-uci/readme.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2191 2023-10-05 09:48:56.000000 declearn-2.3.2/examples/heart-uci/run.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4801 2023-09-01 10:00:51.000000 declearn-2.3.2/examples/heart-uci/server.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.608774 declearn-2.3.2/examples/mnist/
--rw-r--r--   0 paandrey (670133) magnet   (208235)      916 2023-09-06 09:27:59.000000 declearn-2.3.2/examples/mnist/generate_ssl.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3183 2023-09-06 09:27:59.000000 declearn-2.3.2/examples/mnist/prepare_data.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6302 2023-09-06 09:27:59.000000 declearn-2.3.2/examples/mnist/readme.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3959 2023-10-05 09:48:56.000000 declearn-2.3.2/examples/mnist/run_client.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2760 2023-10-05 09:48:56.000000 declearn-2.3.2/examples/mnist/run_demo.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5750 2023-09-06 09:27:59.000000 declearn-2.3.2/examples/mnist/run_server.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.608774 declearn-2.3.2/examples/mnist_quickrun/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1628 2023-09-01 10:00:51.000000 declearn-2.3.2/examples/mnist_quickrun/config.toml
--rw-r--r--   0 paandrey (670133) magnet   (208235)    25127 2023-09-01 10:00:51.000000 declearn-2.3.2/examples/mnist_quickrun/mnist.ipynb
--rw-r--r--   0 paandrey (670133) magnet   (208235)      763 2023-09-07 11:10:19.000000 declearn-2.3.2/examples/mnist_quickrun/model.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1167 2023-09-01 10:00:51.000000 declearn-2.3.2/examples/mnist_quickrun/readme.md
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1046 2023-09-07 11:10:30.000000 declearn-2.3.2/mkdocs.yml
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3639 2023-10-05 09:50:05.000000 declearn-2.3.2/pyproject.toml
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.608774 declearn-2.3.2/scripts/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6860 2023-09-06 09:27:59.000000 declearn-2.3.2/scripts/gen_docs.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     7215 2023-09-07 11:10:33.000000 declearn-2.3.2/scripts/run_tests.sh
--rw-r--r--   0 paandrey (670133) magnet   (208235)       38 2023-10-05 09:52:57.620774 declearn-2.3.2/setup.cfg
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.608774 declearn-2.3.2/test/
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.608774 declearn-2.3.2/test/aggregator/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3011 2023-09-01 10:00:51.000000 declearn-2.3.2/test/aggregator/test_aggregator.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.608774 declearn-2.3.2/test/communication/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1680 2023-09-01 09:13:26.000000 declearn-2.3.2/test/communication/conftest.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    10231 2023-09-07 11:10:33.000000 declearn-2.3.2/test/communication/test_exchanges.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    11813 2023-03-24 21:43:07.000000 declearn-2.3.2/test/communication/test_grpc.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    16395 2023-09-01 10:00:51.000000 declearn-2.3.2/test/communication/test_server.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1529 2023-09-01 10:00:51.000000 declearn-2.3.2/test/conftest.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.612774 declearn-2.3.2/test/data_info/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2103 2023-09-07 11:10:33.000000 declearn-2.3.2/test/data_info/test_classes_field.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5335 2023-09-07 11:10:33.000000 declearn-2.3.2/test/data_info/test_data_info_utils.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2008 2023-09-07 11:10:33.000000 declearn-2.3.2/test/data_info/test_datatype_field.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1809 2023-09-07 11:10:33.000000 declearn-2.3.2/test/data_info/test_nbsamples_field.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2569 2023-09-07 11:10:33.000000 declearn-2.3.2/test/data_info/test_shape_field.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.612774 declearn-2.3.2/test/dataset/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4652 2023-09-06 09:27:59.000000 declearn-2.3.2/test/dataset/dataset_testbase.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6439 2023-09-07 11:10:33.000000 declearn-2.3.2/test/dataset/test_dataset_utils.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2259 2023-10-05 08:27:43.000000 declearn-2.3.2/test/dataset/test_examples.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    12503 2023-09-07 11:10:33.000000 declearn-2.3.2/test/dataset/test_inmemory.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5844 2023-09-07 11:10:33.000000 declearn-2.3.2/test/dataset/test_tensorflow_dataset.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     9979 2023-09-07 11:10:33.000000 declearn-2.3.2/test/dataset/test_torch_dataset.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.612774 declearn-2.3.2/test/functional/
--rw-r--r--   0 paandrey (670133) magnet   (208235)      975 2023-09-01 10:00:47.000000 declearn-2.3.2/test/functional/conftest.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    11506 2023-09-06 09:27:59.000000 declearn-2.3.2/test/functional/test_main.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2247 2023-09-01 10:00:51.000000 declearn-2.3.2/test/functional/test_quickrun.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    16558 2023-09-07 11:10:33.000000 declearn-2.3.2/test/functional/test_toy_reg.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.612774 declearn-2.3.2/test/main/
--rw-r--r--   0 paandrey (670133) magnet   (208235)    19053 2023-09-01 10:00:51.000000 declearn-2.3.2/test/main/test_checkpoint.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3721 2023-09-07 11:10:33.000000 declearn-2.3.2/test/main/test_data_info.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4829 2023-09-07 11:10:33.000000 declearn-2.3.2/test/main/test_early_stopping.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    11884 2023-09-21 14:47:52.000000 declearn-2.3.2/test/main/test_train_manager.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6919 2023-09-01 10:00:51.000000 declearn-2.3.2/test/main/test_train_manager_dp.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.612774 declearn-2.3.2/test/metrics/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     7320 2023-09-01 10:00:47.000000 declearn-2.3.2/test/metrics/metric_testing.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4401 2023-09-06 09:27:59.000000 declearn-2.3.2/test/metrics/test_binary_apr.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     7255 2023-09-06 09:27:59.000000 declearn-2.3.2/test/metrics/test_binary_roc.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4735 2023-09-07 11:10:33.000000 declearn-2.3.2/test/metrics/test_mae_mse.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6907 2023-03-24 21:43:07.000000 declearn-2.3.2/test/metrics/test_metricset.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3197 2023-09-06 09:27:59.000000 declearn-2.3.2/test/metrics/test_multi_apr.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3398 2023-09-06 09:27:59.000000 declearn-2.3.2/test/metrics/test_rsquared.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.612774 declearn-2.3.2/test/model/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8721 2023-09-06 09:27:59.000000 declearn-2.3.2/test/model/model_testing.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    10562 2023-09-07 11:10:33.000000 declearn-2.3.2/test/model/test_haiku_model.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5820 2023-09-07 11:10:33.000000 declearn-2.3.2/test/model/test_sksgd_model.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    11109 2023-09-07 11:10:33.000000 declearn-2.3.2/test/model/test_tflow_model.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    11853 2023-09-07 11:10:33.000000 declearn-2.3.2/test/model/test_torch_model.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.616774 declearn-2.3.2/test/optimizer/
--rw-r--r--   0 paandrey (670133) magnet   (208235)      985 2023-03-24 21:43:07.000000 declearn-2.3.2/test/optimizer/conftest.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5258 2023-09-06 09:27:59.000000 declearn-2.3.2/test/optimizer/optim_testing.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6347 2023-09-07 11:10:33.000000 declearn-2.3.2/test/optimizer/test_modules.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     3868 2023-03-24 21:43:07.000000 declearn-2.3.2/test/optimizer/test_noise.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    15787 2023-09-01 10:00:47.000000 declearn-2.3.2/test/optimizer/test_optimizer.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2189 2023-09-07 11:10:33.000000 declearn-2.3.2/test/optimizer/test_regularizers.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4924 2023-09-01 10:00:47.000000 declearn-2.3.2/test/optimizer/test_scaffold.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     8502 2023-09-07 11:10:33.000000 declearn-2.3.2/test/optimizer/test_tflow_optim.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     9907 2023-09-07 11:10:33.000000 declearn-2.3.2/test/optimizer/test_torch_optim.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.616774 declearn-2.3.2/test/quickrun/
--rw-r--r--   0 paandrey (670133) magnet   (208235)    10013 2023-09-07 11:10:33.000000 declearn-2.3.2/test/quickrun/test_quickrun_utils.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.616774 declearn-2.3.2/test/utils/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5388 2023-03-24 21:43:07.000000 declearn-2.3.2/test/utils/test_json.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     6623 2023-09-01 10:00:51.000000 declearn-2.3.2/test/utils/test_register.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5952 2023-03-24 21:43:07.000000 declearn-2.3.2/test/utils/test_serialize.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    15940 2023-09-01 10:00:51.000000 declearn-2.3.2/test/utils/test_toml.py
-drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-10-05 09:52:57.616774 declearn-2.3.2/test/vector/
--rw-r--r--   0 paandrey (670133) magnet   (208235)     5734 2023-09-07 11:10:33.000000 declearn-2.3.2/test/vector/test_generic_vector.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2935 2023-09-07 11:10:33.000000 declearn-2.3.2/test/vector/test_jaxnp_vector.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1488 2023-09-07 11:10:33.000000 declearn-2.3.2/test/vector/test_numpy_vector.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     4001 2023-09-07 11:10:33.000000 declearn-2.3.2/test/vector/test_tflow_vector.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     2800 2023-09-07 11:10:33.000000 declearn-2.3.2/test/vector/test_torch_vector.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)    14826 2023-09-07 11:10:33.000000 declearn-2.3.2/test/vector/vector_testing.py
--rw-r--r--   0 paandrey (670133) magnet   (208235)     1109 2023-09-07 11:10:33.000000 declearn-2.3.2/tox.ini
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.305459 declearn-2.4.0/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      411 2024-03-18 14:00:55.000000 declearn-2.4.0/.gitignore
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3848 2024-02-19 16:17:07.000000 declearn-2.4.0/.gitlab-ci.yml
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      594 2024-03-18 14:00:55.000000 declearn-2.4.0/AUTHORS
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11357 2023-03-24 21:43:07.000000 declearn-2.4.0/LICENSE
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    21212 2024-03-18 14:03:35.305459 declearn-2.4.0/PKG-INFO
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4977 2023-09-01 10:00:51.000000 declearn-2.4.0/README.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.253459 declearn-2.4.0/declearn/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2731 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/__init__.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.253459 declearn-2.4.0/declearn/aggregator/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1833 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/aggregator/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8671 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/aggregator/_api.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5670 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/aggregator/_avg.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6853 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/aggregator/_gma.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.253459 declearn-2.4.0/declearn/communication/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3341 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/communication/__init__.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.253459 declearn-2.4.0/declearn/communication/api/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1248 2024-02-13 13:54:08.000000 declearn-2.4.0/declearn/communication/api/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12099 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/communication/api/_client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    13682 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/communication/api/_server.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.257459 declearn-2.4.0/declearn/communication/api/backend/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1809 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/communication/api/backend/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    17228 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/communication/api/backend/_handler.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5258 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/communication/api/backend/actions.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1815 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/communication/api/backend/flags.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.257459 declearn-2.4.0/declearn/communication/grpc/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1308 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/communication/grpc/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4637 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/communication/grpc/_client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9018 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/communication/grpc/_server.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.257459 declearn-2.4.0/declearn/communication/grpc/protobufs/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1398 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/communication/grpc/protobufs/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      263 2023-08-02 12:54:57.000000 declearn-2.4.0/declearn/communication/grpc/protobufs/message.proto
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1841 2023-03-24 21:43:07.000000 declearn-2.4.0/declearn/communication/grpc/protobufs/message_pb2.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5239 2023-08-02 12:58:33.000000 declearn-2.4.0/declearn/communication/grpc/protobufs/message_pb2_grpc.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.257459 declearn-2.4.0/declearn/communication/messaging/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1843 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/communication/messaging/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3863 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/communication/messaging/_messages.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.257459 declearn-2.4.0/declearn/communication/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2482 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/communication/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8634 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/communication/utils/_build.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5839 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/communication/utils/_parse.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.257459 declearn-2.4.0/declearn/communication/websockets/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1143 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/communication/websockets/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5830 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/communication/websockets/_client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6519 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/communication/websockets/_server.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3616 2023-10-05 11:55:07.000000 declearn-2.4.0/declearn/communication/websockets/_tools.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.257459 declearn-2.4.0/declearn/data_info/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2608 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/data_info/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8345 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/data_info/_base.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4021 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/data_info/_fields.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.257459 declearn-2.4.0/declearn/dataset/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2676 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/dataset/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5345 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/dataset/_base.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    20762 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/dataset/_inmemory.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8307 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/dataset/_split_data.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.261459 declearn-2.4.0/declearn/dataset/examples/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1053 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/dataset/examples/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5145 2023-10-05 08:18:19.000000 declearn-2.4.0/declearn/dataset/examples/_heart_uci.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3770 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/dataset/examples/_mnist.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.261459 declearn-2.4.0/declearn/dataset/tensorflow/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      910 2023-10-05 11:55:07.000000 declearn-2.4.0/declearn/dataset/tensorflow/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    13965 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/dataset/tensorflow/_tensorflow.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.261459 declearn-2.4.0/declearn/dataset/torch/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1385 2023-10-05 11:55:07.000000 declearn-2.4.0/declearn/dataset/torch/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10812 2023-10-05 11:55:07.000000 declearn-2.4.0/declearn/dataset/torch/_torch.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4900 2024-01-26 10:05:22.000000 declearn-2.4.0/declearn/dataset/torch/_utils.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.261459 declearn-2.4.0/declearn/dataset/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1693 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/dataset/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4866 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/dataset/utils/_save_load.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6022 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/dataset/utils/_sparse.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7065 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/dataset/utils/_split_classif.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.261459 declearn-2.4.0/declearn/main/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2160 2024-02-08 13:26:54.000000 declearn-2.4.0/declearn/main/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    19474 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/main/_client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    29869 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/main/_server.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.261459 declearn-2.4.0/declearn/main/config/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1739 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/main/config/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7728 2023-10-05 11:55:07.000000 declearn-2.4.0/declearn/main/config/_dataclasses.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5589 2024-03-14 15:05:08.000000 declearn-2.4.0/declearn/main/config/_run_config.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7888 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/main/config/_strategy.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.261459 declearn-2.4.0/declearn/main/privacy/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      904 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/main/privacy/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10959 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/main/privacy/_dp_trainer.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.261459 declearn-2.4.0/declearn/main/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2584 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/main/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    21409 2024-01-26 10:05:22.000000 declearn-2.4.0/declearn/main/utils/_checkpoint.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5064 2023-03-24 21:43:07.000000 declearn-2.4.0/declearn/main/utils/_constraints.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7442 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/main/utils/_data_info.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4008 2023-10-05 11:55:07.000000 declearn-2.4.0/declearn/main/utils/_early_stop.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    16579 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/main/utils/_training.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.265459 declearn-2.4.0/declearn/messaging/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2058 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/messaging/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5649 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/messaging/_api.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6272 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/messaging/_base.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.265459 declearn-2.4.0/declearn/metrics/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2991 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/metrics/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12741 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/metrics/_api.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8775 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/metrics/_classif.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5591 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/metrics/_mean.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    13469 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/metrics/_roc_auc.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5336 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/metrics/_rsquared.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2042 2024-02-19 16:17:07.000000 declearn-2.4.0/declearn/metrics/_utils.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9469 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/metrics/_wrapper.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.265459 declearn-2.4.0/declearn/model/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2949 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/model/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3334 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/model/_utils.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.265459 declearn-2.4.0/declearn/model/api/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1328 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/model/api/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12135 2024-01-26 10:05:22.000000 declearn-2.4.0/declearn/model/api/_model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    22651 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/model/api/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.265459 declearn-2.4.0/declearn/model/haiku/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1062 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/model/haiku/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    21296 2024-01-26 10:05:22.000000 declearn-2.4.0/declearn/model/haiku/_model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7120 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/model/haiku/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.265459 declearn-2.4.0/declearn/model/haiku/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      857 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/model/haiku/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2751 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/model/haiku/utils/_gpu.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.265459 declearn-2.4.0/declearn/model/sklearn/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1216 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/model/sklearn/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4973 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/model/sklearn/_np_vec.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    19496 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/model/sklearn/_sgd.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.269459 declearn-2.4.0/declearn/model/tensorflow/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1552 2023-09-01 10:00:47.000000 declearn-2.4.0/declearn/model/tensorflow/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    16156 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/model/tensorflow/_model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11221 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/model/tensorflow/_optim.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    13872 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/model/tensorflow/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.269459 declearn-2.4.0/declearn/model/tensorflow/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1881 2023-09-01 10:00:47.000000 declearn-2.4.0/declearn/model/tensorflow/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4625 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/model/tensorflow/utils/_gpu.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4715 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/model/tensorflow/utils/_loss.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5360 2023-09-01 10:00:47.000000 declearn-2.4.0/declearn/model/tensorflow/utils/_slices.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.269459 declearn-2.4.0/declearn/model/torch/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1474 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/model/torch/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    16769 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/model/torch/_model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12880 2024-02-19 16:17:07.000000 declearn-2.4.0/declearn/model/torch/_optim.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.269459 declearn-2.4.0/declearn/model/torch/_samplewise/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2600 2024-01-26 10:05:22.000000 declearn-2.4.0/declearn/model/torch/_samplewise/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2891 2024-01-26 10:05:22.000000 declearn-2.4.0/declearn/model/torch/_samplewise/functorch.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1653 2024-02-19 16:17:07.000000 declearn-2.4.0/declearn/model/torch/_samplewise/shared.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2894 2024-01-26 10:05:22.000000 declearn-2.4.0/declearn/model/torch/_samplewise/torchfunc.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8556 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/model/torch/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.269459 declearn-2.4.0/declearn/model/torch/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1094 2023-09-01 10:00:47.000000 declearn-2.4.0/declearn/model/torch/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4554 2024-02-19 16:17:07.000000 declearn-2.4.0/declearn/model/torch/utils/_gpu.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.269459 declearn-2.4.0/declearn/optimizer/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1711 2024-02-29 14:40:58.000000 declearn-2.4.0/declearn/optimizer/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    19745 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/optimizer/_base.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3130 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/optimizer/_utils.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.269459 declearn-2.4.0/declearn/optimizer/modules/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3250 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/optimizer/modules/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11020 2023-11-22 10:04:45.000000 declearn-2.4.0/declearn/optimizer/modules/_adaptive.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12377 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/optimizer/modules/_api.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4898 2023-10-05 11:55:07.000000 declearn-2.4.0/declearn/optimizer/modules/_clipping.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6600 2023-11-22 10:06:23.000000 declearn-2.4.0/declearn/optimizer/modules/_momentum.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6031 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/optimizer/modules/_noise.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    17208 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/optimizer/modules/_scaffold.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.269459 declearn-2.4.0/declearn/optimizer/regularizers/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1453 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/optimizer/regularizers/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6166 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/optimizer/regularizers/_api.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3405 2023-08-24 14:24:00.000000 declearn-2.4.0/declearn/optimizer/regularizers/_base.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)        0 2023-03-24 21:43:07.000000 declearn-2.4.0/declearn/py.typed
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.269459 declearn-2.4.0/declearn/quickrun/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1811 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/quickrun/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3938 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/quickrun/_config.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6673 2023-10-05 11:55:07.000000 declearn-2.4.0/declearn/quickrun/_parser.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9702 2024-01-26 10:05:22.000000 declearn-2.4.0/declearn/quickrun/_run.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.273459 declearn-2.4.0/declearn/test_utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1671 2024-03-18 08:20:47.000000 declearn-2.4.0/declearn/test_utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4704 2023-09-01 10:00:51.000000 declearn-2.4.0/declearn/test_utils/_argparse.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8728 2023-10-05 11:55:07.000000 declearn-2.4.0/declearn/test_utils/_assertions.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1564 2023-10-05 11:55:07.000000 declearn-2.4.0/declearn/test_utils/_convert.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11678 2023-10-05 11:55:07.000000 declearn-2.4.0/declearn/test_utils/_gen_ssl.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1772 2023-10-10 13:58:08.000000 declearn-2.4.0/declearn/test_utils/_imports.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5907 2024-02-19 16:17:07.000000 declearn-2.4.0/declearn/test_utils/_vectors.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2096 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/typing.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.273459 declearn-2.4.0/declearn/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5156 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8142 2024-03-18 14:00:51.000000 declearn-2.4.0/declearn/utils/_aggregate.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7779 2024-01-26 10:05:22.000000 declearn-2.4.0/declearn/utils/_dataclass.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4174 2023-09-01 10:00:47.000000 declearn-2.4.0/declearn/utils/_device_policy.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7056 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/utils/_json.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2968 2023-09-21 08:19:20.000000 declearn-2.4.0/declearn/utils/_logging.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9048 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/utils/_multiprocess.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1575 2024-01-29 14:34:31.000000 declearn-2.4.0/declearn/utils/_numpy.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10530 2023-05-04 10:01:14.000000 declearn-2.4.0/declearn/utils/_register.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6342 2024-03-01 12:44:45.000000 declearn-2.4.0/declearn/utils/_serialize.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    15250 2023-11-02 15:50:40.000000 declearn-2.4.0/declearn/utils/_toml_config.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      794 2024-03-18 14:00:55.000000 declearn-2.4.0/declearn/version.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.297459 declearn-2.4.0/declearn.egg-info/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    21212 2024-03-18 14:03:35.000000 declearn-2.4.0/declearn.egg-info/PKG-INFO
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8717 2024-03-18 14:03:35.000000 declearn-2.4.0/declearn.egg-info/SOURCES.txt
+-rw-r--r--   0 paandrey (670133) magnet   (208235)        1 2024-03-18 14:03:35.000000 declearn-2.4.0/declearn.egg-info/dependency_links.txt
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      117 2024-03-18 14:03:35.000000 declearn-2.4.0/declearn.egg-info/entry_points.txt
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      909 2024-03-18 14:03:35.000000 declearn-2.4.0/declearn.egg-info/requires.txt
+-rw-r--r--   0 paandrey (670133) magnet   (208235)        9 2024-03-18 14:03:35.000000 declearn-2.4.0/declearn.egg-info/top_level.txt
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.273459 declearn-2.4.0/docs/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      215 2023-11-29 13:31:58.000000 declearn-2.4.0/docs/SUMMARY.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.273459 declearn-2.4.0/docs/api-reference/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      416 2024-03-13 15:01:57.000000 declearn-2.4.0/docs/api-reference/index.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.277459 declearn-2.4.0/docs/devs-guide/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      207 2023-05-04 10:01:14.000000 declearn-2.4.0/docs/devs-guide/SUMMARY.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4765 2024-03-18 14:00:55.000000 declearn-2.4.0/docs/devs-guide/contribute.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2930 2023-05-04 10:01:14.000000 declearn-2.4.0/docs/devs-guide/docs-build.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10370 2023-05-04 10:01:14.000000 declearn-2.4.0/docs/devs-guide/docs-style.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      746 2023-05-04 10:01:14.000000 declearn-2.4.0/docs/devs-guide/index.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10125 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/devs-guide/tests.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3884 2024-03-13 14:58:46.000000 declearn-2.4.0/docs/index.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12551 2024-01-26 10:05:22.000000 declearn-2.4.0/docs/quickstart.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.281459 declearn-2.4.0/docs/release-notes/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      286 2024-03-18 14:00:55.000000 declearn-2.4.0/docs/release-notes/SUMMARY.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      457 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/release-notes/v2.0.0.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      380 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/release-notes/v2.0.1.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      711 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/release-notes/v2.0.2.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1586 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/release-notes/v2.0.3.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4050 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/release-notes/v2.1.0.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1586 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/release-notes/v2.1.1.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8949 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/release-notes/v2.2.0.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1697 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/release-notes/v2.2.1.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      724 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/release-notes/v2.2.2.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8510 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/release-notes/v2.3.0.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1493 2023-10-05 11:55:07.000000 declearn-2.4.0/docs/release-notes/v2.3.1.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      877 2023-11-29 13:16:31.000000 declearn-2.4.0/docs/release-notes/v2.3.2.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    14591 2024-03-18 14:01:29.000000 declearn-2.4.0/docs/release-notes/v2.4.0.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5328 2024-03-18 14:00:55.000000 declearn-2.4.0/docs/setup.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.281459 declearn-2.4.0/docs/user-guide/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      277 2024-01-12 13:58:06.000000 declearn-2.4.0/docs/user-guide/SUMMARY.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5085 2024-03-18 14:00:55.000000 declearn-2.4.0/docs/user-guide/fl_process.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      928 2024-01-12 13:58:06.000000 declearn-2.4.0/docs/user-guide/index.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4989 2023-05-04 10:01:14.000000 declearn-2.4.0/docs/user-guide/local_dp.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    31304 2024-03-18 14:00:55.000000 declearn-2.4.0/docs/user-guide/optimizer.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8136 2024-03-18 14:00:55.000000 declearn-2.4.0/docs/user-guide/package.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9739 2024-02-19 09:49:07.000000 declearn-2.4.0/docs/user-guide/usage.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.249459 declearn-2.4.0/examples/
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.281459 declearn-2.4.0/examples/adding_rmsprop/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4600 2023-03-24 21:43:07.000000 declearn-2.4.0/examples/adding_rmsprop/readme.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.285459 declearn-2.4.0/examples/heart-uci/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3915 2024-02-19 13:44:10.000000 declearn-2.4.0/examples/heart-uci/client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1642 2024-02-19 13:37:03.000000 declearn-2.4.0/examples/heart-uci/data.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      916 2023-03-24 21:43:07.000000 declearn-2.4.0/examples/heart-uci/gen_ssl.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4214 2023-09-01 10:00:51.000000 declearn-2.4.0/examples/heart-uci/readme.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2308 2024-03-18 14:00:55.000000 declearn-2.4.0/examples/heart-uci/run.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4801 2024-02-19 13:37:21.000000 declearn-2.4.0/examples/heart-uci/server.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.285459 declearn-2.4.0/examples/mnist/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      916 2023-10-05 11:55:07.000000 declearn-2.4.0/examples/mnist/generate_ssl.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3183 2023-10-05 11:55:07.000000 declearn-2.4.0/examples/mnist/prepare_data.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6302 2023-10-05 11:55:07.000000 declearn-2.4.0/examples/mnist/readme.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3984 2024-01-26 10:05:22.000000 declearn-2.4.0/examples/mnist/run_client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2754 2024-02-15 11:01:59.000000 declearn-2.4.0/examples/mnist/run_demo.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5750 2024-02-12 15:17:41.000000 declearn-2.4.0/examples/mnist/run_server.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.285459 declearn-2.4.0/examples/mnist_quickrun/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1687 2024-01-26 10:05:22.000000 declearn-2.4.0/examples/mnist_quickrun/config.toml
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    25780 2024-01-26 10:05:22.000000 declearn-2.4.0/examples/mnist_quickrun/mnist.ipynb
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1417 2024-01-26 10:05:22.000000 declearn-2.4.0/examples/mnist_quickrun/model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1352 2024-01-26 10:05:22.000000 declearn-2.4.0/examples/mnist_quickrun/model_torch.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1167 2023-09-01 10:00:51.000000 declearn-2.4.0/examples/mnist_quickrun/readme.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1088 2024-01-12 13:58:06.000000 declearn-2.4.0/mkdocs.yml
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3869 2024-03-18 14:00:55.000000 declearn-2.4.0/pyproject.toml
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.285459 declearn-2.4.0/scripts/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7000 2024-03-18 14:00:55.000000 declearn-2.4.0/scripts/gen_docs.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7631 2024-03-18 14:00:55.000000 declearn-2.4.0/scripts/run_tests.sh
+-rw-r--r--   0 paandrey (670133) magnet   (208235)       38 2024-03-18 14:03:35.305459 declearn-2.4.0/setup.cfg
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.285459 declearn-2.4.0/test/
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.285459 declearn-2.4.0/test/aggregator/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6641 2024-03-18 14:00:51.000000 declearn-2.4.0/test/aggregator/test_aggregator.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.289459 declearn-2.4.0/test/communication/
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.289459 declearn-2.4.0/test/communication/backend/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4067 2024-03-18 14:00:51.000000 declearn-2.4.0/test/communication/backend/test_actions.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    16543 2024-03-18 14:00:51.000000 declearn-2.4.0/test/communication/backend/test_messages_handler.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1680 2023-09-01 09:13:26.000000 declearn-2.4.0/test/communication/conftest.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10837 2024-03-18 14:00:51.000000 declearn-2.4.0/test/communication/test_exchanges.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12017 2024-03-18 14:00:51.000000 declearn-2.4.0/test/communication/test_grpc.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    17492 2024-03-18 14:00:51.000000 declearn-2.4.0/test/communication/test_server.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7628 2024-03-18 14:00:55.000000 declearn-2.4.0/test/communication/test_utils.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1529 2023-09-01 10:00:51.000000 declearn-2.4.0/test/conftest.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.289459 declearn-2.4.0/test/data_info/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2103 2023-10-05 11:55:07.000000 declearn-2.4.0/test/data_info/test_classes_field.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5335 2023-10-05 11:55:07.000000 declearn-2.4.0/test/data_info/test_data_info_utils.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2008 2023-10-05 11:55:07.000000 declearn-2.4.0/test/data_info/test_datatype_field.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1809 2023-10-05 11:55:07.000000 declearn-2.4.0/test/data_info/test_nbsamples_field.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2569 2023-10-05 11:55:07.000000 declearn-2.4.0/test/data_info/test_shape_field.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.289459 declearn-2.4.0/test/dataset/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4651 2024-03-18 14:00:55.000000 declearn-2.4.0/test/dataset/dataset_testbase.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6439 2023-10-05 11:55:07.000000 declearn-2.4.0/test/dataset/test_dataset_utils.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2259 2024-03-18 14:00:51.000000 declearn-2.4.0/test/dataset/test_examples.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12503 2023-10-05 11:55:07.000000 declearn-2.4.0/test/dataset/test_inmemory.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5844 2023-10-05 11:55:07.000000 declearn-2.4.0/test/dataset/test_tensorflow_dataset.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9979 2024-03-18 14:00:55.000000 declearn-2.4.0/test/dataset/test_torch_dataset.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.289459 declearn-2.4.0/test/functional/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      975 2023-09-01 10:00:47.000000 declearn-2.4.0/test/functional/conftest.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11719 2024-03-18 14:00:55.000000 declearn-2.4.0/test/functional/test_main.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2310 2024-03-18 14:00:51.000000 declearn-2.4.0/test/functional/test_quickrun.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    16684 2024-03-18 14:00:51.000000 declearn-2.4.0/test/functional/test_toy_reg.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.293459 declearn-2.4.0/test/main/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    19053 2024-03-18 14:00:55.000000 declearn-2.4.0/test/main/test_checkpoint.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3721 2023-10-05 11:55:07.000000 declearn-2.4.0/test/main/test_data_info.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4829 2023-10-05 11:55:07.000000 declearn-2.4.0/test/main/test_early_stopping.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12860 2024-03-18 14:00:51.000000 declearn-2.4.0/test/main/test_train_manager.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6862 2024-03-18 14:00:51.000000 declearn-2.4.0/test/main/test_train_manager_dp.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.293459 declearn-2.4.0/test/metrics/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11548 2024-03-18 14:00:51.000000 declearn-2.4.0/test/metrics/metric_testing.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4401 2024-01-22 10:54:32.000000 declearn-2.4.0/test/metrics/test_binary_apr.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7985 2024-03-18 14:00:55.000000 declearn-2.4.0/test/metrics/test_binary_roc.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4044 2024-03-18 14:00:51.000000 declearn-2.4.0/test/metrics/test_mae_mse.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7630 2024-03-18 14:00:51.000000 declearn-2.4.0/test/metrics/test_metricset.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3261 2024-03-18 14:00:51.000000 declearn-2.4.0/test/metrics/test_multi_apr.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3450 2024-03-18 14:00:51.000000 declearn-2.4.0/test/metrics/test_rsquared.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.293459 declearn-2.4.0/test/model/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9022 2024-03-18 14:00:55.000000 declearn-2.4.0/test/model/model_testing.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10708 2024-03-18 14:00:55.000000 declearn-2.4.0/test/model/test_haiku_model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5472 2024-03-18 14:00:55.000000 declearn-2.4.0/test/model/test_sksgd_model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12051 2024-03-18 14:00:55.000000 declearn-2.4.0/test/model/test_tflow_model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12581 2024-03-18 14:00:55.000000 declearn-2.4.0/test/model/test_torch_model.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.293459 declearn-2.4.0/test/optimizer/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1190 2024-02-19 16:17:07.000000 declearn-2.4.0/test/optimizer/conftest.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5284 2024-03-18 14:00:51.000000 declearn-2.4.0/test/optimizer/optim_testing.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6259 2024-03-18 14:00:51.000000 declearn-2.4.0/test/optimizer/test_modules.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3868 2023-03-24 21:43:07.000000 declearn-2.4.0/test/optimizer/test_noise.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    15867 2024-03-18 14:00:51.000000 declearn-2.4.0/test/optimizer/test_optimizer.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2189 2023-11-23 10:30:57.000000 declearn-2.4.0/test/optimizer/test_regularizers.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9551 2024-03-18 14:00:51.000000 declearn-2.4.0/test/optimizer/test_scaffold.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9039 2024-03-18 14:00:55.000000 declearn-2.4.0/test/optimizer/test_tflow_optim.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9842 2024-02-19 16:17:07.000000 declearn-2.4.0/test/optimizer/test_torch_optim.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.297459 declearn-2.4.0/test/quickrun/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10013 2023-10-05 11:55:07.000000 declearn-2.4.0/test/quickrun/test_quickrun_utils.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.297459 declearn-2.4.0/test/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5388 2023-03-24 21:43:07.000000 declearn-2.4.0/test/utils/test_json.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6352 2024-02-19 16:17:07.000000 declearn-2.4.0/test/utils/test_multiprocess.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6623 2023-09-01 10:00:51.000000 declearn-2.4.0/test/utils/test_register.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5952 2023-03-24 21:43:07.000000 declearn-2.4.0/test/utils/test_serialize.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    15940 2023-09-01 10:00:51.000000 declearn-2.4.0/test/utils/test_toml.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2024-03-18 14:03:35.297459 declearn-2.4.0/test/vector/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1147 2024-02-19 16:17:07.000000 declearn-2.4.0/test/vector/conftest.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7754 2024-03-18 14:00:51.000000 declearn-2.4.0/test/vector/test_generic_vector.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2953 2024-02-19 16:17:07.000000 declearn-2.4.0/test/vector/test_jaxnp_vector.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1488 2023-10-05 11:55:07.000000 declearn-2.4.0/test/vector/test_numpy_vector.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3925 2024-02-19 16:17:07.000000 declearn-2.4.0/test/vector/test_tflow_vector.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2724 2024-02-19 16:17:07.000000 declearn-2.4.0/test/vector/test_torch_vector.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    16409 2024-03-18 14:00:51.000000 declearn-2.4.0/test/vector/vector_testing.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2044 2024-02-19 16:17:07.000000 declearn-2.4.0/tox.ini
```

### Comparing `declearn-2.3.2/.gitlab-ci.yml` & `declearn-2.4.0/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -99,29 +99,29 @@
 # Basic test suite: skip GPU use and a few extra integration tests scenarios.
 # This job is called when commits are pushed to a non-draft MR branch.
 # It may also be called manually on commits to draft MR branches.
 test-minimal:
   extends:
     .test_cfg
   script:
-    - tox -e py38 --workdir=$TOX_WORKDIR -- --cpu-only
+    - tox -e py38-ci --workdir=$TOX_WORKDIR -- --cpu-only
   rules:
     - if: $IS_MERGE_REQ && ($CI_MERGE_REQUEST_TITLE !~ /^Draft:.*/)
     - if: $IS_MERGE_REQ && ($CI_MERGE_REQUEST_TITLE =~ /^Draft:.*/)
       when: manual
       allow_failure: true
 
 # Exhaustive test suite: lint the code, run all tests, use GPU when available.
 # This job is called when commits are pushed to a main branch.
 # It may also be called manually on commits to MR branches.
 test-maximal:
   extends:
     .test_cfg
   script:
-    - tox -e py38 --workdir=$TOX_WORKDIR -- --fulltest
+    - tox -e py38-ci --workdir=$TOX_WORKDIR -- --fulltest
   rules:
     - if: $IS_CORE_PUSH
     - if: $IS_MERGE_REQ
       when: manual
       allow_failure: true  # do not block the base "test" pipeline
   tags:
     - gpu
```

### Comparing `declearn-2.3.2/AUTHORS` & `declearn-2.4.0/AUTHORS`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 This file maintains the list of present and past declearn authors.
 A secondary file listing punctual open-source contributors may complement it.
 
+Declearn 2.4
+- Paul Andrey
+
 Declearn 2.1 - 2.3
 - Paul Andrey
 - Nathan Bigaud
 
 Declearn 2.0 (new implementation)
 - Paul Andrey (core developer)
 - Nathan Bigaud (core developer)
```

### Comparing `declearn-2.3.2/LICENSE` & `declearn-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/PKG-INFO` & `declearn-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: declearn
-Version: 2.3.2
+Version: 2.4.0
 Summary: Declearn - a python package for private decentralized learning.
 Author-email: Paul Andrey <paul.andrey@inria.fr>, Nathan Bigaud <nathan.bigaud@inria.fr>
 Maintainer-email: Paul Andrey <paul.andrey@inria.fr>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -221,60 +221,62 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: cryptography>=35.0
-Requires-Dist: fire>=0.4
-Requires-Dist: pandas>=1.2
+Requires-Dist: fire~=0.4
+Requires-Dist: pandas<3.0,>=1.2
 Requires-Dist: requests~=2.18
-Requires-Dist: scikit-learn>=1.0
-Requires-Dist: tomli>=2.0; python_version < "3.11"
-Requires-Dist: typing_extensions>=4.0
+Requires-Dist: scikit-learn~=1.0
+Requires-Dist: tomli~=2.0; python_version < "3.11"
+Requires-Dist: tqdm~=4.62
+Requires-Dist: typing_extensions~=4.0
 Provides-Extra: all
-Requires-Dist: dm-haiku~=0.0.9; extra == "all"
-Requires-Dist: functorch<3.0,>=1.10; extra == "all"
+Requires-Dist: dm-haiku<=0.0.11,>=0.0.9; python_version > "3.8" and extra == "all"
+Requires-Dist: dm-haiku<=0.0.10,>=0.0.9; python_version == "3.8" and extra == "all"
 Requires-Dist: grpcio>=1.45; extra == "all"
 Requires-Dist: jax[cpu]~=0.4.1; extra == "all"
-Requires-Dist: opacus~=1.1; extra == "all"
+Requires-Dist: opacus~=1.4; extra == "all"
 Requires-Dist: protobuf>=3.19; extra == "all"
-Requires-Dist: tensorflow~=2.5; extra == "all"
-Requires-Dist: torch<3.0,>=1.10; extra == "all"
-Requires-Dist: websockets~=10.1; extra == "all"
+Requires-Dist: tensorflow~=2.11; extra == "all"
+Requires-Dist: torch<3.0,>=1.13; extra == "all"
+Requires-Dist: websockets<13.0,>=10.1; extra == "all"
 Provides-Extra: dp
-Requires-Dist: opacus~=1.1; extra == "dp"
+Requires-Dist: opacus~=1.4; extra == "dp"
 Provides-Extra: grpc
 Requires-Dist: grpcio>=1.45; extra == "grpc"
 Requires-Dist: protobuf>=3.19; extra == "grpc"
 Provides-Extra: haiku
-Requires-Dist: dm-haiku~=0.0.9; extra == "haiku"
+Requires-Dist: dm-haiku<=0.0.11,>=0.0.9; python_version > "3.8" and extra == "haiku"
+Requires-Dist: dm-haiku<=0.0.10,>=0.0.9; python_version == "3.8" and extra == "haiku"
 Requires-Dist: jax[cpu]~=0.4.1; extra == "haiku"
 Provides-Extra: tensorflow
-Requires-Dist: tensorflow~=2.5; extra == "tensorflow"
+Requires-Dist: tensorflow~=2.11; extra == "tensorflow"
 Provides-Extra: torch
 Requires-Dist: torch<3.0,>=1.13; extra == "torch"
 Provides-Extra: torch1
 Requires-Dist: torch~=1.13.0; extra == "torch1"
 Provides-Extra: torch2
 Requires-Dist: torch~=2.0; extra == "torch2"
 Provides-Extra: websockets
-Requires-Dist: websockets~=10.1; extra == "websockets"
+Requires-Dist: websockets<13.0,>=10.1; extra == "websockets"
 Provides-Extra: docs
-Requires-Dist: mkdocstrings[python]>=0.8; extra == "docs"
-Requires-Dist: mkdocs-autorefs; extra == "docs"
-Requires-Dist: mkdocs-literate-nav; extra == "docs"
-Requires-Dist: mkdocs-material>=9.1; extra == "docs"
+Requires-Dist: mkdocstrings[python]~=0.8; extra == "docs"
+Requires-Dist: mkdocs-autorefs~=0.4; extra == "docs"
+Requires-Dist: mkdocs-literate-nav~=0.4; extra == "docs"
+Requires-Dist: mkdocs-material~=9.1; extra == "docs"
 Provides-Extra: tests
-Requires-Dist: black~=23.0; extra == "tests"
+Requires-Dist: black~=24.0; extra == "tests"
 Requires-Dist: mypy~=1.0; extra == "tests"
-Requires-Dist: pylint>=2.14; extra == "tests"
-Requires-Dist: pytest>=6.1; extra == "tests"
-Requires-Dist: pytest-asyncio; extra == "tests"
-Requires-Dist: pytest-cov>=4.0; extra == "tests"
+Requires-Dist: pylint~=3.0; extra == "tests"
+Requires-Dist: pytest~=7.4; extra == "tests"
+Requires-Dist: pytest-asyncio~=0.20; extra == "tests"
+Requires-Dist: pytest-cov~=4.0; extra == "tests"
 
 # Declearn: a modular and extensible framework for Federated Learning
 
 - [Introduction](#introduction)
 - [Setup](#setup)
 - [Quickstart](#quickstart)
 - [Usage of the Python API](#usage-of-the-python-api)
```

### Comparing `declearn-2.3.2/README.md` & `declearn-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/__init__.py` & `declearn-2.4.0/declearn/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,33 +36,39 @@
     Client-Server network communications API and implementations.
 * [data_info][declearn.data_info]:
     Tools to write and extend shareable metadata fields specifications.
 * [dataset][declearn.dataset]:
     Data interfacing API and implementations.
 * [main][declearn.main]:
     Main classes implementing a Federated Learning process.
+* [messaging][declearn.messaging]:
+    API and default classes to define parsable messages for applications.
 * [metrics][declearn.metrics]:
     Iterative and federative evaluation metrics computation tools.
 * [model][declearn.model]:
     Model interfacing API and implementations.
 * [optimizer][declearn.optimizer]:
     Framework-agnostic optimizer and algorithmic plug-ins API and tools.
 * [typing][declearn.typing]:
     Type hinting utils, defined and exposed for code readability purposes.
 * [utils][declearn.utils]:
     Shared utils used (extensively) across all of declearn.
+* [version][declearn.version]:
+    DecLearn version information, as hard-coded constants.
 """
 
 from . import (
     aggregator,
     communication,
     data_info,
     dataset,
     main,
     metrics,
+    messaging,
     model,
     optimizer,
     typing,
     utils,
+    version,
 )
 
-__version__ = "2.3.2"
+__version__ = version.VERSION
```

### Comparing `declearn-2.3.2/declearn/aggregator/__init__.py` & `declearn-2.4.0/declearn/aggregator/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,23 +26,25 @@
 This declearn submodule provides with:
 
 API tools
 ---------
 
 * [Aggregator][declearn.aggregator.Aggregator]:
     Abstract base class defining an API for Vector aggregation.
+* [ModelUpdates][declearn.aggregator.ModelUpdates]:
+    Base dataclass for model updates' sharing and aggregation.
 * [list_aggregators][declearn.aggregator.list_aggregators]:
     Return a mapping of registered Aggregator subclasses.
 
 
 Concrete classes
 ----------------
 
 * [AveragingAggregator][declearn.aggregator.AveragingAggregator]:
     Average-based-aggregation Aggregator subclass.
 * [GradientMaskedAveraging][declearn.aggregator.GradientMaskedAveraging]:
     Gradient Masked Averaging Aggregator subclass.
 """
 
-from ._api import Aggregator, list_aggregators
-from ._base import AveragingAggregator
+from ._api import Aggregator, ModelUpdates, list_aggregators
+from ._avg import AveragingAggregator
 from ._gma import GradientMaskedAveraging
```

### Comparing `declearn-2.3.2/declearn/aggregator/_api.py` & `declearn-2.4.0/declearn/aggregator/_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,98 +13,188 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Model updates aggregation API."""
 
-from abc import ABCMeta, abstractmethod
-from typing import Any, ClassVar, Dict, Type, TypeVar
+import abc
+import dataclasses
+import warnings
+from typing import Any, ClassVar, Dict, Generic, Type, TypeVar, Union
 
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.model.api import Vector
 from declearn.utils import (
+    Aggregate,
     access_types_mapping,
     create_types_registry,
     register_type,
 )
 
 __all__ = [
     "Aggregator",
+    "ModelUpdates",
 ]
 
 
 T = TypeVar("T")
 
 
+@dataclasses.dataclass
+class ModelUpdates(Aggregate, base_cls=True, register=True):
+    """Base dataclass for model updates' sharing and aggregation.
+
+    Each and every `Aggregator` subclass is expected to be coupled with
+    one (or multiple) `ModelUpdates` (sub)type(s), that define which data
+    is exchanged and how it is aggregated across a network of peers. An
+    instance resulting from the aggregation of multiple peers' data may
+    be passed to an appropriate `Aggregator` instance for finalization
+    into a `Vector` of model updates.
+
+    This class also defines whether contents are compatible with secure
+    aggregation, and whether some fields should remain in cleartext no
+    matter what.
+
+    Note that subclasses are automatically type-registered, and should be
+    decorated as `dataclasses.dataclass`. To prevent registration, simply
+    pass `register=False` at inheritance.
+    """
+
+    updates: Vector
+    weights: Union[int, float]
+
+    _group_key = "ModelUpdates"
+
+
+ModelUpdatesT = TypeVar("ModelUpdatesT", bound=ModelUpdates)
+
+
 @create_types_registry
-class Aggregator(metaclass=ABCMeta):
-    """Abstract class defining an API for Vector aggregation.
+class Aggregator(Generic[ModelUpdatesT], metaclass=abc.ABCMeta):
+    """Abstract class defining an API for model updates aggregation.
 
     The aim of this abstraction (which itself operates on the Vector
     abstraction, so as to provide framework-agnostic algorithms) is
     to enable implementing arbitrary aggregation rules to turn local
-    model updates into global updates in a federated learning context.
+    model updates into global updates in a federated or decentralized
+    learning context.
 
-    An Aggregator is typically meant to be used on a round-wise basis
-    by the orchestrating server of a centralized federated learning
-    process, to aggregate the client-wise model updated into a Vector
-    that may then be used as "gradients" by the server's Optimizer to
-    update the global model.
+    An Aggregator has three main purposes:
+
+    - Preparing and packaging data that is to be shared with peers
+      based on local model updates into a `ModelUpdates` container
+      that implements aggregation, usually via summation.
+    - Finalizing such a data container into model updates.
 
     Abstract
     --------
-    The following attribute and method require to be overridden
+    The following class attributes and methods must be implemented
     by any non-abstract child class of `Aggregator`:
 
     - name: str class attribute
-        Name identifier of the class (should be unique across existing
-        Aggregator classes). Also used for automatic types-registration
-        of the class (see `Inheritance` section below).
-    - aggregate(updates: Dict[str, Vector], n_steps: Dict[str, int]) -> Vector:
-        Aggregate input vectors into a single one.
-        This is the main method for any `Aggregator`.
+        Name identifier of the class (should be unique across Aggregator
+        classes). Also used for automatic type-registration of the class
+        (see `Inheritance` section below).
+    - prepare_for_sharing(updates: Vector, n_steps: int) -> ModelUpdates:
+        Pre-process and package local model updates for aggregation.
+    - finalize_updates(updates: ModelUpdates):
+        Finalize pre-aggregated data into global model updates.
 
     Overridable
     -----------
+    - updates_cls: type[ModelUpdates] class attribute
+        Type of 'ModelUpdates' data structure used by this Aggregator class.
     - get_config() -> Dict[str, Any]:
         Return a JSON-serializable configuration dict of an instance.
     - from_config(Dict[str, Any]) -> Aggregator:
         Classmethod to instantiate an Aggregator from a config dict.
 
     Inheritance
     -----------
     When a subclass inheriting from `Aggregator` is declared, it is
     automatically registered under the "Aggregator" group using its
     class-attribute `name`. This can be prevented by adding `register=False`
     to the inheritance specs (e.g. `class MyCls(Aggregator, register=False)`).
     See `declearn.utils.register_type` for details on types registration.
     """
 
-    name: ClassVar[str] = NotImplemented
+    name: ClassVar[str]
     """Name identifier of the class, unique across Aggregator classes."""
 
+    updates_cls: ClassVar[Type[ModelUpdates]] = ModelUpdates
+    """Type of 'ModelUpdates' data structure used by this Aggregator class."""
+
     def __init_subclass__(
         cls,
         register: bool = True,
         **kwargs: Any,
     ) -> None:
         """Automatically type-register Aggregator subclasses."""
         super().__init_subclass__(**kwargs)
         if register:
             register_type(cls, cls.name, group="Aggregator")
 
-    @abstractmethod
+    @abc.abstractmethod
+    def prepare_for_sharing(
+        self,
+        updates: Vector,
+        n_steps: int,  # revise: generalize kwargs?
+    ) -> ModelUpdatesT:
+        """Pre-process and package local model updates for aggregation.
+
+        Parameters
+        ----------
+        updates:
+            Local model updates, as a Vector value.
+        n_steps:
+            Number of local training steps taken to produce `updates`.
+
+        Returns
+        -------
+        updates:
+            Data to be shared with peers, wrapped into a `ModelUpdates`
+            (subclass) instance.
+        """
+
+    @abc.abstractmethod
+    def finalize_updates(
+        self,
+        updates: ModelUpdatesT,
+    ) -> Vector:
+        """Finalize pre-aggregated data into global model updates.
+
+        Parameters
+        ----------
+        updates:
+            `ModelUpdates` instance holding aggregated data to finalize,
+            resulting from peers' shared instances' sum-aggregation.
+        """
+
+    def get_config(
+        self,
+    ) -> Dict[str, Any]:
+        """Return a JSON-serializable dict with this object's parameters."""
+        return {}  # pragma: no cover
+
+    @classmethod
+    def from_config(
+        cls,
+        config: Dict[str, Any],
+    ) -> Self:
+        """Instantiate an Aggregator from its configuration dict."""
+        return cls(**config)
+
     def aggregate(
         self,
         updates: Dict[str, Vector[T]],
         n_steps: Dict[str, int],  # revise: abstract~generalize kwargs use
     ) -> Vector[T]:
-        """Aggregate input vectors into a single one.
+        """DEPRECATED - Aggregate input vectors into a single one.
 
         Parameters
         ----------
         updates: dict[str, Vector]
             Client-wise updates, as a dictionary with clients' names as
             string keys and updates as Vector values.
         n_steps: dict[str, int]
@@ -118,28 +208,28 @@
             the server-side optimizer.
 
         Raises
         ------
         TypeError
             If the input `updates` are an empty dict.
         """
-
-    def get_config(
-        self,
-    ) -> Dict[str, Any]:
-        """Return a JSON-serializable dict with this object's parameters."""
-        return {}  # pragma: no cover
-
-    @classmethod
-    def from_config(
-        cls,
-        config: Dict[str, Any],
-    ) -> Self:
-        """Instantiate an Aggregator from its configuration dict."""
-        return cls(**config)
+        warnings.warn(
+            "'Aggregator.aggregate' was deprecated in DecLearn v2.4 in favor "
+            "of new API methods. It will be removed in DecLearn v2.6 and/or "
+            "v3.0.",
+            DeprecationWarning,
+        )
+        if not updates:
+            raise TypeError("'Aggregator.aggregate' received an empty dict.")
+        partials = [
+            self.prepare_for_sharing(updates[client], n_steps[client])
+            for client in updates
+        ]
+        aggregated = sum(partials[1:], start=partials[0])
+        return self.finalize_updates(aggregated)
 
 
 def list_aggregators() -> Dict[str, Type[Aggregator]]:
     """Return a mapping of registered Aggregator subclasses.
 
     This function aims at making it easy for end-users to list and access
     all available Aggregator classes at any given time. The returned dict
```

### Comparing `declearn-2.3.2/declearn/communication/__init__.py` & `declearn-2.4.0/declearn/communication/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,47 +21,51 @@
 endpoints for federated learning processes, as well as suitable messages to
 be transmitted, and the available communication protocols.
 
 This module contains the following core submodules:
 
 * [api][declearn.communication.api]:
     Base API to define client- and server-side communication endpoints.
-* [messaging][declearn.communication.messaging]:
-    Message dataclasses defining information containers to be exchanged
-    between communication endpoints.
+* [utils][declearn.communication.utils]:
+    Utils related to network communication endpoints' setup and usage.
 
-It also exposes the following core utility functions and dataclasses:
+
+It re-exports publicly from `utils` the following elements:
 
 * [build_client][declearn.communication.build_client]:
     Instantiate a NetworkClient, selecting its subclass based on protocol name.
 * [build_server][declearn.communication.build_server]:
     Instantiate a NetworkServer, selecting its subclass based on protocol name.
 * [list_available_protocols][declearn.communication.list_available_protocols]:
     List the protocol names for which both a NetworkClient and NetworkServer
     classes are registered (hence available to `build_client`/`build_server`).
 * [NetworkClientConfig][declearn.communication.NetworkClientConfig]:
     TOML-parsable dataclass for network clients' instantiation.
 * [NetworkServerConfig][declearn.communication.NetworkServerConfig]:
     TOML-parsable dataclass for network servers' instantiation.
 
-
 Finally, it defines the following protocol-specific submodules, provided
 the associated third-party dependencies are available:
 
 * [grpc][declearn.communication.grpc]:
     gRPC-based network communication endpoints.
     Requires the `grpcio` and `protobuf` third-party packages.
 * [websockets][declearn.communication.websockets]:
     WebSockets-based network communication endpoints.
     Requires the `websockets` third-party package.
+
+Additionnally, for retro-compatibility purposes, it exports the DEPRECATED
+[messaging][declearn.communication.messaging] submodule, that should no
+longer be used, as its contents were re-dispatched elsewhere in DecLearn.
 """
 
-# Messaging and Communications API and base tools:
-from . import api, messaging
-from ._build import (
+# Messaging API and base tools:
+from . import api
+from . import utils
+from .utils import (
     _INSTALLABLE_BACKENDS,
     NetworkClientConfig,
     NetworkServerConfig,
     build_client,
     build_server,
     list_available_protocols,
 )
@@ -71,7 +75,10 @@
     from . import grpc
 except ImportError:  # pragma: no cover
     _INSTALLABLE_BACKENDS["grpc"] = ("grpcio", "protobuf")
 try:
     from . import websockets
 except ImportError:  # pragma: no cover
     _INSTALLABLE_BACKENDS["websockets"] = ("websockets",)
+
+# DEPRECATED submodule, kept for retro-compatibility until 2.6 and/or 3.0.
+from . import messaging
```

### Comparing `declearn-2.3.2/declearn/communication/_build.py` & `declearn-2.4.0/declearn/communication/utils/_build.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,24 +98,31 @@
     except KeyError as exc:  # pragma: no cover
         raise_if_installable(protocol, exc)
         raise KeyError(
             "Failed to retrieve NetworkClient "
             f"class for protocol '{protocol}'."
         ) from exc
     assert issubclass(cls, NetworkClient)  # guaranteed by TypesRegistry
-    return cls(server_uri, name, certificate, logger, **kwargs)
+    return cls(
+        server_uri=server_uri,
+        name=name,
+        certificate=certificate,
+        logger=logger,
+        **kwargs,
+    )
 
 
 def build_server(
     protocol: str,
     host: str,
     port: int,
     certificate: Optional[str] = None,
     private_key: Optional[str] = None,
     password: Optional[str] = None,
+    heartbeat: float = 1.0,
     logger: Union[logging.Logger, str, None] = None,
     **kwargs: Any,
 ) -> NetworkServer:
     """Set up and return a NetworkServer communication endpoint.
 
     Parameters
     ----------
@@ -133,14 +140,17 @@
     private_key: str or None, default=None
         Path to the server private key to use SSL/TLS communications
         encryption. If provided, `certificate` must be set as well.
     password: str or None, default=None
         Optional password used to access `private_key`, or path to a
         file from which to read such a password.
         If None but a password is needed, an input will be prompted.
+    heartbeat: float, default=1.0
+        Delay (in seconds) between verifications when checking for a
+        message having beend received from or collected by a client.
     logger: logging.Logger or str or None, default=None,
         Logger to use, or name of a logger to set up with
         `declearn.utils.get_logger`. If None, use `type(server)`.
     **kwargs:
         Any valid additional keyword parameter may be passed as well.
         Refer to the target `NetworkServer` subclass for details.
 
@@ -157,15 +167,22 @@
         raise_if_installable(protocol, exc)
         raise KeyError(
             "Failed to retrieve NetworkServer "
             f"class for protocol '{protocol}'."
         ) from exc
     assert issubclass(cls, NetworkServer)  # guaranteed by TypesRegistry
     return cls(
-        host, port, certificate, private_key, password, logger, **kwargs
+        host=host,
+        port=port,
+        certificate=certificate,
+        private_key=private_key,
+        password=password,
+        heartbeat=heartbeat,
+        logger=logger,
+        **kwargs,
     )
 
 
 BuildClientConfig = dataclass_from_func(build_client)
 
 
 BuildServerConfig = dataclass_from_func(build_server)
```

### Comparing `declearn-2.3.2/declearn/communication/api/__init__.py` & `declearn-2.4.0/declearn/communication/api/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/communication/api/_client.py` & `declearn-2.4.0/declearn/communication/api/_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,36 +13,46 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Abstract class defining an API for client-side communication endpoints."""
 
+import abc
+import asyncio
 import logging
 import types
-from abc import ABCMeta, abstractmethod
+import warnings
 from typing import Any, ClassVar, Dict, Optional, Type, Union
 
-from declearn.communication.messaging import (
-    Empty,
-    Error,
-    GetMessageRequest,
-    JoinReply,
-    JoinRequest,
-    Message,
+from typing_extensions import Self  # future: import from typing (py >=3.11)
+
+from declearn.communication.api.backend import flags
+from declearn.communication.api.backend.actions import (
+    Accept,
+    ActionMessage,
+    # Drop,  # FUTURE: implement a method to drop politely
+    Join,
+    Ping,
+    Recv,
+    Reject,
+    Send,
+    parse_action_from_string,
 )
+from declearn.messaging import Message, SerializedMessage
 from declearn.utils import create_types_registry, get_logger, register_type
+from declearn.version import VERSION
 
 __all__ = [
     "NetworkClient",
 ]
 
 
 @create_types_registry
-class NetworkClient(metaclass=ABCMeta):
+class NetworkClient(metaclass=abc.ABCMeta):
     """Abstract class defining an API for client-side communication endpoints.
 
     This class defines the key methods used to communicate between a
     client and the orchestrating server during a federated learning
     process, agnostic to the actual communication protocol in use.
 
     Instantiating a `NetworkClient` does not trigger a connection to
@@ -50,25 +60,25 @@
     `NetworkClient` object, its `start` method must first be awaited
     and conversely, its `stop` method should be awaited to close the
     connection:
     ```
     >>> client = ClientSubclass("example.domain.com:8765", "name", "cert_path")
     >>> await client.start()
     >>> try:
-    >>>     client.register(data_info)
+    >>>     client.register()
     >>>     ...
     >>> finally:
     >>>     await client.stop()
     ```
 
     An alternative syntax to achieve the former is using the client
     object as an asynchronous context manager:
     ```
     >>> async with ClientSubclass(...) as client:
-    >>>     client.register(data_info)
+    >>>     client.register()
     >>>     ...
     ```
 
     Note that a declearn `NetworkServer` manages an allow-list of
     clients, which is defined during a registration phase of limited
     time, based on requests emitted through the `NetworkClient.register`
     method. Any message emitted using `NetworkClient.send_message` will
@@ -84,15 +94,14 @@
         **kwargs: Any,
     ) -> None:
         """Automate the type-registration of NetworkClient subclasses."""
         super().__init_subclass__(**kwargs)
         if register:
             register_type(cls, cls.protocol, group="NetworkClient")
 
-    @abstractmethod
     def __init__(
         self,
         server_uri: str,
         name: str,
         certificate: Optional[str] = None,
         logger: Union[logging.Logger, str, None] = None,
     ) -> None:
@@ -108,173 +117,242 @@
         certificate: str or None, default=None,
             Path to a certificate (publickey) PEM file, to use SSL/TLS
             communcations encryption.
         logger: logging.Logger or str or None, default=None,
             Logger to use, or name of a logger to set up using
             `declearn.utils.get_logger`. If None, use `type(self)-name`.
         """
-        # Assign basic attributes. Note: children must handle 'certificate'.
         self.server_uri = server_uri
         self.name = name
         self._ssl = self._setup_ssl_context(certificate)
         if isinstance(logger, logging.Logger):
             self.logger = logger
         else:
             self.logger = get_logger(logger or f"{type(self).__name__}-{name}")
 
     @staticmethod
-    @abstractmethod
+    @abc.abstractmethod
     def _setup_ssl_context(
         certificate: Optional[str] = None,
     ) -> Any:
         """Set up and return an (optional) SSL context object.
 
         The return type is communication-protocol dependent.
         """
 
     # similar to NetworkServer API; pylint: disable=duplicate-code
 
-    @abstractmethod
-    async def start(self) -> None:
+    @abc.abstractmethod
+    async def start(
+        self,
+    ) -> None:
         """Start the client, i.e. connect to the server.
 
         Note: this method can be called safely even if the
         client is already running (simply having no effect).
         """
 
-    @abstractmethod
-    async def stop(self) -> None:
+    @abc.abstractmethod
+    async def stop(
+        self,
+    ) -> None:
         """Stop the client, i.e. close all connections.
 
         Note: this method can be called safely even if the
         client is not running (simply having no effect).
         """
 
     async def __aenter__(
         self,
-    ) -> "NetworkClient":
+    ) -> Self:
         await self.start()
         return self
 
     async def __aexit__(
         self,
         exc_type: Type[Exception],
         exc_value: Exception,
         exc_tb: types.TracebackType,
     ) -> None:
         await self.stop()
 
     # pylint: enable=duplicate-code
 
+    @abc.abstractmethod
+    async def _send_message(
+        self,
+        message: str,
+    ) -> str:
+        """Send a message to the server and return the obtained reply.
+
+        This method should be defined by concrete NetworkClient child
+        classes, and implement communication-protocol-specific code
+        to send a message to the server and await the primary reply
+        from the `MessagesHandler` used by the server.
+        """
+
+    async def _exchange_action_messages(
+        self,
+        message: ActionMessage,
+    ) -> ActionMessage:
+        """Send an `ActionMessage` to the server and await its response."""
+        query = message.to_string()
+        reply = await self._send_message(query)
+        try:
+            return parse_action_from_string(reply)
+        except Exception as exc:
+            error = "Failed to decode a reply from the server."
+            self.logger.critical(error)
+            raise RuntimeError(error) from exc
+
     async def register(
         self,
-        data_info: Dict[str, Any],
+        data_info: Optional[Dict[str, Any]] = None,
     ) -> bool:
-        """Request the server to join a federating learning session.
-
-        Parameters
-        ----------
-        data_info : dict[str, any]
-            JSON-serializable dictionary holding information on the local
-            data that the server will use to set up the training model.
+        """Register to the server as a client.
 
         Returns
         -------
         accepted: bool
-            Whether the registration request was accepted by the server
-            or not.
+            Whether the registration request was accepted by the server.
 
         Raises
         -------
         TypeError
-            If the server does not return a JoinReply message.
+            If the server does not return a valid message.
+            This is a failsafe and should never happen.
         """
-        reply = await self._send_message(JoinRequest(self.name, data_info))
-        # Case when a JoinReply was received.
-        if isinstance(reply, JoinReply):
-            self.logger.info(
-                "Registration was %saccepted: '%s'",
-                "" if reply.accept else "not ",
-                reply.flag,
-            )
-            return reply.accept
-        # Case when an Error was received.
-        if isinstance(reply, Error):
-            self.logger.error(
-                "Registration request triggered an error:\n%s", reply.message
+        if data_info:
+            warnings.warn(
+                "Sending dataset information is no longer part of the client "
+                "registration process. The argument was ignored, and will be "
+                "removed in DecLearn version 2.4 and/or 3.0.",
+                DeprecationWarning,
             )
+        query = Join(name=self.name, version=VERSION)
+        reply = await self._exchange_action_messages(query)
+        # Case when registration was accepted.
+        if isinstance(reply, Accept):
+            self.logger.info("Registration was accepted: '%s'", reply.flag)
+            return True
+        # Case when registration was rejected.
+        if isinstance(reply, Reject):
+            self.logger.error("Registration was rejected: '%s'", reply.flag)
             return False
         # Otherwise, raise.
-        raise TypeError(
-            "Received an undue message type in response to JoinRequest."
+        error = (
+            "Received an undue response type when attempting to register "
+            f"with the server: '{type(reply)}'."
         )
-
-    @abstractmethod
-    async def _send_message(
-        self,
-        message: Message,
-    ) -> Message:
-        """Send a message to the server and return the obtained reply.
-
-        This method should be defined by concrete NetworkClient child
-        classes, and implement communication-protocol-specific code
-        to send a Message (of any kind) to the server and await the
-        primary reply from the `MessagesHandler` used by the server.
-        """
+        self.logger.critical(error)
+        raise TypeError(error)
 
     async def send_message(
         self,
         message: Message,
     ) -> None:
         """Send a message to the server.
 
         Parameters
         ----------
-        message: Message
+        message: str
             Message instance that is to be delivered to the server.
 
         Raises
         ------
         RuntimeError
-            If the server emits an Error message in response to the
-            message sent.
+            If the server rejects the sent message.
         TypeError
-            If the server returns a non-Empty message.
+            If the server returns neither a ping-back nor rejection message.
+            This is a failsafe and should never happen.
 
         Note
         ----
         The message sent here is designed to be received using the
         `NetworkServer.wait_for_messages` method.
         """
-        reply = await self._send_message(message)
-        if isinstance(reply, Empty):
+        query = Send(message.to_string())
+        reply = await self._exchange_action_messages(query)
+        if isinstance(reply, Ping):
             return None
-        if isinstance(reply, Error):
-            raise RuntimeError(
-                f"Message was rejected with error: {reply.message}"
-            )
-        raise TypeError(
-            "Received an undue message type in response to the posted message."
+        if isinstance(reply, Reject):
+            error = f"Message was rejected: {reply.flag}"
+            self.logger.error(error)
+            raise RuntimeError(error)
+        error = (
+            "Received an undue response type when attempting to send a "
+            f"message: '{type(reply)}'."
         )
+        self.logger.critical(error)
+        raise TypeError(error)
 
-    async def check_message(self, timeout: Optional[int] = None) -> Message:
-        """Retrieve the next message sent by the server.
+    async def recv_message(
+        self,
+        timeout: Optional[float] = None,
+    ) -> SerializedMessage:
+        """Await a message from the server, with optional timeout.
 
         Parameters
         ----------
-        timeout: int or None, default=None
-            Optional timeout delay, after which the server will send an
-            Error message with `messaging.flags.CHECK_MESSAGE_TIMEOUT`
-            if no other message awaits collection by this client.
+        timeout: float or None, default=None
+            Optional timeout delay, after which the server will send
+            a timeout notification to this client if no message is
+            available for it.
 
         Returns
         -------
-        message: Message
-            Message received from the server.
+        message: SerializedMessage
+            Serialized message received from the server.
 
         Note
         ----
         The message received here is expected to have been sent
         using one of the following `NetorkServer` methods:
         `send_message`, `send_messages`, or `broadcast_message`.
+
+        Raises
+        ------
+        asyncio.TimeoutError
+            If no message is available after the `timeout` delay.
+        RuntimeError
+            If the request is rejected by the server.
+        TypeError
+            If the server returns data of unproper type.
+            This is a failsafe and should never happen.
+        """
+        # Send a query, get a reply and return its content when possible.
+        query = Recv(timeout)
+        reply = await self._exchange_action_messages(query)
+        if isinstance(reply, Send):
+            return SerializedMessage.from_message_string(reply.content)
+        # Handle the various kinds of failures and raise accordingly.
+        if isinstance(reply, Reject):
+            if reply.flag == flags.CHECK_MESSAGE_TIMEOUT:
+                error = "Message-retrieval request timed out."
+                self.logger.error(error)
+                raise asyncio.TimeoutError(error)
+            error = f"Message-retrieval request was rejected: '{reply.flag}'."
+            self.logger.error(error)
+            raise RuntimeError(error)
+        error = (
+            "Received an undue response type when attempting to receive a "
+            f"message: '{type(reply)}'."
+        )
+        self.logger.critical(error)
+        raise TypeError(error)
+
+    async def check_message(
+        self,
+        timeout: Optional[float] = None,
+    ) -> SerializedMessage:
+        """Await a message from the server, with optional timeout.
+
+        This method is DEPRECATED in favor of the `recv_message` one.
+        It acts as an alias and will be removed in v2.6 and/or v3.0.
         """
-        return await self._send_message(GetMessageRequest(timeout))
+        warnings.warn(
+            "'NetworkServer.check_message' was renamed as 'recv_message' "
+            "in DecLearn 2.4. It now acts as an alias, but will be removed "
+            "in version 2.6 and/or 3.0.",
+            DeprecationWarning,
+        )
+        return await self.recv_message(timeout)
```

### Comparing `declearn-2.3.2/declearn/communication/api/_server.py` & `declearn-2.4.0/declearn/communication/api/_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,33 +13,37 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Abstract class defining an API for server-side communication endpoints."""
 
+import abc
 import asyncio
 import logging
 import types
-from abc import ABCMeta, abstractmethod
-from typing import Any, Dict, Optional, Set, Type, Union, ClassVar
+from typing import (
+    # fmt: off
+    Any, ClassVar, Dict, List, Mapping, Optional, Set, Type, Tuple, Union
+)
 
+from typing_extensions import Self  # future: import from typing (py >=3.11)
 
-from declearn.communication.api._service import MessagesHandler
-from declearn.communication.messaging import Message
+from declearn.communication.api.backend import MessagesHandler
+from declearn.messaging import Message, SerializedMessage
 from declearn.utils import create_types_registry, get_logger, register_type
 
 
 __all__ = [
     "NetworkServer",
 ]
 
 
 @create_types_registry
-class NetworkServer(metaclass=ABCMeta):
+class NetworkServer(metaclass=abc.ABCMeta):
     """Abstract class defining an API for server-side communication endpoints.
 
     This class defines the key methods used to communicate between
     a server and its clients during a federated learning process,
     agnostic to the actual communication protocol in use.
 
     Instantiating a `NetworkServer` does not instantly serve the declearn
@@ -49,25 +53,25 @@
     should be awaited to close the connection:
     ```
     >>> server = ServerSubclass(
     ...     "example.domain.com", 8765, "cert_path", "pkey_path"
     ... )
     >>> await server.start()
     >>> try:
-    >>>     data_info = server.wait_for_clients(...)
+    >>>     server.wait_for_clients(...)
     >>>     ...
     >>> finally:
     >>>     await server.stop()
     ```
 
     An alternative syntax to achieve the former is using the server
     object as an asynchronous context manager:
     ```
     >>> async with ServerSubclass(...) as server:
-    >>>     data_info = server.wait_for_clients(...)
+    >>>     server.wait_for_clients(...)
     >>>     ...
     ```
 
     Note that a `NetworkServer` manages an allow-list of clients,
     which is defined based on `NetworkClient.register(...)`-emitted
     requests during a registration phase restricted to the context
     of the awaitable `wait_for_clients` method.
@@ -82,22 +86,22 @@
         **kwargs: Any,
     ) -> None:
         """Automate the type-registration of NetworkServer subclasses."""
         super().__init_subclass__(**kwargs)
         if register:
             register_type(cls, cls.protocol, group="NetworkServer")
 
-    @abstractmethod
     def __init__(
         self,
         host: str,
         port: int,
         certificate: Optional[str] = None,
         private_key: Optional[str] = None,
         password: Optional[str] = None,
+        heartbeat: float = 1.0,
         logger: Union[logging.Logger, str, None] = None,
     ) -> None:
         """Instantiate the server-side communications handler.
 
         Parameters
         ----------
         host: str
@@ -111,30 +115,33 @@
         private_key: str or None, default=None
             Path to the server private key to use SSL/TLS communications
             encryption. If provided, `certificate` must be set as well.
         password: str or None, default=None
             Optional password used to access `private_key`, or path to a
             file from which to read such a password.
             If None but a password is needed, an input will be prompted.
+        heartbeat: float, default=1.0
+            Delay (in seconds) between verifications when checking for a
+            message having beend received from or collected by a client.
         logger: logging.Logger or str or None, default=None,
             Logger to use, or name of a logger to set up with
             `declearn.utils.get_logger`. If None, use `type(self)`.
         """
         # arguments serve modularity; pylint: disable=too-many-arguments
         self.host = host
         self.port = port
         self._ssl = self._setup_ssl(certificate, private_key, password)
         if isinstance(logger, logging.Logger):
             self.logger = logger
         else:
             self.logger = get_logger(logger or f"{type(self).__name__}")
-        self.handler = MessagesHandler(self.logger)
+        self.handler = MessagesHandler(logger=self.logger, heartbeat=heartbeat)
 
     @property
-    @abstractmethod
+    @abc.abstractmethod
     def uri(self) -> str:
         """URI on which this server is exposed, to be requested by clients."""
 
     @property
     def client_names(self) -> Set[str]:
         """Set of registered clients' names."""
         return self.handler.client_names
@@ -155,37 +162,37 @@
             raise ValueError(
                 "Both 'certificate' and 'private_key' are required "
                 "to set up SSL encryption."
             )
         return self._setup_ssl_context(certificate, private_key, password)
 
     @staticmethod
-    @abstractmethod
+    @abc.abstractmethod
     def _setup_ssl_context(
         certificate: str,
         private_key: str,
         password: Optional[str] = None,
     ) -> Any:
         """Set up and return a SSL context object suitable for this class."""
 
-    @abstractmethod
+    @abc.abstractmethod
     async def start(
         self,
     ) -> None:
         """Initialize the server and start welcoming communications."""
 
-    @abstractmethod
+    @abc.abstractmethod
     async def stop(
         self,
     ) -> None:
         """Stop the server and purge information about clients."""
 
     async def __aenter__(
         self,
-    ) -> "NetworkServer":
+    ) -> Self:
         await self.start()
         return self
 
     async def __aexit__(
         self,
         exc_type: Type[Exception],
         exc_value: Exception,
@@ -193,183 +200,184 @@
     ) -> None:
         await self.stop()
 
     async def wait_for_clients(
         self,
         min_clients: int = 1,
         max_clients: Optional[int] = None,
-        timeout: Optional[int] = None,
-    ) -> Dict[str, Dict[str, Any]]:
+        timeout: Optional[float] = None,
+    ) -> None:
         """Wait for clients to register for training, with given criteria.
 
         Parameters
         ----------
         min_clients: int, default=1
             Minimum number of clients required. Corrected to be >= 1.
             If `timeout` is None, used as the exact number of clients
             required - once reached, registration will be closed.
         max_clients: int or None, default=None
             Maximum number of clients authorized to register.
-        timeout: int or None, default=None
+        timeout: float or None, default=None
             Optional maximum waiting time (in seconds) beyond which
             to close registration and either return or raise.
 
         Raises
         ------
         RuntimeError
             If the number of registered clients does not abide by the
             provided boundaries at the end of the process.
-
-        Returns
-        -------
-        client_info: dict[str, dict[str, any]]
-            A dictionary where the keys are the participants
-            and the values are their information.
         """
-        return await self.handler.wait_for_clients(
-            min_clients, max_clients, timeout
-        )
+        await self.handler.wait_for_clients(min_clients, max_clients, timeout)
 
-    async def broadcast_message(
+    async def send_message(
         self,
         message: Message,
-        clients: Optional[Set[str]] = None,
-        heartbeat: int = 1,
-        timeout: Optional[int] = None,
+        client: str,
+        timeout: Optional[float] = None,
     ) -> None:
-        """Send a message to an ensemble of clients and await its collection.
+        """Send a message to a given client and wait for it to be collected.
 
         Parameters
         ----------
-        message: Message
+        message: str
             Message instance that is to be delivered to the client.
-        clients: set[str] or None, default=None
-            Optional subset of registered clients, messages from
-            whom to wait for. If None, set to `self.client_names`.
-        heartbeat: int, default=1
-            Delay (in seconds) between verifications that the message
-            has been collected by the client.
-        timeout: int or None, default=None
+        client: str
+            Identifier of the client to whom the message is addressed.
+        timeout: float or None, default=None
             Optional maximum delay (in seconds) beyond which to stop
             waiting for collection and raise an asyncio.TimeoutError.
 
         Raises
         ------
         asyncio.TimeoutError
             If `timeout` is set and is reached while the message is
-            yet to be collected by at least one of the clients.
+            yet to be collected by the client.
         """
-        if clients is None:
-            clients = self.client_names
-        messages = {client: message for client in clients}
-        await self.send_messages(messages, heartbeat, timeout)
+        await self.handler.send_message(message.to_string(), client, timeout)
 
     async def send_messages(
         self,
-        messages: Dict[str, Message],
-        heartbeat: int = 1,
-        timeout: Optional[int] = None,
+        messages: Mapping[str, Message],
+        timeout: Optional[float] = None,
     ) -> None:
-        """Send a message to an ensemble of clients and await its collection.
+        """Send messages to an ensemble of clients and await their collection.
 
         Parameters
         ----------
         messages: dict[str, Message]
-            Dict mapping Message instances that are to be delivered
-            to the names of their destinatory client.
-        heartbeat: int, default=1
-            Delay (in seconds) between verifications that the message
-            has been collected by the client.
-        timeout: int or None, default=None
+            Dict mapping client names to the messages addressed to them.
+        timeout: float or None, default=None
             Optional maximum delay (in seconds) beyond which to stop
             waiting for collection and raise an asyncio.TimeoutError.
 
         Raises
         ------
         asyncio.TimeoutError
             If `timeout` is set and is reached while the message is
             yet to be collected by at least one of the clients.
         """
         routines = [
-            self.send_message(message, client, heartbeat, timeout)
+            self.send_message(message, client, timeout)
             for client, message in messages.items()
         ]
-        results = await asyncio.gather(*routines, return_exceptions=True)
-        for result in results:
-            if isinstance(result, Exception):
-                raise result
+        await asyncio.gather(*routines, return_exceptions=False)
 
-    async def send_message(
+    async def broadcast_message(
         self,
         message: Message,
-        client: str,
-        heartbeat: int = 1,
-        timeout: Optional[int] = None,
+        clients: Optional[Set[str]] = None,
+        timeout: Optional[float] = None,
     ) -> None:
-        """Send a message to a given client and wait for it to be collected.
+        """Send a message to an ensemble of clients and await its collection.
 
         Parameters
         ----------
-        message: Message
-            Message instance that is to be delivered to the client.
-        client: str
-            Identifier of the client to whom the message is addressed.
-        heartbeat: int, default=1
-            Delay (in seconds) between verifications that the message
-            has been collected by the client.
-        timeout: int or None, default=None
+        message: str
+            Message instance that is to be delivered to the clients.
+        clients: set[str] or None, default=None
+            Optional subset of registered clients, messages from
+            whom to wait for. If None, set to `self.client_names`.
+        timeout: float or None, default=None
             Optional maximum delay (in seconds) beyond which to stop
             waiting for collection and raise an asyncio.TimeoutError.
 
         Raises
         ------
         asyncio.TimeoutError
             If `timeout` is set and is reached while the message is
-            yet to be collected by the client.
+            yet to be collected by at least one of the clients.
         """
-        await self.handler.send_message(message, client, heartbeat, timeout)
+        if clients is None:
+            clients = self.client_names
+        messages = {client: message for client in clients}
+        await self.send_messages(messages, timeout)
 
     async def wait_for_messages(
         self,
         clients: Optional[Set[str]] = None,
-        heartbeat: int = 1,
-        timeout: Optional[int] = None,
-    ) -> Dict[str, Message]:
-        """Wait for an ensemble of clients to have sent a message.
+    ) -> Dict[str, SerializedMessage]:
+        """Wait for messages from (a subset of) all clients.
 
         Parameters
         ----------
         clients: set[str] or None, default=None
             Optional subset of registered clients, messages from
             whom to wait for. If None, set to `self.client_names`.
-        heartbeat: int, default=1
-            Delay (in seconds) between verifications that a client
-            has sent their message.
-        timeout: int or None, default=None
-            Optional maximum delay (in seconds) beyond which to stop
-            waiting for messages and raise an asyncio.TimeoutError.
 
-        Raises
-        ------
-        asyncio.TimeoutError
-            If any of the clients has failed to deliver a message
-            before `timeout` was reached.
+        Returns
+        -------
+        messages:
+            A dictionary mapping clients' names to the serialized
+            messages they sent to the server.
+        """
+        if clients is None:
+            clients = self.client_names
+        routines = [self.handler.recv_message(client) for client in clients]
+        received = await asyncio.gather(*routines, return_exceptions=False)
+        return {
+            client: SerializedMessage.from_message_string(string)
+            for client, string in zip(clients, received)
+        }
+
+    async def wait_for_messages_with_timeout(
+        self,
+        timeout: float,
+        clients: Optional[Set[str]] = None,
+    ) -> Tuple[Dict[str, SerializedMessage], List[str]]:
+        """Wait for an ensemble of clients to have sent a message.
+
+        Parameters
+        ----------
+        timeout: float or None, default=None
+            Maximum waiting delay (in seconds) before returning
+            received messages, even if some are missing.
+        clients: set[str] or None, default=None
+            Optional subset of registered clients, messages from
+            whom to wait for. If None, set to `self.client_names`.
 
         Returns
         -------
         messages: dict[str, Message]
             A dictionary where the keys are the clients' names and
             the values are Message objects they sent to the server.
+        timeouts: list[str]
+            List of names of clients that failed to send a message
+            prior to `timeout` being reached.
         """
         if clients is None:
             clients = self.client_names
         routines = [
-            self.handler.recv_message(client, heartbeat, timeout)
-            for client in clients
+            self.handler.recv_message(client, timeout) for client in clients
         ]
         received = await asyncio.gather(*routines, return_exceptions=True)
-        messages = {}  # type: Dict[str, Message]
-        for client, message in zip(clients, received):
-            if isinstance(message, Exception):
-                raise message
-            messages[client] = message
-        return messages
+        messages = {}  # type: Dict[str, SerializedMessage]
+        timeouts = []  # type: List[str]
+        for client, output in zip(clients, received):
+            if isinstance(output, asyncio.TimeoutError):
+                timeouts.append(client)
+            elif isinstance(output, BaseException):
+                raise output
+            else:
+                messages[client] = SerializedMessage.from_message_string(
+                    output
+                )
+        return messages, timeouts
```

### Comparing `declearn-2.3.2/declearn/communication/api/_service.py` & `declearn-2.4.0/declearn/communication/api/backend/_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,256 +15,291 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Protocol-agnostic server-side network messages handler."""
 
 import asyncio
 import logging
+import math
 from typing import Any, Dict, Optional, Set, Union
 
 
-from declearn.communication.messaging import (
-    Empty,
-    Error,
-    EvaluationReply,
-    GenericMessage,
-    GetMessageRequest,
-    JoinReply,
-    JoinRequest,
-    Message,
-    TrainReply,
-    flags,
-    parse_message_from_string,
+from declearn.communication.api.backend import flags
+from declearn.communication.api.backend.actions import (
+    Accept,
+    ActionMessage,
+    Drop,
+    Join,
+    LegacyMessageError,
+    LegacyReject,
+    Ping,
+    Recv,
+    Reject,
+    Send,
+    parse_action_from_string,
 )
-
-
-__all__ = [
-    "MessagesHandler",
-]
+from declearn.version import VERSION
 
 
 class MessagesHandler:
-    """Protocol-agnostic server-side network messages handler.
-
-    This class implements generic mechanisms to:
-    * manage an allow-list of registered clients
-    * parse incoming messages from string into Message instances
-    * handle messages based on their Message subclass, to either:
-      - process the registration request from a client
-      - make a message sent by the client available to the server
-      - return a message posted by the server to an asking client
-    * enable a managing server to:
-      - post messages for clients to collect
-      - collect messages sent by clients
-    """
+    """Minimal protocol-agnostic server-side messages handler."""
 
     def __init__(
         self,
         logger: logging.Logger,
+        heartbeat: float = 1.0,
     ) -> None:
+        # Assign parameters as attributes.
         self.logger = logger
+        self.heartbeat = heartbeat
+        # Set up containers for client identifiers and pending messages.
         self.registered_clients = {}  # type: Dict[Any, str]
-        self.data_info = {}  # type: Dict[str, Dict[str, Any]]
-        self.out_messages = {}  # type: Dict[str, Message]
-        self.inc_messages = {}  # type: Dict[str, Message]
-        # Declare attributes to be managed by the server class.
+        self.outgoing_messages = {}  # type: Dict[str, str]
+        self.incoming_messages = {}  # type: Dict[str, str]
+        # Mark client-registration as unopened.
         self.registration_status = flags.REGISTRATION_UNSTARTED
 
     @property
     def client_names(self) -> Set[str]:
         """Names of the registered clients."""
         return set(self.registered_clients.values())
 
     async def purge(
         self,
     ) -> None:
-        """Close opened connections and purge information about users."""
-        self.registered_clients = {}
-        self.data_info = {}
-        self.out_messages = {}
-        self.inc_messages = {}
+        """Close opened connections and purge information about users.
+
+        This resets the instance as though it was first initialized.
+        User registration will be marked as unstarted.
+        """
+        self.registered_clients.clear()
+        self.outgoing_messages.clear()
+        self.incoming_messages.clear()
+        self.registration_status = flags.REGISTRATION_UNSTARTED
 
     async def handle_message(
         self,
         string: str,
         context: Any,
-    ) -> Message:
+    ) -> ActionMessage:
         """Handle an incoming message from a client.
 
         Parameters
         ----------
         string: str
             Received message, as a string that can be parsed back
-            into a `declearn.communication.api.Message` instance.
+            into an `ActionMessage` instance.
         context: hashable
             Communications-protocol-specific hashable object that
             may be used to uniquely identify (and thereof contact)
             the client that sent the message being handled.
 
         Returns
         -------
-        message: Message
+        message: ActionMessage
             Message to return to the sender, the specific type of
             which depends on the type of incoming request, errors
             encountered, etc.
         """
-        # case-switch function; pylint: disable=too-many-return-statements
-        # Parse the incoming message. If it is incorrect, send back an error.
+        # Parse the incoming message. If it is incorrect, reject it.
         try:
-            message = parse_message_from_string(string)
-        except (KeyError, TypeError) as exc:
+            message = parse_action_from_string(string)
+        except (KeyError, TypeError, ValueError) as exc:
             self.logger.info(
-                "%s encountered while parsing received message: %s",
-                type(exc).__name__,
-                exc,
+                "Exception encountered while parsing received message: %s",
+                repr(exc),
             )
-            return Error(flags.INVALID_MESSAGE)
-        # Return a message-type-based response.
-        # Case: join request. Otherwise, reject messages from unknown clients.
-        if isinstance(message, JoinRequest):
+            return Reject(flags.INVALID_MESSAGE)
+        except LegacyMessageError as exc:
+            self.logger.info(repr(exc))
+            return LegacyReject()
+        # Case: join request from a (new) client. Handle it.
+        if isinstance(message, Join):
             return await self._handle_join_request(message, context)
+        # Case: unregistered client. Reject message.
         if context not in self.registered_clients:
-            return Error(flags.REJECT_UNREGISTERED)
-        # Case: ping request.
-        if isinstance(message, Empty):
-            return Empty()
-        # Case: request from client to collect a posted message.
-        if isinstance(message, GetMessageRequest):
+            return Reject(flags.REJECT_UNREGISTERED)
+        # Case: registered client. Handle it.
+        return await self._handle_registered_client_message(message, context)
+
+    async def _handle_registered_client_message(
+        self,
+        message: ActionMessage,
+        context: Any,
+    ) -> ActionMessage:
+        """Backend to handle a message from a registered client."""
+        # Case: message-receiving request. Handle it.
+        if isinstance(message, Recv):
             return await self._handle_recv_request(message, context)
-        # Case: expected type of message being sent to server.
-        acceptable = (Error, EvaluationReply, GenericMessage, TrainReply)
-        if isinstance(message, acceptable):
+        # Case: message-sending request. Handle it.
+        if isinstance(message, Send):
             return await self._handle_send_request(message, context)
-        # Otherwise, send back an error regarding incorrect message type.
+        # Case: drop message from a client. Handle it.
+        if isinstance(message, Drop):
+            return await self._handle_drop_request(message, context)
+        # Case: ping request. Ping back.
+        if isinstance(message, Ping):
+            return Ping()
+        # Case: unsupported message. Reject it.
         self.logger.error(
             "TypeError: received a message of unexpected type '%s'",
             type(message).__name__,
         )
-        return Error(flags.INVALID_MESSAGE)
+        return Reject(flags.INVALID_MESSAGE)
 
     async def _handle_join_request(
         self,
-        message: JoinRequest,
+        message: Join,
         context: Any,
-    ) -> JoinReply:
+    ) -> Union[Accept, Reject]:
         """Handle a join request."""
         # Case when client is already registered: warn but send OK.
         if context in self.registered_clients:
             self.logger.info(
                 "Client %s is already registered.",
                 self.registered_clients[context],
             )
-            reply = JoinReply(accept=True, flag=flags.REGISTERED_ALREADY)
+            return Accept(flags.REGISTERED_ALREADY)
         # Case when registration is not opened: warn and reject.
-        elif self.registration_status != flags.REGISTRATION_OPEN:
+        if self.registration_status != flags.REGISTRATION_OPEN:
             self.logger.info("Rejecting registration request.")
-            reply = JoinReply(accept=False, flag=self.registration_status)
+            return Reject(flag=self.registration_status)
+        # Case when the client uses an incompatible declearn version.
+        if (err := self._verify_version_compatibility(message)) is not None:
+            return err
         # Case when registration is opened: register the client.
-        else:
-            self._register_client(message, context)
-            reply = JoinReply(accept=True, flag=flags.REGISTERED_WELCOME)
-        # Return the selected reply.
-        return reply
+        self._register_client(message, context)
+        return Accept(flag=flags.REGISTERED_WELCOME)
+
+    def _verify_version_compatibility(
+        self,
+        message: Join,
+    ) -> Optional[Reject]:
+        """Return an 'Error' if a 'JoinRequest' is of incompatible version."""
+        if message.version.split(".")[:2] == VERSION.split(".")[:2]:
+            return None
+        self.logger.info(
+            "Received a registration request under name %s, that is "
+            "invalid due to the client using DecLearn '%s'.",
+            message.name,
+            message.version,
+        )
+        return Reject(flags.REJECT_INCOMPATIBLE_VERSION)
 
     def _register_client(
         self,
-        message: JoinRequest,
+        message: Join,
         context: Any,
     ) -> None:
-        """Register a user based on their JoinRequest and context object."""
+        """Register a user based on their Join request and context object."""
         # Alias the user name if needed to avoid duplication issues.
         name = message.name
         used = self.client_names
         if name in used:
             idx = sum(other.rsplit(".", 1)[0] == name for other in used)
             name = f"{name}.{idx}"
         # Register the user, recording context and received data information.
         self.logger.info("Registering client '%s' for training.", name)
         self.registered_clients[context] = name
-        self.data_info[name] = message.data_info
 
     async def _handle_send_request(
         self,
-        message: Message,
+        message: Send,
         context: Any,
-    ) -> Union[Empty, Error]:
+    ) -> Union[Ping, Reject]:
         """Handle a message-sending request (client-to-server)."""
         name = self.registered_clients[context]
         # Wait for any previous message from this client to be collected.
-        while self.inc_messages.get(name):  # revise: remove? add timeout?
-            await asyncio.sleep(1)
+        while self.incoming_messages.get(name):
+            await asyncio.sleep(self.heartbeat)
         # Record the received message, and return a ping-back response.
-        self.inc_messages[name] = message
-        return Empty()
+        self.incoming_messages[name] = message.content
+        return Ping()
 
     async def _handle_recv_request(
         self,
-        message: GetMessageRequest,
+        message: Recv,
         context: Any,
-    ) -> Message:
+    ) -> Union[Send, Reject]:
         """Handle a message-receiving request."""
         # Set up the optional timeout mechanism.
-        countdown = -1 if (message.timeout is None) else message.timeout
+        timeout = message.timeout
+        countdown = (
+            max(math.ceil(timeout / self.heartbeat), 1) if timeout else -1
+        )
         # Wait for a message to be available or timeout to be reached.
         name = self.registered_clients[context]
-        while (not self.out_messages.get(name)) and countdown:
-            await asyncio.sleep(1)
+        while (not self.outgoing_messages.get(name)) and countdown:
+            await asyncio.sleep(self.heartbeat)
             countdown -= 1
         # Either send back the collected message, or a timeout error.
         try:
-            reply = self.out_messages.pop(name)  # type: Message
+            content = self.outgoing_messages.pop(name)
         except KeyError:
-            reply = Error(flags.CHECK_MESSAGE_TIMEOUT)
-        return reply
+            return Reject(flags.CHECK_MESSAGE_TIMEOUT)
+        return Send(content)
+
+    async def _handle_drop_request(
+        self,
+        message: Drop,
+        context: Any,
+    ) -> Ping:
+        """Handle a drop request from a client."""
+        name = self.registered_clients.pop(context)
+        reason = (
+            f"reason: '{message.reason}'" if message.reason else "no reason"
+        )
+        self.logger.info("Client %s has dropped with %s.", name, reason)
+        return Ping()
 
-    def post_message(self, message: Message, client: str) -> None:
+    def post_message(
+        self,
+        message: str,
+        client: str,
+    ) -> None:
         """Post a message to be requested by a given client.
 
         Parameters
         ----------
-        message: Message
-            Message that is to be posted for the client to collect.
+        message: str
+            Message string that is to be posted for the client to collect.
         client: str
             Name of the client to whom the message is addressed.
 
         Notes
         -----
         This method merely makes the message available for the client
         to request, without any guarantee that it is received.
         See the `send_message` async method to wait for the posted
         message to have been requested by and thus sent to the client.
         """
         if client not in self.client_names:
             raise KeyError(f"Unkown destinatory client '{client}'.")
-        if client in self.out_messages:
+        if client in self.outgoing_messages:
             self.logger.warning(
                 "Overwriting pending message uncollected by client '%s'.",
                 client,
             )
-        self.out_messages[client] = message
+        self.outgoing_messages[client] = message
 
     async def send_message(
         self,
-        message: Message,
+        message: str,
         client: str,
-        heartbeat: int = 1,
-        timeout: Optional[int] = None,
+        timeout: Optional[float] = None,
     ) -> None:
         """Post a message for a client and wait for it to be collected.
 
         Parameters
         ----------
-        message: Message
-            Message that is to be posted for the client to collect.
+        message: str
+            Message string that is to be posted for the client to collect.
         client: str
             Name of the client to whom the message is addressed.
-        heartbeat: int, default=1
-            Delay (in seconds) between verifications that the message
-            has been collected by the client.
-        timeout: int or None, default=None
+        timeout: float or None, default=None
             Optional maximum delay (in seconds) beyond which to stop
             waiting for collection and raise an asyncio.TimeoutError.
 
         Raises
         ------
         asyncio.TimeoutError
             If `timeout` is set and is reached while the message is
@@ -273,168 +308,167 @@
         Notes
         -----
         See the `post_message` method to synchronously post a message
         and move on without guarantees that it was collected.
         """
         # Post the message. Wait for it to have been collected.
         self.post_message(message, client)
-        countdown = -1
-        if timeout is not None:
-            countdown = (timeout // heartbeat) + bool(timeout % heartbeat)
-        while self.out_messages.get(client, False) and countdown:
-            await asyncio.sleep(heartbeat)
+        countdown = (
+            max(math.ceil(timeout / self.heartbeat), 1) if timeout else -1
+        )
+        while self.outgoing_messages.get(client, False) and countdown:
+            await asyncio.sleep(self.heartbeat)
             countdown -= 1
         # If the message is still there, raise a TimeoutError.
-        if self.out_messages.get(client):
+        if self.outgoing_messages.get(client):
             raise asyncio.TimeoutError(
                 "Timeout reached before the sent message was collected."
             )
 
     def check_message(
         self,
         client: str,
-    ) -> Optional[Message]:
+    ) -> Optional[str]:
         """Check whether a message was received from a given client.
 
         Parameters
         ----------
         client: str
             Name of the client whose emitted message to check for.
 
         Returns
         -------
-        message: Message or None
+        message:
             Collected message that was sent by `client`, if any.
             In case no message is available, return None.
 
         Notes
         -----
         See the `recv_message` async method to wait for a message
         from the client to be available, collect and return it.
         """
         if client not in self.client_names:
             raise KeyError(f"Unregistered checked-for client '{client}'.")
-        return self.inc_messages.pop(client, None)
+        return self.incoming_messages.pop(client, None)
 
     async def recv_message(
         self,
         client: str,
-        heartbeat: int = 1,
-        timeout: Optional[int] = None,
-    ) -> Message:
+        timeout: Optional[float] = None,
+    ) -> str:
         """Wait for a message to be received from a given client.
 
         Parameters
         ----------
         client: str
             Name of the client whose emitted message to check for.
-        heartbeat: int, default=1
-            Delay (in seconds) between verifications that a message
-            has been received from the client.
-        timeout: int or None, default=None
+        timeout: float or None, default=None
             Optional maximum delay (in seconds) beyond which to stop
             waiting for a message and raise an asyncio.TimeoutError.
 
         Raises
         ------
         asyncio.TimeoutError
             If `timeout` is set and is reached while no message has
             been received from the client.
 
         Returns
         -------
-        message: Message
+        message:
             Collected message that was sent by `client`.
 
         Notes
         -----
         See the `check_message` method to synchronously check whether
         a message from the client is available and return it or None.
         """
-        countdown = -1
-        if timeout is not None:
-            countdown = (timeout // heartbeat) + bool(timeout % heartbeat)
+        countdown = (
+            max(math.ceil(timeout / self.heartbeat), 1) if timeout else -1
+        )
         while countdown:
             message = self.check_message(client)
             if message is not None:
                 return message
-            await asyncio.sleep(heartbeat)
+            await asyncio.sleep(self.heartbeat)
             countdown -= 1
         raise asyncio.TimeoutError(
             "Timeout reached before a message was received."
         )
 
+    def open_clients_registration(
+        self,
+    ) -> None:
+        """Make this servicer accept registration of new clients."""
+        self.registration_status = flags.REGISTRATION_OPEN
+
+    def close_clients_registration(
+        self,
+    ) -> None:
+        """Make this servicer reject registration of new clients."""
+        self.registration_status = flags.REGISTRATION_CLOSED
+
     async def wait_for_clients(
         self,
         min_clients: int = 1,
         max_clients: Optional[int] = None,
-        timeout: Optional[int] = None,
-    ) -> Dict[str, Dict[str, Any]]:
+        timeout: Optional[float] = None,
+    ) -> None:
         """Wait for clients to register for training, with given criteria.
 
         Parameters
         ----------
         min_clients: int, default=1
             Minimum number of clients required. Corrected to be >= 1.
             If `timeout` is None, used as the exact number of clients
             required - once reached, registration will be closed.
         max_clients: int or None, default=None
             Maximum number of clients authorized to register.
-        timeout: int or None, default=None
+        timeout: float or None, default=None
             Optional maximum waiting time (in seconds) beyond which
             to close registration and either return or raise.
 
         Raises
         ------
         RuntimeError
             If the number of registered clients does not abide by the
             provided boundaries at the end of the process.
-
-        Returns
-        -------
-        client_info: dict[str, dict[str, any]]
-            A dictionary where the keys are the participants
-            and the values are their information.
         """
         # Ensure any collected information is purged in case of failure
         # (due to raised errors or wrong number of registered clients).
         try:
             await self._wait_for_clients(min_clients, max_clients, timeout)
         except Exception as exc:  # re-raise; pylint: disable=broad-except
-            self.registration_status = flags.REGISTRATION_UNSTARTED
             await self.purge()
             raise exc
-        return self.data_info.copy()
 
     async def _wait_for_clients(
         self,
         min_clients: int = 1,
         max_clients: Optional[int] = None,
-        timeout: Optional[int] = None,
+        timeout: Optional[float] = None,
     ) -> None:
         """Backend of `wait_for_clients` method, without safeguards."""
         # Parse information on the required number of clients.
         min_clients = max(min_clients, 1)
-        if max_clients is None:
-            if timeout is None:
-                max_clients = min_clients
-            else:
-                max_clients = float("inf")  # type: ignore
+        max_clients = -1 if max_clients is None else max_clients
+        if max_clients < 0:
+            max_clients = (
+                min_clients if timeout is None else math.inf  # type: ignore
+            )
         else:
             max_clients = max(min_clients, max_clients)
         # Wait for the required number of clients to have joined.
-        self.registration_status = flags.REGISTRATION_OPEN
-        countdown = timeout or -1
-        while countdown:
-            n_clients = len(self.registered_clients)
-            if n_clients >= max_clients:  # type: ignore
-                break
-            await asyncio.sleep(1)
+        self.open_clients_registration()
+        countdown = (
+            max(math.ceil(timeout / self.heartbeat), 1) if timeout else -1
+        )
+        while countdown and (len(self.registered_clients) < max_clients):
+            await asyncio.sleep(self.heartbeat)
             countdown -= 1
-        self.registration_status = flags.REGISTRATION_CLOSED
+        self.close_clients_registration()
         # Check whether all requirements have been checked.
         n_clients = len(self.registered_clients)
-        if not min_clients <= n_clients <= max_clients:  # type: ignore
+        if not min_clients <= n_clients <= max_clients:
             raise RuntimeError(
                 f"The number of registered clients is {n_clients}, which "
                 f"is out of the [{min_clients}, {max_clients}] range."
             )
```

### Comparing `declearn-2.3.2/declearn/communication/grpc/__init__.py` & `declearn-2.4.0/declearn/communication/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/communication/grpc/_client.py` & `declearn-2.4.0/declearn/communication/grpc/_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import grpc  # type: ignore
 
 from declearn.communication.api import NetworkClient
 from declearn.communication.grpc.protobufs import message_pb2
 from declearn.communication.grpc.protobufs.message_pb2_grpc import (
     MessageBoardStub,
 )
-from declearn.communication.messaging import Message, parse_message_from_string
 
 __all__ = [
     "GrpcClient",
 ]
 
 
 CHUNK_LENGTH = 2**22 - 50  # 2**22 - sys.getsizeof("") - 1
@@ -94,41 +93,38 @@
         if self._channel is not None:
             await self._channel.close()
             self._channel = None
             self._service = None
 
     async def _send_message(
         self,
-        message: Message,
-    ) -> Message:
+        message: str,
+    ) -> str:
         """Send a message to the server and return the obtained reply."""
         if self._service is None:
             raise RuntimeError("Cannot send messages while not connected.")
         # Send the message, as a unary or as a stream of message chunks.
-        string = message.to_string()
-        if len(string) <= CHUNK_LENGTH:
-            message = message_pb2.Message(message=string)
+        if len(message) <= CHUNK_LENGTH:
+            message = message_pb2.Message(message=message)
             replies = self._service.send(message)
         else:
-            # fmt: off
             chunks = (
-                message_pb2.Message(message=string[idx:idx + CHUNK_LENGTH])
-                for idx in range(0, len(string), CHUNK_LENGTH)
+                message_pb2.Message(message=message[idx : idx + CHUNK_LENGTH])
+                for idx in range(0, len(message), CHUNK_LENGTH)
             )
-            # fmt: on
             replies = self._service.send_stream(chunks)
         # Collect the reply from a stream of message chunks.
         buffer = ""
         async for chunk in replies:
             buffer += chunk.message
-        return parse_message_from_string(buffer)
+        return buffer
 
     async def register(
         self,
-        data_info: Dict[str, Any],
+        data_info: Optional[Dict[str, Any]] = None,
     ) -> bool:
         try:
             return await super().register(data_info)
         except grpc.aio.AioRpcError as err:
             self.logger.error(
                 "Connection failed during registration: %s %s",
                 err.code(),
```

### Comparing `declearn-2.3.2/declearn/communication/grpc/_server.py` & `declearn-2.4.0/declearn/communication/grpc/_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,22 +23,20 @@
 from concurrent import futures
 from typing import AsyncIterator, Optional, Union
 
 import grpc  # type: ignore
 from cryptography.hazmat.primitives import serialization
 
 from declearn.communication.api import NetworkServer
-from declearn.communication.api._service import MessagesHandler
+from declearn.communication.api.backend import MessagesHandler, actions, flags
 from declearn.communication.grpc.protobufs import message_pb2
 from declearn.communication.grpc.protobufs.message_pb2_grpc import (
     MessageBoardServicer,
     add_MessageBoardServicer_to_server,
 )
-from declearn.communication.messaging import Error
-
 
 __all__ = [
     "GrpcServer",
 ]
 
 
 CHUNK_LENGTH = 2**22 - 50  # 2**22 - sys.getsizeof("") - 1
@@ -76,14 +74,15 @@
     def __init__(
         self,
         host: str = "localhost",
         port: int = 8765,
         certificate: Optional[str] = None,
         private_key: Optional[str] = None,
         password: Optional[str] = None,
+        heartbeat: float = 1.0,
         logger: Union[logging.Logger, str, None] = None,
     ) -> None:
         """Instantiate the server-side gRPC communications handler.
 
         Parameters
         ----------
         host : str, default='localhost'
@@ -99,22 +98,25 @@
         private_key: str or None, default=None
             Path to the server private key to use SSL/TLS communications
             encryption. If provided, `certificate` must be set as well.
         password: str or None, default=None
             Optional password used to access `private_key`, or path to a
             file from which to read such a password.
             If None but a password is needed, an input will be prompted.
+        heartbeat: float, default=1.0
+            Delay (in seconds) between verifications when checking for a
+            message having beend received from or collected by a client.
         logger: logging.Logger or str or None, default=None,
             Logger to use, or name of a logger to set up with
             `declearn.utils.get_logger`. If None, use `type(self)`.
         """
         # inherited signature; pylint: disable=too-many-arguments
         # Assign attributes and set up the gRPC server.
         super().__init__(
-            host, port, certificate, private_key, password, logger
+            host, port, certificate, private_key, password, heartbeat, logger
         )
         self._server = None  # type: Optional[grpc.Server]
 
     @property
     def uri(self) -> str:
         return f"{self.host}:{self.port}"
 
@@ -215,17 +217,15 @@
         request_iterator: AsyncIterator[message_pb2.Message],  # type: ignore
         context: grpc.ServicerContext,
     ) -> AsyncIterator[message_pb2.Message]:  # type: ignore
         """Handle a chunked Message-sending request from a client."""
         # async is needed; pylint: disable=invalid-overridden-method
         # Case when an unknown peer attempts sending a stream: send an error.
         if context.peer() not in self.handler.registered_clients:
-            error = Error(
-                "Chunked messages from unregistered clients are not allowed."
-            )
+            error = actions.Reject(flags.REJECT_UNREGISTERED_CHUNKED)
             self.handler.logger.warning(
                 "Refused a chunks-streaming request from client %s",
                 context.peer(),
             )
             yield message_pb2.Message(message=error.to_string())
         # Otherwise, assemble the message for streamed chunks, then reply.
         else:
```

### Comparing `declearn-2.3.2/declearn/communication/grpc/protobufs/__init__.py` & `declearn-2.4.0/declearn/communication/grpc/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/communication/grpc/protobufs/message_pb2.py` & `declearn-2.4.0/declearn/communication/grpc/protobufs/message_pb2.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/communication/grpc/protobufs/message_pb2_grpc.py` & `declearn-2.4.0/declearn/communication/grpc/protobufs/message_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/communication/messaging/_messages.py` & `declearn-2.4.0/declearn/messaging/_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,91 +11,58 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Dataclasses defining messages used in declearn communications."""
+"""Messages for the default Federated Learning process of DecLearn."""
 
 import dataclasses
-import json
-from abc import ABCMeta
-from typing import Any, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, Dict, List, Optional, Tuple
 
-import numpy as np
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
-from declearn.metrics import MetricInputType
+from declearn.aggregator import Aggregator, ModelUpdates
+from declearn.messaging._api import Message
+from declearn.metrics import MetricInputType, MetricState
 from declearn.model.api import Model, Vector
 from declearn.optimizer import Optimizer
-from declearn.utils import (
-    deserialize_object,
-    json_pack,
-    json_unpack,
-    serialize_object,
-)
+from declearn.optimizer.modules import AuxVar
+from declearn.utils import deserialize_object, serialize_object
 
 
 __all__ = [
     "CancelTraining",
-    "Empty",
     "Error",
     "EvaluationReply",
     "EvaluationRequest",
     "GenericMessage",
-    "GetMessageRequest",
     "InitRequest",
-    "JoinReply",
-    "JoinRequest",
-    "Message",
+    "InitReply",
+    "MetadataQuery",
+    "MetadataReply",
     "PrivacyRequest",
+    "PrivacyReply",
     "StopTraining",
     "TrainReply",
     "TrainRequest",
-    "parse_message_from_string",
 ]
 
 
 @dataclasses.dataclass
-class Message(metaclass=ABCMeta):
-    """Base class to define declearn messages."""
-
-    typekey: str = dataclasses.field(init=False)
-
-    def to_string(self) -> str:
-        """Convert the message to a JSON-serialized string."""
-        data = dataclasses.asdict(self)
-        return json.dumps(data, default=json_pack)
-
-    @classmethod
-    def from_kwargs(cls, **kwargs: Any) -> Self:
-        """Parse the message from JSON-deserialized attributes."""
-        # NOTE: override this method to de-serialize attributes
-        #       that are not handled by declearn.utils.json_pack
-        return cls(**kwargs)
-
-
-@dataclasses.dataclass
 class CancelTraining(Message):
     """Empty message used to ping or signal message reception."""
 
     typekey = "cancel"
 
     reason: str
 
 
 @dataclasses.dataclass
-class Empty(Message):
-    """Empty message used to ping or signal message reception."""
-
-    typekey = "empty"
-
-
-@dataclasses.dataclass
 class Error(Message):
     """Error message container, used to convey exceptions between nodes."""
 
     typekey = "error"
 
     message: str
 
@@ -103,97 +70,102 @@
 @dataclasses.dataclass
 class EvaluationRequest(Message):
     """Server-emitted request to participate in an evaluation round."""
 
     typekey = "eval_request"
 
     round_i: int
-    weights: Vector
+    weights: Optional[Vector]
     batches: Dict[str, Any]
     n_steps: Optional[int]
     timeout: Optional[int]
 
 
 @dataclasses.dataclass
 class EvaluationReply(Message):
     """Client-emitted results from a local evaluation round."""
 
     typekey = "eval_reply"
 
     loss: float
     n_steps: int
     t_spent: float
-    metrics: Dict[
-        str, Dict[str, Union[float, np.ndarray]]
-    ] = dataclasses.field(default_factory=dict)
+    metrics: Dict[str, MetricState] = dataclasses.field(default_factory=dict)
+
+    def to_kwargs(
+        self,
+    ) -> Dict[str, Any]:
+        # Undo recursive dict-conversion of dataclasses.
+        kwargs = super().to_kwargs()
+        kwargs["metrics"] = self.metrics
+        return kwargs
 
 
 @dataclasses.dataclass
 class GenericMessage(Message):
     """Generic message format, with action/params pair."""
 
     typekey = "generic"
 
     action: str  # revise: Literal on possible flags?
     params: Dict[str, Any]
 
 
 @dataclasses.dataclass
-class GetMessageRequest(Message):
-    """Client-emitted prompt to collect a message posted by the server."""
-
-    typekey = "get_message"
-
-    timeout: Optional[int] = None
-
-
-@dataclasses.dataclass
 class InitRequest(Message):
     """Server-emitted request to initialize local model and optimizer."""
 
     typekey = "init_request"
 
     model: Model
     optim: Optimizer
+    aggrg: Aggregator
     metrics: List[MetricInputType] = dataclasses.field(default_factory=list)
     dpsgd: bool = False
 
-    def to_string(self) -> str:
-        data = {"typekey": self.typekey}  # type: Dict[str, Any]
+    def to_kwargs(self) -> Dict[str, Any]:
+        data = {}  # type: Dict[str, Any]
         data["model"] = serialize_object(self.model, group="Model").to_dict()
         data["optim"] = self.optim.get_config()
+        data["aggrg"] = serialize_object(self.aggrg, "Aggregator").to_dict()
         data["metrics"] = self.metrics
         data["dpsgd"] = self.dpsgd
-        return json.dumps(data, default=json_pack)
+        return data
 
     @classmethod
     def from_kwargs(cls, **kwargs: Any) -> Self:
         kwargs["model"] = deserialize_object(kwargs["model"])
         kwargs["optim"] = Optimizer.from_config(kwargs["optim"])
+        kwargs["aggrg"] = deserialize_object(kwargs["aggrg"])
         return cls(**kwargs)
 
 
 @dataclasses.dataclass
-class JoinRequest(Message):
-    """Client-emitted request to join training."""
+class InitReply(Message):
+    """Client-emitted message indicating that initialization went fine."""
 
-    typekey = "join_request"
+    typekey = "init_reply"
 
-    name: str
-    data_info: Dict[str, Any]
+
+@dataclasses.dataclass
+class MetadataQuery(Message):
+    """Server-emitted request for metadata on a client's dataset."""
+
+    typekey = "metadata_query"
+
+    fields: List[str]
 
 
 @dataclasses.dataclass
-class JoinReply(Message):
-    """Server-emitted reply to a JoinRequest."""
+class MetadataReply(Message):
+    """Client-emitted metadata in response to a server request."""
 
-    typekey = "join_reply"
+    typekey = "metadata_reply"
 
-    accept: bool
-    flag: str
+    data_info: Dict[str, Any]
 
 
 @dataclasses.dataclass
 class PrivacyRequest(Message):
     """Server-emitted request to set up local differential privacy."""
 
     # dataclass; pylint: disable=too-many-instance-attributes
@@ -210,14 +182,21 @@
     rounds: int
     batches: Dict[str, Any]
     n_epoch: Optional[int]
     n_steps: Optional[int]
 
 
 @dataclasses.dataclass
+class PrivacyReply(Message):
+    """Client-emitted message indicating that DP setup went fine."""
+
+    typekey = "privacy_reply"
+
+
+@dataclasses.dataclass
 class StopTraining(Message):
     """Server-emitted notification that the training process is over."""
 
     typekey = "stop_training"
 
     weights: Vector
     loss: float
@@ -227,59 +206,39 @@
 @dataclasses.dataclass
 class TrainRequest(Message):
     """Server-emitted request to participate in a training round."""
 
     typekey = "train_request"
 
     round_i: int
-    weights: Vector
-    aux_var: Dict[str, Dict[str, Any]]
+    weights: Optional[Vector]
+    aux_var: Dict[str, AuxVar]
     batches: Dict[str, Any]
     n_epoch: Optional[int] = None
     n_steps: Optional[int] = None
     timeout: Optional[int] = None
 
+    def to_kwargs(self) -> Dict[str, Any]:
+        # Undo recursive dict-conversion of dataclasses.
+        data = super().to_kwargs()
+        data["aux_var"] = self.aux_var
+        return data
+
 
 @dataclasses.dataclass
 class TrainReply(Message):
     """Client-emitted results from a local training round."""
 
     typekey = "train_reply"
 
     n_epoch: int
     n_steps: int
     t_spent: float
-    updates: Vector
-    aux_var: Dict[str, Dict[str, Any]]
-
+    updates: ModelUpdates
+    aux_var: Dict[str, AuxVar]
 
-_MESSAGE_CLASSES = [
-    CancelTraining,
-    Empty,
-    Error,
-    EvaluationReply,
-    EvaluationRequest,
-    GenericMessage,
-    GetMessageRequest,
-    InitRequest,
-    JoinReply,
-    JoinRequest,
-    PrivacyRequest,
-    StopTraining,
-    TrainReply,
-    TrainRequest,
-]  # type: List[Type[Message]]
-MESSAGE_CLASSES = {cls.typekey: cls for cls in _MESSAGE_CLASSES}
-
-
-def parse_message_from_string(
-    string: str,
-) -> Message:
-    """Instantiate a Message from a JSON-serialized string."""
-    data = json.loads(string, object_hook=json_unpack)
-    if "typekey" not in data:
-        raise KeyError("Missing required 'typekey'")
-    typekey = data.pop("typekey")
-    cls = MESSAGE_CLASSES.get(typekey)
-    if cls is None:
-        raise KeyError(f"No Message matches typekey '{typekey}'.")
-    return cls.from_kwargs(**data)
+    def to_kwargs(self) -> Dict[str, Any]:
+        # Undo recursive dict-conversion of dataclasses.
+        data = super().to_kwargs()
+        data["updates"] = self.updates
+        data["aux_var"] = self.aux_var
+        return data
```

### Comparing `declearn-2.3.2/declearn/communication/messaging/flags.py` & `declearn-2.4.0/declearn/communication/api/backend/flags.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,33 +11,47 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Communication flags used in declearn communication backends.
+"""Communication flags used by the declearn communication backend.
 
-This module exposes the following flags, which are all str constants:
-
-- REGISTRATION_UNSTARTED
-- REGISTRATION_OPEN
-- REGISTRATION_CLOSED
-- REGISTERED_WELCOME
-- REGISTERED_ALREADY
-- CHECK_MESSAGE_TIMEOUT
-- INVALID_MESSAGE
-- REJECT_UNREGISTERED
+This module exposes conventional flags, which are all str constants.
 """
 
 
+from declearn.version import VERSION
+
+__all__ = [
+    "CHECK_MESSAGE_TIMEOUT",
+    "INVALID_MESSAGE",
+    "REGISTERED_ALREADY",
+    "REGISTERED_WELCOME",
+    "REGISTRATION_CLOSED",
+    "REGISTRATION_OPEN",
+    "REGISTRATION_UNSTARTED",
+    "REJECT_INCOMPATIBLE_VERSION",
+    "REJECT_UNREGISTERED",
+    "REJECT_UNREGISTERED_CHUNKED",
+]
+
+
 # Registration flags.
-REGISTRATION_UNSTARTED = "registration is not opened yet"
-REGISTRATION_OPEN = "registration is open"
-REGISTRATION_CLOSED = "registration is closed"
-REGISTERED_WELCOME = "welcome, you are now registered"
 REGISTERED_ALREADY = "you were already registered"
+REGISTERED_WELCOME = "welcome, you are now registered"
+REGISTRATION_CLOSED = "registration is closed"
+REGISTRATION_OPEN = "registration is open"
+REGISTRATION_UNSTARTED = "registration is not opened yet"
 
 # Error flags.
 CHECK_MESSAGE_TIMEOUT = "no available message at timeout"
 INVALID_MESSAGE = "invalid message"
+REJECT_INCOMPATIBLE_VERSION = (
+    "cannot register due to the DecLearn version in use; "
+    f"please update to `declearn ~= {VERSION}`"
+)
 REJECT_UNREGISTERED = "rejected: not a registered user"
+REJECT_UNREGISTERED_CHUNKED = (
+    "chunked messages from unregistered clients are not allowed"
+)
```

### Comparing `declearn-2.3.2/declearn/communication/websockets/__init__.py` & `declearn-2.4.0/declearn/communication/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/communication/websockets/_client.py` & `declearn-2.4.0/declearn/communication/websockets/_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from typing import Any, Dict, Optional, Union, ClassVar
 
 import websockets as ws
 from websockets.client import WebSocketClientProtocol
 from websockets.exceptions import ConnectionClosedOK, ConnectionClosedError
 
 from declearn.communication.api import NetworkClient
-from declearn.communication.messaging import Message, parse_message_from_string
 from declearn.communication.websockets._tools import (
     receive_websockets_message,
     send_websockets_message,
 )
 
 __all__ = [
     "WebsocketsClient",
@@ -128,30 +127,28 @@
     async def stop(self) -> None:
         if self._socket is not None:
             await self._socket.close()
             self._socket = None
 
     async def _send_message(
         self,
-        message: Message,
-    ) -> Message:
+        message: str,
+    ) -> str:
         """Send a message to the server and return the obtained reply."""
         if self._socket is None:
             raise RuntimeError("Cannot communicate while not connected.")
-        string = message.to_string()
-        await send_websockets_message(string, self._socket)
+        await send_websockets_message(message, self._socket)
         answer = await self._socket.recv()
-        string = await receive_websockets_message(
+        return await receive_websockets_message(
             message=answer, socket=self._socket, allow_chunks=True
         )
-        return parse_message_from_string(string)
 
     async def register(
         self,
-        data_info: Dict[str, Any],
+        data_info: Optional[Dict[str, Any]] = None,
     ) -> bool:
         try:
             return await super().register(data_info)
         except (ConnectionClosedOK, ConnectionClosedError) as err:
             self.logger.error("Connection closed during registration: %s", err)
             self.logger.info("Reconnecting to the server.")
             await self.stop()
```

### Comparing `declearn-2.3.2/declearn/communication/websockets/_server.py` & `declearn-2.4.0/declearn/communication/websockets/_server.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     def __init__(
         self,
         host: str = "localhost",
         port: int = 8765,
         certificate: Optional[str] = None,
         private_key: Optional[str] = None,
         password: Optional[str] = None,
+        heartbeat: float = 1.0,
         logger: Union[logging.Logger, str, None] = None,
     ) -> None:
         """Instantiate the server-side WebSockets communications handler.
 
         Parameters
         ----------
         host : str, default='localhost'
@@ -67,21 +68,24 @@
         private_key: str or None, default=None
             Path to the server private key to use SSL/TLS communications
             encryption. If provided, `certificate` must be set as well.
         password: str or None, default=None
             Optional password used to access `private_key`, or path to a
             file from which to read such a password.
             If None but a password is needed, an input will be prompted.
+        heartbeat: float, default=1.0
+            Delay (in seconds) between verifications when checking for a
+            message having beend received from or collected by a client.
         logger: logging.Logger or str or None, default=None,
             Logger to use, or name of a logger to set up with
             `declearn.utils.get_logger`. If None, use `type(self)`.
         """
         # inherited signature; pylint: disable=too-many-arguments
         super().__init__(
-            host, port, certificate, private_key, password, logger
+            host, port, certificate, private_key, password, heartbeat, logger
         )
         self._server = None  # type: Optional[WebSocketServer]
 
     @property
     def uri(self) -> str:
         protocol = "ws" if self._ssl is None else "wss"
         return f"{protocol}://{self.host}:{self.port}"
```

### Comparing `declearn-2.3.2/declearn/communication/websockets/_tools.py` & `declearn-2.4.0/declearn/communication/websockets/_tools.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/data_info/__init__.py` & `declearn-2.4.0/declearn/data_info/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,31 +48,21 @@
     Specification for the 'classes' field.
 * [DataTypeField][declearn.data_info.DataTypeField]:
     Specification for the 'data_type' field.
 * [FeaturesShapeField][declearn.data_info.FeaturesShapeField]:
     Specification for the 'features_shape' field.
 * [NbSamplesField][declearn.data_info.NbSamplesField]:
     Specification for the 'n_samples' field.
-
-Deprecated field specifications
--------------------------------
-
-* [InputShapeField][declearn.data_info.InputShapeField]:
-    Deprecacted as of v2.2 in favor of FeaturesShapeField.
-* [NbFeaturesField][declearn.data_info.NbFeaturesField]:
-    Deprecacted as of v2.2 in favor of FeaturesShapeField.
 """
 
 from ._base import (
     DataInfoField,
     aggregate_data_info,
     get_data_info_fields_documentation,
     register_data_info_field,
 )
 from ._fields import (
     ClassesField,
     DataTypeField,
-    InputShapeField,
     FeaturesShapeField,
-    NbFeaturesField,
     NbSamplesField,
 )
```

### Comparing `declearn-2.3.2/declearn/data_info/_base.py` & `declearn-2.4.0/declearn/data_info/_base.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/dataset/__init__.py` & `declearn-2.4.0/declearn/dataset/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 API tools
 ---------
 * [Dataset][declearn.dataset.Dataset]:
     Abstract base class defining an API to access training or testing data.
 * [DataSpec][declearn.dataset.DataSpecs]:
     Dataclass to wrap a dataset's metadata.
 * [load_dataset_from_json][declearn.dataset.load_dataset_from_json]
-    Utility function to parse a JSON into a dataset object.
+    DEPRECATED Utility function to parse a JSON into a dataset object.
 
 Dataset subclasses
 ------------------
 * [InMemoryDataset][declearn.dataset.InMemoryDataset]:
     Dataset subclass serving numpy(-like) memory-loaded data arrays.
 
 Manual-import submodules
```

### Comparing `declearn-2.3.2/declearn/dataset/_base.py` & `declearn-2.4.0/declearn/dataset/_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,97 +13,62 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Dataset abstraction API."""
 
+import abc
+import dataclasses
 import warnings
-from abc import ABCMeta, abstractmethod
-from dataclasses import dataclass
 from typing import Any, Iterator, List, Optional, Set, Tuple, Union
 
 from declearn.typing import Batch
 from declearn.utils import access_registered, create_types_registry, json_load
 
 __all__ = [
     "DataSpecs",
     "Dataset",
 ]
 
 
-@dataclass
+@dataclasses.dataclass
 class DataSpecs:
-    """Dataclass to wrap a dataset's metadata.
-
-    Note
-    ----
-    The `n_features` attribute has been deprecated as of declearn 2.2
-    and will be removed in v2.4 and/or v3.0. It should therefore not
-    be used, whether at instantiation or afterwards. Please use the
-    `features_shape` attribute instead.
-    """
+    """Dataclass to wrap a dataset's metadata."""
 
     n_samples: int
     features_shape: Optional[
         Union[Tuple[Optional[int], ...], List[Optional[int]]]
     ] = None
     classes: Optional[Set[Any]] = None
     data_type: Optional[str] = None
-    n_features: Optional[int] = None  # DEPRECATED as of declearn v2.2
-
-    def __post_init__(self):  # pragma: no cover
-        # future: remove this (declearn >=2.4)
-        if isinstance(self.features_shape, int):
-            self.features_shape = (self.features_shape,)
-            warnings.warn(
-                "'features_shape' has replaced now-deprecated 'n_features'"
-                " and should therefore be passed as a tuple or list.",
-                RuntimeWarning,
-                stacklevel=3,
-            )
-        if self.n_features is not None:
-            warnings.warn(
-                "'DataSepc.n_features' has been deprecated as of declearn v2.2"
-                " and should therefore no longer be used. It will be removed"
-                " in v2.4 and/or v3.0.",
-                RuntimeWarning,
-                stacklevel=3,
-            )
-            if self.features_shape[-1] != self.n_features:
-                raise ValueError(
-                    "Both 'features_shape' and deprecated 'n_features' were "
-                    "passed to 'DataSpecs.__init__', with incoherent values."
-                )
-        if self.features_shape:
-            self.n_features = self.features_shape[-1]
 
 
 @create_types_registry
-class Dataset(metaclass=ABCMeta):
+class Dataset(metaclass=abc.ABCMeta):
     """Abstract class defining an API to access training or testing data.
 
     A 'Dataset' is an interface towards data that exposes methods
     to query batched data samples and key metadata while remaining
     agnostic of the way the data is actually being loaded (from a
     source file, a database, a network reader, another API...).
 
     This is notably done to allow clients to use distinct data
     storage and loading architectures, even implementing their
     own subclass if needed, while ensuring that data access is
     straightforward to specify as part of FL algorithms.
     """
 
-    @abstractmethod
+    @abc.abstractmethod
     def get_data_specs(
         self,
     ) -> DataSpecs:
         """Return a DataSpecs object describing this dataset."""
 
-    @abstractmethod
+    @abc.abstractmethod
     def generate_batches(  # pylint: disable=too-many-arguments
         self,
         batch_size: int,
         shuffle: bool = False,
         drop_remainder: bool = True,
         replacement: bool = False,
         poisson: bool = False,
@@ -142,26 +107,44 @@
             May be None for unsupervised or semi-supervised tasks.
         weights: 1-d data array or None
             Optional weights associated with the samples, that are
             typically used to balance a model's loss or metrics.
         """
 
 
-def load_dataset_from_json(path: str) -> Dataset:
-    """Instantiate a dataset based on a JSON dump file.
+def load_dataset_from_json(path: str) -> Dataset:  # pragma: no cover
+    """DEPRECATED Instantiate a dataset based on a JSON dump file.
 
     Parameters
     ----------
     path: str
         Path to a JSON file output by the `save_to_json`
         method of the Dataset that is being reloaded.
         The actual type of dataset should be specified
         under the "name" field of that file.
 
     Returns
     -------
     dataset: Dataset
         Dataset (subclass) instance, reloaded from JSON.
+
+    Raises
+    ------
+    NotImplementedError
+        If the target `Dataset` does not implement a `load_from_json`
+        method (which was removed from the API in DecLearn 2.3.0).
     """
+    warnings.warn(
+        "'load_dataset_from_json' was deprecated in Declearn 2.4.0, after"
+        "'Dataset.load_from_json' was removed from the API in v2.3.0. It "
+        "may raise a 'NotImplementedError', and will be removed in DecLearn "
+        "2.6 and/or 3.0.",
+        category=DeprecationWarning,
+        stacklevel=2,
+    )
     dump = json_load(path)
     cls = access_registered(dump["name"], group="Dataset")
+    if not hasattr(cls, "load_from_json"):
+        raise NotImplementedError(
+            f"Dataset class '{cls}' does not implement 'load_from_json'."
+        )
     return cls.load_from_json(path)
```

### Comparing `declearn-2.3.2/declearn/dataset/_inmemory.py` & `declearn-2.4.0/declearn/dataset/_inmemory.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Dataset implementation to serve scikit-learn compatible in-memory data."""
 
 import os
-import warnings
 from typing import Any, Dict, Iterator, List, Optional, Set, Union
 
 import numpy as np
 import pandas as pd
 from numpy.typing import ArrayLike
 from scipy.sparse import spmatrix  # type: ignore
 from sklearn.datasets import load_svmlight_file  # type: ignore
@@ -218,56 +217,14 @@
             return list(dtypes)[0]
         if isinstance(self.feats, (pd.Series, np.ndarray, spmatrix)):
             return str(self.feats.dtype)
         raise TypeError(  # pragma: no cover
             f"Invalid 'data' attribute type: '{type(self.target)}'."
         )
 
-    @staticmethod
-    def load_data_array(
-        path: str,
-        **kwargs: Any,
-    ) -> DataArray:  # pragma: no cover
-        """Load a data array from a dump file.
-
-        As of declearn v2.2, this staticmethod is DEPRECATED in favor of
-        `declearn.dataset.utils.load_data_array`, which is now calls. It
-        will be removed in v2.4 and/or v3.0.
-
-        See [declearn.dataset.utils.load_data_array][] for more details.
-        """
-        warnings.warn(
-            "'InMemoryDataset.load_data_array' has been deprecated in favor"
-            " of `declearn.dataset.utils.load_data_array`. It will be removed"
-            " in version 2.4 and/or 3.0.",
-            category=DeprecationWarning,
-        )
-        return load_data_array(path, **kwargs)
-
-    @staticmethod
-    def save_data_array(
-        path: str,
-        array: Union[DataArray, pd.Series],
-    ) -> str:  # pragma: no cover
-        """Save a data array to a dump file.
-
-        As of declearn v2.2, this staticmethod is DEPRECATED in favor of
-        `declearn.dataset.utils.save_data_array`, which is now calls. It
-        will be removed in v2.4 and/or v3.0.
-
-        See [declearn.dataset.utils.save_data_array][] for more details.
-        """
-        warnings.warn(
-            "'InMemoryDataset.save_data_array' has been deprecated in favor"
-            " of `declearn.dataset.utils.save_data_array`. It will be removed"
-            " in version 2.4 and/or 3.0.",
-            category=DeprecationWarning,
-        )
-        return save_data_array(path, array)
-
     @classmethod
     def from_svmlight(
         cls,
         path: str,
         f_cols: Optional[List[int]] = None,
         dtype: Union[str, np.dtype] = "float64",
     ) -> Self:
```

### Comparing `declearn-2.3.2/declearn/dataset/_split_data.py` & `declearn-2.4.0/declearn/dataset/_split_data.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/dataset/examples/__init__.py` & `declearn-2.4.0/declearn/dataset/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/dataset/examples/_heart_uci.py` & `declearn-2.4.0/declearn/dataset/examples/_heart_uci.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/dataset/examples/_mnist.py` & `declearn-2.4.0/declearn/dataset/examples/_mnist.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/dataset/tensorflow/__init__.py` & `declearn-2.4.0/declearn/dataset/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/dataset/tensorflow/_tensorflow.py` & `declearn-2.4.0/declearn/dataset/tensorflow/_tensorflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
         "Invalid value for 'batch_mode': should be one of "
         f"{{'default', 'padded', 'ragged'}}, not '{batch_mode}'."
     )
 
 
 def get_stack_function(
     batch_mode: BatchMode,
-) -> Callable[[Union[List[None], List[tf.Tensor]]], Optional[tf.Tensor],]:
+) -> Callable[[Union[List[None], List[tf.Tensor]]], Optional[tf.Tensor]]:
     """Return a function to stack sample-wise atomic elements."""
     if batch_mode == "default":
         return _stack_default
     if batch_mode == "padded":
         return _stack_padded
     if batch_mode == "ragged":
         return _stack_ragged
```

### Comparing `declearn-2.3.2/declearn/dataset/torch/__init__.py` & `declearn-2.4.0/declearn/dataset/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/dataset/torch/_torch.py` & `declearn-2.4.0/declearn/dataset/torch/_torch.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/dataset/torch/_utils.py` & `declearn-2.4.0/declearn/dataset/torch/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,16 @@
             Number of samples in the dataset to sample from.
         sample_rate: float
             Sampling rate, i.e. probability for each sample to be included
             in any given batch. Hence, average number of samples per batch.
         generator: torch.Generator or None, default=None
             Optional RNG, that may be used to produce seeded results.
         """
+        # super init is empty and its signature will change in torch 2.2
+        # pylint: disable=super-init-not-called
         self.num_samples = num_samples
         self.sample_rate = sample_rate
         self.generator = generator
 
     def __len__(self):
         return int(1 / self.sample_rate)
```

### Comparing `declearn-2.3.2/declearn/dataset/utils/__init__.py` & `declearn-2.4.0/declearn/dataset/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/dataset/utils/_save_load.py` & `declearn-2.4.0/declearn/dataset/utils/_save_load.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/dataset/utils/_sparse.py` & `declearn-2.4.0/declearn/dataset/utils/_sparse.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/dataset/utils/_split_classif.py` & `declearn-2.4.0/declearn/dataset/utils/_split_classif.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/main/__init__.py` & `declearn-2.4.0/declearn/main/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/main/_client.py` & `declearn-2.4.0/declearn/main/_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,21 +16,28 @@
 # limitations under the License.
 
 """Client-side main Federated Learning orchestrating class."""
 
 import asyncio
 import dataclasses
 import logging
+import os
 from typing import Any, Dict, Optional, Union
 
-from declearn.communication import NetworkClientConfig, messaging
+import numpy as np
+
+from declearn import messaging
 from declearn.communication.api import NetworkClient
+from declearn.communication.utils import (
+    NetworkClientConfig,
+    verify_server_message_validity,
+)
 from declearn.dataset import Dataset, load_dataset_from_json
 from declearn.main.utils import Checkpointer, TrainingManager
-from declearn.utils import get_logger
+from declearn.utils import LOGGING_LEVEL_MAJOR, get_logger
 
 
 __all__ = [
     "FederatedClient",
 ]
 
 
@@ -43,45 +50,51 @@
         self,
         netwk: Union[NetworkClient, NetworkClientConfig, Dict[str, Any], str],
         train_data: Union[Dataset, str],
         valid_data: Optional[Union[Dataset, str]] = None,
         checkpoint: Union[Checkpointer, Dict[str, Any], str, None] = None,
         share_metrics: bool = True,
         logger: Union[logging.Logger, str, None] = None,
+        verbose: bool = True,
     ) -> None:
         """Instantiate a client to participate in a federated learning task.
 
         Parameters
         ----------
         netwk: NetworkClient or NetworkClientConfig or dict or str
             NetworkClient communication endpoint instance, or configuration
             dict, dataclass or path to a TOML file enabling its instantiation.
             In the latter three cases, the object's default logger will be set
             to that of this `FederatedClient`.
         train_data: Dataset or str
-            Dataset instance wrapping the training data, or path to
-            a JSON file from which it can be instantiated.
+            Dataset instance wrapping the training data.
+            (DEPRECATED) May be a path to a JSON dump file.
         valid_data: Dataset or str or None
-            Optional Dataset instance wrapping validation data, or
-            path to a JSON file from which it can be instantiated.
+            Optional Dataset instance wrapping validation data.
             If None, run evaluation rounds over `train_data`.
+            (DEPRECATED) May be a path to a JSON dump file.
         checkpoint: Checkpointer or dict or str or None, default=None
             Optional Checkpointer instance or instantiation dict to be
             used so as to save round-wise model, optimizer and metrics.
             If a single string is provided, treat it as the checkpoint
             folder path and use default values for other parameters.
         share_metrics: bool, default=True
             Whether to share evaluation metrics with the server,
             or save them locally and only send the model's loss.
             This may prevent information leakage, e.g. as to the
             local distribution of target labels or values.
         logger: logging.Logger or str or None, default=None,
             Logger to use, or name of a logger to set up with
             `declearn.utils.get_logger`.
             If None, use `type(self):netwk.name`.
+        verbose: bool, default=True
+            Whether to verbose about ongoing operations.
+            If True, display progress bars during training and validation
+            rounds. If False and `logger is None`, set the logger's level
+            to filter off most routine information.
         """
         # arguments serve modularity; pylint: disable=too-many-arguments
         # Assign the wrapped NetworkClient.
         replace_netwk_logger = False
         if isinstance(netwk, str):
             netwk = NetworkClientConfig.from_toml(netwk)
         elif isinstance(netwk, dict):
@@ -94,15 +107,16 @@
                 "'netwk' should be a declearn.communication.api.NetworkClient,"
                 " or the valid configuration of one."
             )
         self.netwk = netwk
         # Assign the logger and optionally replace that of the network client.
         if not isinstance(logger, logging.Logger):
             logger = get_logger(
-                logger or f"{type(self).__name__}-{netwk.name}"
+                name=logger or f"{type(self).__name__}-{netwk.name}",
+                level=logging.INFO if verbose else LOGGING_LEVEL_MAJOR,
             )
         self.logger = logger
         if replace_netwk_logger:
             self.netwk.logger = self.logger
         # Assign the wrapped training dataset.
         if isinstance(train_data, str):
             train_data = load_dataset_from_json(train_data)
@@ -115,16 +129,17 @@
         if not (valid_data is None or isinstance(valid_data, Dataset)):
             raise TypeError("'valid_data' should be a Dataset or path to one.")
         self.valid_data = valid_data
         # Assign an optional checkpointer.
         if checkpoint is not None:
             checkpoint = Checkpointer.from_specs(checkpoint)
         self.ckptr = checkpoint
-        # Record the metric-sharing boolean switch.
+        # Record the metric-sharing and verbosity bool values.
         self.share_metrics = bool(share_metrics)
+        self.verbose = bool(verbose)
         # Create a TrainingManager slot, populated at initialization phase.
         self.trainmanager = None  # type: Optional[TrainingManager]
 
     def run(
         self,
     ) -> None:
         """Participate in the federated learning process.
@@ -149,48 +164,48 @@
         """
         async with self.netwk:
             # Register for training, then collect initialization information.
             await self.register()
             await self.initialize()
             # Process server instructions as they come.
             while True:
-                message = await self.netwk.check_message()
+                message = await self.netwk.recv_message()
                 stoprun = await self.handle_message(message)
                 if stoprun:
                     break
 
     async def handle_message(
         self,
-        message: messaging.Message,
+        message: messaging.SerializedMessage,
     ) -> bool:
         """Handle an incoming message from the server.
 
         Parameters
         ----------
-        message: messaging.Message
-            Message instance that needs triage and processing.
+        message: messaging.SerializedMessage
+            Serialized message that needs triage and processing.
 
         Returns
         -------
         exit_loop: bool
             Whether to interrupt the client's message-receiving loop.
         """
         exit_loop = False
-        if isinstance(message, messaging.TrainRequest):
-            await self.training_round(message)
-        elif isinstance(message, messaging.EvaluationRequest):
-            await self.evaluation_round(message)
-        elif isinstance(message, messaging.StopTraining):
-            await self.stop_training(message)
+        if issubclass(message.message_cls, messaging.TrainRequest):
+            await self.training_round(message.deserialize())
+        elif issubclass(message.message_cls, messaging.EvaluationRequest):
+            await self.evaluation_round(message.deserialize())
+        elif issubclass(message.message_cls, messaging.StopTraining):
+            await self.stop_training(message.deserialize())
             exit_loop = True
-        elif isinstance(message, messaging.CancelTraining):
-            await self.cancel_training(message)
+        elif issubclass(message.message_cls, messaging.CancelTraining):
+            await self.cancel_training(message.deserialize())
         else:
-            error = "Unexpected instruction received from server:"
-            error += repr(message)
+            error = "Unexpected message type received from server: "
+            error += message.message_cls.__name__
             self.logger.error(error)
             raise ValueError(error)
         return exit_loop
 
     async def register(
         self,
     ) -> None:
@@ -198,21 +213,19 @@
 
         Raises
         ------
         RuntimeError
             If registration has failed 10 times (with a 1 minute delay
             between connection and registration attempts).
         """
-        # revise: add validation dataset specs
-        data_info = dataclasses.asdict(self.train_data.get_data_specs())
         for i in range(10):  # max_attempts (10)
             self.logger.info(
                 "Attempting to join training (attempt n°%s)", i + 1
             )
-            registered = await self.netwk.register(data_info)
+            registered = await self.netwk.register()
             if registered:
                 break
             await asyncio.sleep(60)  # delay_retries (1 minute)
         else:
             raise RuntimeError("Failed to register for training.")
 
     async def initialize(
@@ -233,79 +246,99 @@
         Returns
         -------
         model: Model
             Model that is to be trained (with shared initial parameters).
         optim: Optimizer
             Optimizer that is to be used locally to train the model.
         """
-        # Await initialization instructions. Report messages-unpacking errors.
+        # Await initialization instructions.
         self.logger.info("Awaiting initialization instructions from server.")
+        received = await self.netwk.recv_message()
+        # If a MetadataQuery is received, process it, then await InitRequest.
+        if issubclass(received.message_cls, messaging.MetadataQuery):
+            await self._collect_and_send_metadata(received.deserialize())
+            received = await self.netwk.recv_message()
+        # Ensure that an 'InitRequest' was received.
+        message = await verify_server_message_validity(
+            self.netwk, received, expected=messaging.InitRequest
+        )
+        # Perform initialization, catching errors to report them to the server.
         try:
-            message = await self.netwk.check_message()
+            self.trainmanager = TrainingManager(
+                model=message.model,
+                optim=message.optim,
+                aggrg=message.aggrg,
+                train_data=self.train_data,
+                valid_data=self.valid_data,
+                metrics=message.metrics,
+                logger=self.logger,
+                verbose=self.verbose,
+            )
         except Exception as exc:
             await self.netwk.send_message(messaging.Error(repr(exc)))
             raise RuntimeError("Initialization failed.") from exc
-        # Otherwise, check that the request is of valid type.
-        if not isinstance(message, messaging.InitRequest):
-            error = f"Awaited InitRequest message, got: '{message}'"
-            self.logger.error(error)
-            raise RuntimeError(error)
-        # Send back an empty message to indicate that all went fine.
-        self.logger.info("Notifying the server that initialization went fine.")
-        await self.netwk.send_message(
-            messaging.GenericMessage(action="InitializationOK", params={})
-        )
-        # Wrap up the model and optimizer received from the server.
-        self.trainmanager = TrainingManager(
-            model=message.model,
-            optim=message.optim,
-            train_data=self.train_data,
-            valid_data=self.valid_data,
-            metrics=message.metrics,
-            logger=self.logger,
-        )
-        # If instructed to do so, await a PrivacyRequest to set up DP-SGD.
+        # If instructed to do so, run additional steps to set up DP-SGD.
         if message.dpsgd:
             await self._initialize_dpsgd()
+        # Send back an empty message to indicate that all went fine.
+        self.logger.info("Notifying the server that initialization went fine.")
+        await self.netwk.send_message(messaging.InitReply())
         # Optionally checkpoint the received model and optimizer.
         if self.ckptr:
             self.ckptr.checkpoint(
                 model=self.trainmanager.model,
                 optimizer=self.trainmanager.optim,
                 first_call=True,
             )
 
+    async def _collect_and_send_metadata(
+        self,
+        message: messaging.MetadataQuery,
+    ) -> None:
+        """Collect and report some metadata based on server instructions."""
+        self.logger.info("Collecting metadata to send to the server.")
+        metadata = dataclasses.asdict(self.train_data.get_data_specs())
+        if missing := set(message.fields).difference(metadata):
+            err_msg = f"Metadata query for undefined fields: {missing}."
+            await self.netwk.send_message(messaging.Error(err_msg))
+            raise RuntimeError(err_msg)
+        data_info = {key: metadata[key] for key in message.fields}
+        self.logger.info(
+            "Sending training dataset metadata to the server: %s.",
+            list(data_info),
+        )
+        await self.netwk.send_message(messaging.MetadataReply(data_info))
+
     async def _initialize_dpsgd(
         self,
     ) -> None:
         """Set up differentially-private training as part of initialization.
 
         This method wraps the `make_private` one in the context of
         `initialize` and should never be called in another context.
         """
-        message = await self.netwk.check_message()
-        if not isinstance(message, messaging.PrivacyRequest):
-            msg = f"Expected a PrivacyRequest but received a '{type(message)}'"
-            self.logger.error(msg)
-            await self.netwk.send_message(messaging.Error(msg))
-            raise RuntimeError(f"DP-SGD initialization failed: {msg}.")
+        received = await self.netwk.recv_message()
+        try:
+            message = await verify_server_message_validity(
+                self.netwk, received, expected=messaging.PrivacyRequest
+            )
+        except Exception as exc:
+            raise RuntimeError("DP-SGD initialization failed.") from exc
         self.logger.info("Received a request to set up DP-SGD.")
         try:
             self.make_private(message)
         except Exception as exc:  # pylint: disable=broad-except
             self.logger.error(
                 "Exception encountered in `make_private`: %s", exc
             )
             await self.netwk.send_message(messaging.Error(repr(exc)))
             raise RuntimeError("DP-SGD initialization failed.") from exc
         # If things went right, notify the server.
         self.logger.info("Notifying the server that DP-SGD setup went fine.")
-        await self.netwk.send_message(
-            messaging.GenericMessage(action="privacy-ok", params={})
-        )
+        await self.netwk.send_message(messaging.PrivacyReply())
 
     def make_private(
         self,
         message: messaging.PrivacyRequest,
     ) -> None:
         """Set up differentially-private training, using DP-SGD.
 
@@ -327,18 +360,20 @@
         # heavy-loadtime dependencies; pylint: disable=import-outside-toplevel
         from declearn.main.privacy import DPTrainingManager
 
         # pylint: enable=import-outside-toplevel
         self.trainmanager = DPTrainingManager(
             model=self.trainmanager.model,
             optim=self.trainmanager.optim,
+            aggrg=self.trainmanager.aggrg,
             train_data=self.trainmanager.train_data,
             valid_data=self.trainmanager.valid_data,
             metrics=self.trainmanager.metrics,
             logger=self.trainmanager.logger,
+            verbose=self.trainmanager.verbose,
         )
         self.trainmanager.make_private(message)
 
     async def training_round(
         self,
         message: messaging.TrainRequest,
     ) -> None:
@@ -352,14 +387,24 @@
         ----------
         message: TrainRequest
             Instructions from the server regarding the training round.
         """
         assert self.trainmanager is not None
         # Run the training round.
         reply = self.trainmanager.training_round(message)
+        # Collect and optionally record batch-wise training losses.
+        # Note: collection enables purging them from memory.
+        losses = self.trainmanager.model.collect_training_losses()
+        if self.ckptr is not None:
+            self.ckptr.save_metrics(
+                metrics={"training_losses": np.array(losses)},
+                prefix="training_losses",
+                append=True,
+                timestamp=f"round_{message.round_i}",
+            )
         # Send training results (or error message) to the server.
         await self.netwk.send_message(reply)
 
     async def evaluation_round(
         self,
         message: messaging.EvaluationRequest,
     ) -> None:
@@ -408,15 +453,15 @@
         """
         self.logger.info(
             "Training is now over, after %s rounds. Global loss: %s",
             message.rounds,
             message.loss,
         )
         if self.ckptr:
-            path = f"{self.ckptr.folder}/model_state_best.json"
+            path = os.path.join(self.ckptr.folder, "model_state_best.json")
             self.logger.info("Checkpointing final weights under %s.", path)
             assert self.trainmanager is not None  # for mypy
             self.trainmanager.model.set_weights(message.weights)
             self.ckptr.save_model(self.trainmanager.model, timestamp="best")
 
     async def cancel_training(
         self,
```

### Comparing `declearn-2.3.2/declearn/main/_server.py` & `declearn-2.4.0/declearn/main/_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,36 +14,40 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Server-side main Federated Learning orchestrating class."""
 
 import asyncio
+import copy
 import dataclasses
 import logging
 from typing import Any, Dict, List, Optional, Set, Tuple, Type, TypeVar, Union
 
 import numpy as np
 
-from declearn.communication import NetworkServerConfig, messaging
+from declearn import messaging
+from declearn.communication import NetworkServerConfig
 from declearn.communication.api import NetworkServer
 from declearn.main.config import (
     EvaluateConfig,
     FLOptimConfig,
     FLRunConfig,
     TrainingConfig,
 )
 from declearn.main.utils import (
     AggregationError,
     Checkpointer,
     EarlyStopping,
     aggregate_clients_data_info,
 )
 from declearn.metrics import MetricInputType, MetricSet
+from declearn.metrics._mean import MeanState
 from declearn.model.api import Model, Vector
+from declearn.optimizer.modules import AuxVar
 from declearn.utils import deserialize_object, get_logger
 
 
 __all__ = [
     "FederatedServer",
 ]
 
@@ -143,14 +147,16 @@
         # Assign an optional checkpointer.
         if checkpoint is not None:
             checkpoint = Checkpointer.from_specs(checkpoint)
         self.ckptr = checkpoint
         # Set up private attributes to record the loss values and best weights.
         self._loss = {}  # type: Dict[int, float]
         self._best = None  # type: Optional[Vector]
+        # Set up a private attribute to prevent redundant weights sharing.
+        self._clients_holding_latest_model = set()  # type: Set[str]
 
     def run(
         self,
         config: Union[FLRunConfig, str, Dict[str, Any]],
     ) -> None:
         """Orchestrate the federated learning routine.
 
@@ -234,72 +240,80 @@
         RuntimeError
             In case any of the clients returned an Error message rather
             than an Empty ping-back message. Send CancelTraining to all
             clients before raising.
         """
         # Gather the RegisterConfig instance from the main FLRunConfig.
         regst_cfg = config.register
-        # Wait for clients to register and process their data information.
+        # Wait for clients to register.
         self.logger.info("Starting clients registration process.")
-        data_info = await self.netwk.wait_for_clients(
+        await self.netwk.wait_for_clients(
             regst_cfg.min_clients, regst_cfg.max_clients, regst_cfg.timeout
         )
         self.logger.info("Clients' registration is now complete.")
-        await self._process_data_info(data_info)
+        # When needed, prompt clients for metadata and process them.
+        await self._require_and_process_data_info()
         # Serialize intialization information and send it to clients.
         message = messaging.InitRequest(
             model=self.model,
             optim=self.c_opt,
+            aggrg=self.aggrg,
             metrics=self.metrics.get_config()["metrics"],
             dpsgd=config.privacy is not None,
         )
         self.logger.info("Sending initialization requests to clients.")
         await self.netwk.broadcast_message(message)
         # Await a confirmation from clients that initialization went well.
         # If any client has failed to initialize, raise.
         self.logger.info("Waiting for clients' responses.")
         await self._collect_results(
             clients=self.netwk.client_names,
-            msgtype=messaging.GenericMessage,
-            context="initialization",
+            msgtype=messaging.InitReply,
+            context="Initialization",
         )
         # If local differential privacy is configured, set it up.
         if config.privacy is not None:
             await self._initialize_dpsgd(config)
         self.logger.info("Initialization was successful.")
 
-    async def _process_data_info(
+    async def _require_and_process_data_info(
         self,
-        clients_data_info: Dict[str, Dict[str, Any]],
     ) -> None:
-        """Validate, aggregate and make use of clients' data-info.
-
-        Parameters
-        ----------
-        clients_data_info: dict[str, dict[str, any]]
-            Client-wise data-info dict, that are to be aggregated
-            and passed to the global model for initialization.
+        """Collect, validate, aggregate and make use of clients' data-info.
 
         Raises
         ------
         AggregationError
             In case (some of) the clients' data info is invalid, or
             incompatible. Send CancelTraining to all clients before
             raising.
         """
         fields = self.model.required_data_info  # revise: add optimizer, etc.
+        if not fields:
+            return
+        # Collect required metadata from clients.
+        query = messaging.MetadataQuery(list(fields))
+        await self.netwk.broadcast_message(query)
+        replies = await self._collect_results(
+            self.netwk.client_names,
+            msgtype=messaging.MetadataReply,
+            context="Metadata collection",
+        )
+        clients_data_info = {
+            client: reply.data_info for client, reply in replies.items()
+        }
         # Try aggregating the input data_info.
         try:
             info = aggregate_clients_data_info(clients_data_info, fields)
         # In case of failure, cancel training, notify clients, log and raise.
         except AggregationError as exc:
             messages = {
                 client: messaging.CancelTraining(reason)
                 for client, reason in exc.messages.items()
-            }  # type: Dict[str, messaging.Message]
+            }
             await self.netwk.send_messages(messages)
             self.logger.error(exc.error)
             raise exc
         # Otherwise, initialize the model based on the aggregated information.
         self.model.initialize(info)
 
     async def _collect_results(
@@ -332,21 +346,22 @@
         results: dict[str, `msgtype`]
             Client-wise collected messages.
         """
         # Await clients' responses and type-check them.
         replies = await self.netwk.wait_for_messages(clients)
         results = {}  # type: Dict[str, MessageT]
         errors = {}  # type: Dict[str, str]
-        for client, message in replies.items():
-            if isinstance(message, msgtype):
-                results[client] = message
-            elif isinstance(message, messaging.Error):
-                errors[client] = f"{context} failed: {message.message}"
+        for client, reply in replies.items():
+            if issubclass(reply.message_cls, msgtype):
+                results[client] = reply.deserialize()
+            elif issubclass(reply.message_cls, messaging.Error):
+                err_msg = reply.deserialize().message
+                errors[client] = f"{context} failed: {err_msg}"
             else:
-                errors[client] = f"Unexpected message: {message}"
+                errors[client] = f"Unexpected message: {reply.message_cls}"
         # If any client has failed to send proper results, raise.
         # future: modularize errors-handling behaviour
         if errors:
             err_msg = f"{context} failed for another client."
             messages = {
                 client: messaging.CancelTraining(errors.get(client, err_msg))
                 for client in self.netwk.client_names
@@ -383,15 +398,15 @@
             **dataclasses.asdict(config.privacy),
         }  # type: Dict[str, Any]
         message = messaging.PrivacyRequest(**params)
         await self.netwk.broadcast_message(message)
         self.logger.info("Waiting for clients' responses.")
         await self._collect_results(
             clients=self.netwk.client_names,
-            msgtype=messaging.GenericMessage,
+            msgtype=messaging.PrivacyReply,
             context="Privacy initialization",
         )
         self.logger.info("Privacy requests were processed by clients.")
 
     async def training_round(
         self,
         round_i: int,
@@ -437,55 +452,80 @@
             Names of the clients participating in the training round.
         round_i: int
             Index of the training round.
         train_cfg: TrainingConfig
             TrainingConfig dataclass instance wrapping data-batching
             and computational effort constraints hyper-parameters.
         """
-        # Set up shared training parameters.
-        params = {
-            "round_i": round_i,
-            "weights": self.model.get_weights(trainable=True),
+        # Set up the base training request.
+        msg_light = messaging.TrainRequest(
+            round_i=round_i,
+            weights=None,
+            aux_var=self.optim.collect_aux_var(),
             **train_cfg.message_params,
-        }  # type: Dict[str, Any]
-        messages = {}  # type: Dict[str, messaging.Message]
-        # Dispatch auxiliary variables (which may be client-specific).
-        aux_var = self.optim.collect_aux_var()
-        for client in clients:
-            params["aux_var"] = {
-                key: val.get(client, val) for key, val in aux_var.items()
+        )
+        # Send it to clients, sparingly joining model weights.
+        await self._send_request_with_optional_weights(msg_light, clients)
+
+    async def _send_request_with_optional_weights(
+        self,
+        msg_light: Union[messaging.TrainRequest, messaging.EvaluationRequest],
+        clients: Set[str],
+    ) -> None:
+        """Send a request to clients, sparingly adding model weights to it.
+
+        Transmit the input message to all clients, adding a copy of the
+        global model weights for clients that do not already hold them.
+
+        Parameters
+        ----------
+        msg_light:
+            Message to send, with a 'weights' field left to None.
+        clients:
+            Name of the clients to whom the message is adressed.
+        """
+        # Identify clients that do not already hold latest model weights.
+        needs_weights = clients.difference(self._clients_holding_latest_model)
+        # If any client does not hold latest weights, ensure they get it.
+        if needs_weights:
+            msg_heavy = copy.copy(msg_light)
+            msg_heavy.weights = self.model.get_weights(trainable=True)
+            messages = {
+                client: msg_heavy if client in needs_weights else msg_light
+                for client in clients
             }
-            messages[client] = messaging.TrainRequest(**params)
-        # Send client-wise messages.
-        await self.netwk.send_messages(messages)
+            await self.netwk.send_messages(messages)
+            self._clients_holding_latest_model.update(needs_weights)
+        # If no client requires weights, do not even access them.
+        else:
+            await self.netwk.broadcast_message(msg_light, clients)
 
     def _conduct_global_update(
         self,
         results: Dict[str, messaging.TrainReply],
     ) -> None:
         """Use training results from clients to update the global model.
 
         Parameters
         ----------
         results: dict[str, TrainReply]
             Client-wise TrainReply message sent after a training round.
         """
-        # Reformat received auxiliary variables and pass them to the Optimizer.
-        aux_var = {}  # type: Dict[str, Dict[str, Dict[str, Any]]]
-        for client, result in results.items():
-            for module, params in result.aux_var.items():
-                aux_var.setdefault(module, {})[client] = params
+        # Unpack, aggregate and finally process optimizer auxiliary variables.
+        aux_var = {}  # type: Dict[str, AuxVar]
+        for msg in results.values():
+            for key, aux in msg.aux_var.items():
+                aux_var[key] = aux_var.get(key, 0) + aux
         self.optim.process_aux_var(aux_var)
         # Compute aggregated "gradients" (updates) and apply them to the model.
-        # revise: pass n_epoch / t_spent / ?
-        gradients = self.aggrg.aggregate(
-            {client: result.updates for client, result in results.items()},
-            {client: result.n_steps for client, result in results.items()},
-        )
+        updates = sum(msg.updates for msg in results.values())
+        gradients = self.aggrg.finalize_updates(updates)
         self.optim.apply_gradients(self.model, gradients)
+        # Record that no clients hold the updated model.
+        self._clients_holding_latest_model.clear()
 
     async def evaluation_round(
         self,
         round_i: int,
         valid_cfg: EvaluateConfig,
     ) -> None:
         """Orchestrate an evaluation round.
@@ -543,20 +583,22 @@
             Names of the clients participating in the evaluation round.
         round_i: int
             Index of the evaluation round.
         valid_cfg: EvaluateConfig
             EvaluateConfig dataclass instance wrapping data-batching
             and computational effort constraints hyper-parameters.
         """
-        message = messaging.EvaluationRequest(
+        # Set up the base evaluation request.
+        msg_light = messaging.EvaluationRequest(
             round_i=round_i,
-            weights=self.model.get_weights(trainable=True),
+            weights=None,
             **valid_cfg.message_params,
         )
-        await self.netwk.broadcast_message(message, clients)
+        # Send it to clients, sparingly joining model weights.
+        await self._send_request_with_optional_weights(msg_light, clients)
 
     def _aggregate_evaluation_results(
         self,
         results: Dict[str, messaging.EvaluationReply],
     ) -> Tuple[float, Dict[str, Union[float, np.ndarray]]]:
         """Aggregate evaluation results from clients into a global loss.
 
@@ -573,32 +615,37 @@
         metrics: dict[str, (float | np.ndarray)]
             The aggregated evaluation metrics computes from clients' ones.
         """
         # Reset the local MetricSet and set up ad hoc variables for the loss.
         loss = 0.0
         dvsr = 0.0
         self.metrics.reset()
+        agg_states = self.metrics.get_states()
         # Iteratively update the MetricSet and loss floats based on results.
         for client, reply in results.items():
             # Case when the client reported some metrics.
             if reply.metrics:
                 states = reply.metrics.copy()
-                # Update the global metrics based on the local ones.
+                # Deal with loss metric's aggregation.
                 s_loss = states.pop("loss")
-                loss += s_loss["current"]  # type: ignore
-                dvsr += s_loss["divisor"]  # type: ignore
-                self.metrics.agg_states(states)
+                assert isinstance(s_loss, MeanState)
+                loss += s_loss.num_sum
+                dvsr += s_loss.divisor
+                # Aggregate other metrics.
+                for key, val in states.items():
+                    agg_states[key] += val
             # Case when the client only reported the aggregated local loss.
             else:
                 self.logger.info(
                     "Client %s refused to share their local metrics.", client
                 )
                 loss += reply.loss
                 dvsr += reply.n_steps
         # Compute the final results.
+        self.metrics.set_states(agg_states)
         metrics = self.metrics.get_result()
         loss = loss / dvsr
         return loss, metrics
 
     def _checkpoint_after_evaluation(
         self,
         metrics: Dict[str, Union[float, np.ndarray]],
@@ -624,24 +671,21 @@
             )
         # Checkpoint the model, optimizer and global evaluation metrics.
         timestamp = self.ckptr.checkpoint(
             model=self.model, optimizer=self.optim, metrics=metrics
         )
         # Checkpoint the client-wise metrics (or at least their loss).
         # Use the same timestamp label as for global metrics and states.
-        local = MetricSet.from_config(self.metrics.get_config())
         for client, reply in results.items():
+            metrics = {"loss": reply.loss}
             if reply.metrics:
-                local.reset()
-                local.agg_states(reply.metrics)
-                metrics = local.get_result()
-            else:
-                metrics = {"loss": reply.loss}
+                self.metrics.set_states(reply.metrics)
+                metrics.update(self.metrics.get_result())
             self.ckptr.save_metrics(
-                metrics=local.get_result(),
+                metrics=metrics,
                 prefix=f"metrics_{client}",
                 append=bool(self._loss),
                 timestamp=timestamp,
             )
 
     def _keep_training(
         self,
```

### Comparing `declearn-2.3.2/declearn/main/config/__init__.py` & `declearn-2.4.0/declearn/main/config/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/main/config/_dataclasses.py` & `declearn-2.4.0/declearn/main/config/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/main/config/_run_config.py` & `declearn-2.4.0/declearn/main/config/_run_config.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/main/config/_strategy.py` & `declearn-2.4.0/declearn/main/config/_strategy.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/main/privacy/__init__.py` & `declearn-2.4.0/declearn/main/privacy/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/main/privacy/_dp_trainer.py` & `declearn-2.4.0/declearn/main/privacy/_dp_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import logging
 from typing import List, Optional, Tuple, Union
 
 from opacus.accountants import IAccountant, create_accountant  # type: ignore
 from opacus.accountants.utils import get_noise_multiplier  # type: ignore
 
+from declearn.aggregator import Aggregator
 from declearn.communication import messaging
 from declearn.dataset import Dataset
 from declearn.main.utils import TrainingManager
 from declearn.metrics import MetricInputType, MetricSet
 from declearn.model.api import Model
 from declearn.optimizer import Optimizer
 from declearn.optimizer.modules import GaussianNoiseModule
@@ -64,21 +65,32 @@
         https://arxiv.org/abs/1607.00133
     """
 
     def __init__(
         self,
         model: Model,
         optim: Optimizer,
+        aggrg: Aggregator,
         train_data: Dataset,
         valid_data: Optional[Dataset] = None,
         metrics: Union[MetricSet, List[MetricInputType], None] = None,
         logger: Union[logging.Logger, str, None] = None,
+        verbose: bool = True,
     ) -> None:
         # inherited signature; pylint: disable=too-many-arguments
-        super().__init__(model, optim, train_data, valid_data, metrics, logger)
+        super().__init__(
+            model=model,
+            optim=optim,
+            aggrg=aggrg,
+            train_data=train_data,
+            valid_data=valid_data,
+            metrics=metrics,
+            logger=logger,
+            verbose=verbose,
+        )
         # Add DP-related fields: accountant, clipping norm and budget.
         self.accountant = None  # type: Optional[IAccountant]
         self.sclip_norm = None  # type: Optional[float]
         self._dp_budget = (0.0, 0.0)
         self._dp_states = None  # type: Optional[Tuple[float, float]]
 
     def make_private(
```

### Comparing `declearn-2.3.2/declearn/main/utils/__init__.py` & `declearn-2.4.0/declearn/main/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/main/utils/_checkpoint.py` & `declearn-2.4.0/declearn/main/utils/_checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import json
 import os
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
-import pandas as pd  # type: ignore
+import pandas as pd
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.model.api import Model
 from declearn.optimizer import Optimizer
 from declearn.utils import (
     deserialize_object,
     json_dump,
@@ -315,24 +315,25 @@
             timestamp = datetime.now().strftime("%y-%m-%d_%H-%M-%S")
         scores = {
             key: val.tolist() if isinstance(val, np.ndarray) else float(val)
             for key, val in metrics.items()
         }
         # Filter out scalar metrics and write them to a csv file.
         scalars = {k: v for k, v in scores.items() if isinstance(v, float)}
-        fpath = os.path.join(self.folder, f"{prefix}.csv")
-        pd.DataFrame(scalars, index=[timestamp]).to_csv(
-            fpath,
-            sep=",",
-            mode=("a" if append else "w"),
-            header=not (append and os.path.isfile(fpath)),
-            index=True,
-            index_label="timestamp",
-            encoding="utf-8",
-        )
+        if scalars:
+            fpath = os.path.join(self.folder, f"{prefix}.csv")
+            pd.DataFrame(scalars, index=[timestamp]).to_csv(
+                fpath,
+                sep=",",
+                mode=("a" if append else "w"),
+                header=not (append and os.path.isfile(fpath)),
+                index=True,
+                index_label="timestamp",
+                encoding="utf-8",
+            )
         # Write the full set of metrics to a JSON file.
         jdump = json.dumps({timestamp: scores})[1:-1]  # bracket-less dict
         fpath = os.path.join(self.folder, f"{prefix}.json")
         mode = "a" if append and os.path.isfile(fpath) else "w"
         with open(fpath, mode=mode, encoding="utf-8") as file:
             # First time, initialize the json file as a dict.
             if mode == "w":
```

### Comparing `declearn-2.3.2/declearn/main/utils/_constraints.py` & `declearn-2.4.0/declearn/main/utils/_constraints.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/main/utils/_data_info.py` & `declearn-2.4.0/declearn/main/utils/_data_info.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/main/utils/_early_stop.py` & `declearn-2.4.0/declearn/main/utils/_early_stop.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/main/utils/_training.py` & `declearn-2.4.0/declearn/main/utils/_training.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,80 +14,97 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Wrapper to run local training and evaluation rounds in a FL process."""
 
 import logging
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
+import tqdm
 
+from declearn.aggregator import Aggregator
 from declearn.communication import messaging
 from declearn.dataset import Dataset
 from declearn.main.utils._constraints import (
     Constraint,
     ConstraintSet,
     TimeoutConstraint,
 )
-from declearn.metrics import MeanMetric, Metric, MetricInputType, MetricSet
+from declearn.metrics import (
+    # fmt: off
+    MeanMetric, Metric, MetricInputType, MetricSet, MetricState
+)
 from declearn.model.api import Model
 from declearn.optimizer import Optimizer
 from declearn.typing import Batch
 from declearn.utils import LOGGING_LEVEL_MAJOR, get_logger
 
 __all__ = [
     "TrainingManager",
 ]
 
 
 class TrainingManager:
     """Class wrapping the logic for local training and evaluation rounds."""
 
+    # one too-many attribute; pylint: disable=too-many-instance-attributes
+
     def __init__(
         self,
         model: Model,
         optim: Optimizer,
+        aggrg: Aggregator,
         train_data: Dataset,
         valid_data: Optional[Dataset] = None,
         metrics: Union[MetricSet, List[MetricInputType], None] = None,
         logger: Union[logging.Logger, str, None] = None,
+        verbose: bool = True,
     ) -> None:
         """Instantiate the client-side training and evaluation process.
 
         Parameters
         ----------
         model: Model
             Model instance that needs training and/or evaluating.
         optim: Optimizer
             Optimizer instance that orchestrates training steps.
+        aggrg: Aggregator
+            Aggregator instance that is used to derive global model
+            updates from peer-wise local ones.
         train_data: Dataset
             Dataset instance wrapping the local training dataset.
         valid_data: Dataset or None, default=None
             Dataset instance wrapping the local validation dataset.
             If None, use `train_data` in the evaluation rounds.
         metrics: MetricSet or list[MetricInputType] or None, default=None
             MetricSet instance or list of Metric instances and/or specs
             to wrap into one, defining evaluation metrics to compute in
             addition to the model's loss.
             If None, only compute and report the model's loss.
         logger: logging.Logger or str or None, default=None,
             Logger to use, or name of a logger to set up with
             `declearn.utils.get_logger`.
             If None, use `type(self).__name__`.
+        verbose: bool, default=True
+            Whether to display progress bars when running training
+            and validation rounds.
         """
         # arguments serve modularity; pylint: disable=too-many-arguments
         self.model = model
         self.optim = optim
+        self.aggrg = aggrg
         self.train_data = train_data
         self.valid_data = valid_data
         self.metrics = self._prepare_metrics(metrics)
         if not isinstance(logger, logging.Logger):
             logger = get_logger(logger or f"{type(self).__name__}")
         self.logger = logger
+        self.verbose = verbose
 
     def _prepare_metrics(
         self,
         metrics: Union[MetricSet, List[MetricInputType], None],
     ) -> MetricSet:
         """Parse the `metrics` instantiation inputs into a MetricSet."""
         # Type-check and/or transform the inputs into a MetricSet instance.
@@ -108,15 +125,15 @@
         """Return an ad-hoc Metric object to compute the model's loss."""
         loss_fn = self.model.loss_function
 
         # Write a custom, unregistered Metric subclass.
         class LossMetric(MeanMetric, register=False):
             """Ad hoc Metric wrapping a model's loss function."""
 
-            name: ClassVar[str] = "loss"
+            name = "loss"
 
             def metric_func(
                 self, y_true: np.ndarray, y_pred: np.ndarray
             ) -> np.ndarray:
                 return loss_fn(y_true, y_pred)
 
         # Instantiate and return the ad-hoc loss metric.
@@ -156,49 +173,63 @@
     def _training_round(
         self,
         message: messaging.TrainRequest,
     ) -> messaging.TrainReply:
         """Backend to `training_round`, without exception capture hooks."""
         # Unpack and apply model weights and optimizer auxiliary variables.
         self.logger.info("Applying server updates to local objects.")
-        self.model.set_weights(message.weights, trainable=True)
+        if message.weights is None:
+            start_weights = self.model.get_weights(trainable=True)
+        else:
+            start_weights = message.weights
+            self.model.set_weights(start_weights, trainable=True)
         self.optim.process_aux_var(message.aux_var)
         self.optim.start_round()  # trigger loss regularizer's `on_round_start`
         # Train under instructed effort constraints.
         params = message.n_epoch, message.n_steps, message.timeout
         self.logger.info(
             "Training local model for %s epochs | %s steps | %s seconds.",
             *params,
         )
-        effort = self._train_under_constraints(message.batches, *params)
-        # Compute model updates and collect auxiliary variables.
+        effort = self.train_under_constraints(message.batches, *params)
+        # Compute and preprocess model updates and collect auxiliary variables.
         self.logger.info("Packing local updates to be sent to the server.")
+        updates = self.aggrg.prepare_for_sharing(
+            updates=start_weights - self.model.get_weights(trainable=True),
+            n_steps=int(effort["n_steps"]),
+        )
+        aux_var = self.optim.collect_aux_var()
+        # Wrap them as a TrainReply together with effort metadata and return.
         return messaging.TrainReply(
-            updates=message.weights - self.model.get_weights(trainable=True),
-            aux_var=self.optim.collect_aux_var(),
+            updates=updates,
+            aux_var=aux_var,
             n_epoch=int(effort["n_epoch"]),
             n_steps=int(effort["n_steps"]),
             t_spent=round(effort["t_spent"], 3),
         )
 
-    def _train_under_constraints(
+    def train_under_constraints(
         self,
         batch_cfg: Dict[str, Any],
-        n_epoch: Optional[int],
-        n_steps: Optional[int],
-        timeout: Optional[int],
+        n_epoch: Optional[int] = 1,
+        n_steps: Optional[int] = None,
+        timeout: Optional[int] = None,
     ) -> Dict[str, float]:
-        """Backend code to run local SGD steps under effort constraints.
+        """Run local SGD steps under effort constraints.
+
+        This is the core backend to the `training_round` method,
+        which further handles message parsing and passing, as well
+        as exception catching.
 
         Parameters
         ----------
         batch_cfg: Dict[str, Any]
             Keyword arguments for `self.train_data.generate_batches`
             i.e. specifications of batches used in local SGD steps.
-        n_epoch: int or None, default=None
+        n_epoch: int or None, default=1
             Maximum number of local training epochs to perform.
             May be overridden by `n_steps` or `timeout`.
         n_steps: int or None, default=None
             Maximum number of local training steps to perform.
             May be overridden by `n_epoch` or `timeout`.
         timeout: int or None, default=None
             Time (in seconds) beyond which to interrupt training,
@@ -220,22 +251,26 @@
         epochs = Constraint(limit=n_epoch, name="n_epoch")
         constraints = ConstraintSet(
             Constraint(limit=n_steps, name="n_steps"),
             TimeoutConstraint(limit=timeout, name="t_spent"),
         )
         # Run batch train steps for as long as constraints allow it.
         stop_training = False
+        if self.verbose:
+            progress_bar = tqdm.tqdm(desc="Training round", unit=" steps")
         while not (stop_training or epochs.saturated):
             for batch in self.train_data.generate_batches(**batch_cfg):
                 try:
                     self._run_train_step(batch)
                 except StopIteration as exc:
                     self.logger.warning("Interrupting training round: %s", exc)
                     stop_training = True
                     break
+                if self.verbose:
+                    progress_bar.update()
                 constraints.increment()
                 if constraints.saturated:
                     stop_training = True
                     break
             epochs.increment()
         # Return a dict storing information on the training effort.
         effort = {"n_epoch": epochs.value}
@@ -282,78 +317,110 @@
             error raised during it.
         """
         self.logger.info(
             "Participating in evaluation round %s", message.round_i
         )
         # Try running the evaluation round.
         try:
-            # Update the model's weights and evaluate on the local dataset.
-            # Revise: make the weights' update optional.
-            self.model.set_weights(message.weights, trainable=True)
-            return self._evaluate_under_constraints(
-                message.batches, message.n_steps, message.timeout
-            )
+            return self._evaluation_round(message)
         # In case of failure, wrap the exception as an Error message.
         except Exception as exception:  # pylint: disable=broad-except
             self.logger.error(
                 "Error encountered during evaluation: %s.", exception
             )
             return messaging.Error(repr(exception))
 
-    def _evaluate_under_constraints(
+    def _evaluation_round(
+        self,
+        message: messaging.EvaluationRequest,
+    ) -> messaging.EvaluationReply:
+        """Backend to `evaluation_round`, without exception capture hooks."""
+        # Update the model's weights and evaluate on the local dataset.
+        if message.weights is not None:
+            self.model.set_weights(message.weights, trainable=True)
+        metrics, states, effort = self.evaluate_under_constraints(
+            message.batches, message.n_steps, message.timeout
+        )
+        # Pack the resulting information into a message.
+        self.logger.info("Packing local results to be sent to the server.")
+        return messaging.EvaluationReply(
+            loss=float(metrics["loss"]),
+            metrics=states,
+            n_steps=int(effort["n_steps"]),
+            t_spent=round(effort["t_spent"], 3),
+        )
+
+    def evaluate_under_constraints(
         self,
         batch_cfg: Dict[str, Any],
         n_steps: Optional[int] = None,
         timeout: Optional[int] = None,
-    ) -> messaging.EvaluationReply:
-        """Backend code to run local loss computation under effort constraints.
+    ) -> Tuple[
+        Dict[str, Union[float, np.ndarray]],
+        Dict[str, MetricState],
+        Dict[str, float],
+    ]:
+        """Run local loss computation under effort constraints.
+
+        This is the core backend to the `evaluation_round` method,
+        which further handles message parsing and passing, as well
+        as exception catching.
 
         Parameters
         ----------
         batch_cfg: Dict[str, Any]
             Keyword arguments to `self.valid_data.generate_batches`.
         n_steps: int or None, default=None
             Maximum number of local evaluation steps to perform.
             May be overridden by `timeout` or dataset size.
         timeout: int or None, default=None
             Time (in seconds) beyond which to interrupt evaluation,
             regardless of the actual number of steps taken (> 0).
 
         Returns
         -------
-        reply: messaging.EvaluationReply
-            EvaluationReply message wrapping the computed loss on the
-            local validation (or, if absent, training) dataset as well
-            as the number of steps and the time taken to obtain it.
+        metrics:
+            Computed metrics, as a dict with float or array values.
+        states:
+            Computed metrics, as partial values that may be shared
+            with other agents to federatively compute final values
+            with the same specs as `metrics`.
+        effort:
+            Dictionary storing information on the computational
+            effort effectively performed:
+            * n_epoch: int
+                Number of evaluation epochs completed.
+            * n_steps: int
+                Number of evaluation steps completed.
+            * t_spent: float
+                Time spent running training steps (in seconds).
         """
         # Set up effort constraints under which to operate.
         constraints = ConstraintSet(
             Constraint(limit=n_steps, name="n_steps"),
             TimeoutConstraint(limit=timeout, name="t_spent"),
         )
         # Ensure evaluation metrics start from their base state.
         self.metrics.reset()
         # Run batch evaluation steps for as long as constraints allow it.
         dataset = self.valid_data or self.train_data
+        if self.verbose:
+            progress_bar = tqdm.tqdm(desc="Evaluation round", unit=" batches")
         for batch in dataset.generate_batches(**batch_cfg):
             inputs = self.model.compute_batch_predictions(batch)
             self.metrics.update(*inputs)
+            if self.verbose:
+                progress_bar.update()
             constraints.increment()
             if constraints.saturated:
                 break
         # Gather the computed metrics and computational effort information.
         effort = constraints.get_values()
-        result = self.metrics.get_result()
+        values = self.metrics.get_result()
         states = self.metrics.get_states()
         self.logger.log(
             LOGGING_LEVEL_MAJOR,
             "Local scalar evaluation metrics: %s",
-            {k: v for k, v in result.items() if isinstance(v, float)},
-        )
-        # Pack the result and computational effort information into a message.
-        self.logger.info("Packing local results to be sent to the server.")
-        return messaging.EvaluationReply(
-            loss=float(result["loss"]),
-            metrics=states,
-            n_steps=int(effort["n_steps"]),
-            t_spent=round(effort["t_spent"], 3),
+            {k: v for k, v in values.items() if isinstance(v, float)},
         )
+        # Return the metrics' values, their states and the effort information.
+        return values, states, effort
```

### Comparing `declearn-2.3.2/declearn/metrics/__init__.py` & `declearn-2.4.0/declearn/metrics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 an API to iteratively and/or federatively compute evaluation metrics,
 as well as a number of concrete standard machine learning metrics.
 
 Abstractions
 ------------
 * [Metric][declearn.metrics.Metric]:
     Abstract base class defining an API for metrics' computation.
+* [MetricState][declearn.metrics.MetricState]:
+    Abstract base class for Metrics intermediate aggregatable states.
 * [MeanMetric][declearn.metrics.MeanMetric]:
     Abstract class that defines a template for simple scores' averaging.
 
 Utils
 -----
 * [MetricSet][declearn.metrics.MetricSet]:
     Wrapper to bind together an ensemble of Metric instances.
@@ -60,15 +62,15 @@
     Identifier name: "mse".
 * [RSquared][declearn.metrics.RSquared]:
     R^2 (R-Squared, coefficient of determination) regression metric.
     Identifier name: "r2".
 
 """
 
-from ._api import Metric
+from ._api import Metric, MetricState
 from ._classif import (
     BinaryAccuracyPrecisionRecall,
     MulticlassAccuracyPrecisionRecall,
 )
 from ._mean import MeanMetric, MeanAbsoluteError, MeanSquaredError
 from ._roc_auc import BinaryRocAUC
 from ._rsquared import RSquared
```

### Comparing `declearn-2.3.2/declearn/metrics/_api.py` & `declearn-2.4.0/declearn/metrics/_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,35 +13,62 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Iterative and federative evaluation metrics base class."""
 
+import abc
 import warnings
-from abc import ABCMeta, abstractmethod
 from copy import deepcopy
-from typing import Any, ClassVar, Dict, Optional, Union
+from typing import Any, ClassVar, Dict, Generic, Optional, Type, TypeVar, Union
 
 import numpy as np
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.utils import (
+    Aggregate,
     access_registered,
     create_types_registry,
     register_type,
 )
 
 __all__ = [
     "Metric",
+    "MetricState",
 ]
 
 
+class MetricState(
+    Aggregate, base_cls=True, register=False, metaclass=abc.ABCMeta
+):
+    """Abstract base class for Metrics intermediate aggregatable states.
+
+    Each and every `Metric` subclass is expected to be coupled with one
+    (or multiple) `MetricState` subtypes, which are used to exchange and
+    aggregate partial results across a network of peers, which can in the
+    end be passed to a single `Metric` instance for metrics' finalization.
+
+    This class also defines whether contents are compatible with secure
+    aggregation, and whether some fields should remain in cleartext no
+    matter what.
+
+    Note that subclasses are automatically type-registered, and should be
+    decorated as `dataclasses.dataclass`. To prevent registration, simply
+    pass `register=False` at inheritance.
+    """
+
+    _group_key = "MetricState"
+
+
+MetricStateT = TypeVar("MetricStateT", bound=MetricState)
+
+
 @create_types_registry(name="Metric")
-class Metric(metaclass=ABCMeta):
+class Metric(Generic[MetricStateT], metaclass=abc.ABCMeta):
     """Abstract class defining an API to compute federative metrics.
 
     This class defines an API to instantiate stateful containers
     for one or multiple metrics, that enable computing the final
     results through iterative update steps that may additionally
     be run in a federative way.
 
@@ -59,59 +86,52 @@
     ```
     >>> # Instantiate 2+ metrics and run local update steps.
     >>> metric_0 = MetricSubclass()
     >>> metric_1 = MetricSubclass()
     >>> metric_0.udpate(y_true_0, y_pred_0)
     >>> metric_1.update(y_true_1, y_pred_1)
     >>> # Gather and share metric states (aggregated information).
-    >>> states_0 = metric_0.get_states()  # metrics_0 is unaltered
-    >>> metric_1.agg_states(states_0)     # metrics_1 is updated
+    >>> states_0 = metric_0.get_states()  # metric_0 is unaltered
+    >>> states_1 = metric_1.get_states()  # metric_1 is unaltered
     >>> # Compute results that aggregate info from both clients.
-    >>> metric_1.get_result()
+    >>> states = states_0 + states_1
+    >>> metric_0.set_states(states)  # would work the same with metrics_1
+    >>> metric_0.get_result()
     ```
 
     Abstract
     --------
     To define a concrete Metric, one must subclass it and define:
 
     - name: str class attribute
         Name identifier of the class (should be unique across existing
         Metric classes). Also used for automatic types-registration of
         the class (see `Inheritance` section below).
-    - _build_states() -> dict[str, (float | np.ndarray)]:
-        Build and return an ensemble of state variables.
+    - build_initial_states() -> MetricState:
+        Return the initial states for this Metric instance.
         This method is called to initialize the `_states` attribute,
         that should be used and updated by other abstract methods.
     - update(y_true: np.ndarray, y_pred: np.ndarray, s_wght: np.ndarray|None):
         Update the metric's internal state based on a data batch.
         This method should update `self._states` in-place.
     - get_result() -> dict[str, (float | np.ndarray)]:
         Compute the metric(s), based on the current state variables.
         This method should make use of `self._states` and prevent
         side effects on its contents.
 
     Overridable
     -----------
-    Some methods may be overridden based on the concrete Metric's needs.
-    The most imporant one is the states-aggregation method:
-
-    - agg_states(states: dict[str, (float | np.ndarray)]:
-        Aggregate provided state variables into self ones.
-        By default, it expects input and internal states to have
-        similar specifications, and aggregates them by summation,
-        which might no be proper depending on the actual metric.
-
-    A pair of methods may be extended to cover non-`self._states`-contained
-    variables:
+    Some methods may be overridden based on the concrete Metric's needs:
 
     - reset():
         Reset the metric to its initial state.
-    - get_states() -> dict[str, (float | np.ndarray)]:
+    - get_states() -> MetricState:
         Return a copy of the current state variables.
-
+    - set_states(MetricState):
+        Replace current state variables with a copy of inputs.
 
     Finally, depending on the hyper-parameters defined by the subclass's
     `__init__`, one should adjust JSON-configuration-interfacing methods:
 
     - get_config() -> dict[str, any]:
         Return a JSON-serializable configuration dict for this Metric.
     - from_config(config: dict[str, any]) -> Self:
@@ -123,58 +143,52 @@
     registered under the "Metric" group using its class-attribute `name`.
     This can be prevented by adding `register=False` to the inheritance specs
     (e.g. `class MyCls(Metric, register=False)`).
 
     See `declearn.utils.register_type` for details on types registration.
     """
 
-    name: ClassVar[str] = NotImplemented
+    name: ClassVar[str]
     """Name identifier of the class, unique across Metric classes."""
 
+    state_cls: ClassVar[Type[MetricState]]
+    """Type of 'MetricState' data structure used by this 'Metric' class."""
+
     def __init__(
         self,
     ) -> None:
         """Instantiate the metric object."""
-        self._states = self._build_states()
+        self._states = self.build_initial_states()
 
-    @abstractmethod
-    def _build_states(
+    @abc.abstractmethod
+    def build_initial_states(
         self,
-    ) -> Dict[str, Union[float, np.ndarray]]:
-        """Build and return an ensemble of state variables.
-
-        The state variables stored in this dict are (by default)
-        sharable with other instances of this metric and may be
-        combined with the latter's through summation in order to
-        compute final metrics in a federated way.
-
-        Note that the update process may be altered by extending
-        or overridding the `agg_states` method.
+    ) -> MetricStateT:
+        """Return the initial states for this Metric instance.
 
         Returns
         -------
-        states: dict[str, float or numpy.ndarray]
-            Dict of initial states that are to be assigned as
-            `_states` private attribute.
+        states:
+            Initial internal states for this object, as a `MetricState`.
         """
 
-    @abstractmethod
+    @abc.abstractmethod
     def get_result(
         self,
     ) -> Dict[str, Union[float, np.ndarray]]:
-        """Compute the metric(s), based on the current state variables.
+        """Compute finalized metric(s), based on the current state variables.
 
         Returns
         -------
         results: dict[str, float or numpy.ndarray]
             Dict of named result metrics, that may either be
             unitary float scores or numpy arrays.
         """
 
-    @abstractmethod
+    @abc.abstractmethod
     def update(
         self,
         y_true: np.ndarray,
         y_pred: np.ndarray,
         s_wght: Optional[np.ndarray] = None,
     ) -> None:
         """Update the metric's internal state based on a data batch.
@@ -189,73 +203,94 @@
             Optional sample weights to take into account in scores.
         """
 
     def reset(
         self,
     ) -> None:
         """Reset the metric to its initial state."""
-        self._states = self._build_states()
+        self._states = self.build_initial_states()
 
     def get_states(
         self,
-    ) -> Dict[str, Union[float, np.ndarray]]:
+    ) -> MetricStateT:
         """Return a copy of the current state variables.
 
         This method is designed to expose and share partial results
         that may be aggregated with those of other instances of the
         same metric before computing overall results.
 
         Returns
         -------
-        states: dict[str, float or numpy.ndarray]
-            Dict of states that may be fed to another instance of
-            this class via its `agg_states` method.
+        states:
+            Copy of current states, as a `MetricState` instance.
         """
         return deepcopy(self._states)
 
+    def set_states(
+        self,
+        states: MetricStateT,
+    ) -> None:
+        """Replace internal states with a copy of incoming ones.
+
+        Parameters
+        ----------
+        states:
+            Replacement states, as a compatible `MetricState` instance.
+
+        Raises
+        ------
+        TypeError
+            If `states` is of improper type.
+        """
+        if not isinstance(states, self.state_cls):
+            raise TypeError(
+                f"'{self.__class__.__name__}.set_states' expected "
+                f"'{self.state_cls}' inputs, got '{type(states)}'."
+            )
+        self._states = deepcopy(states)  # type: ignore
+
     def agg_states(
         self,
-        states: Dict[str, Union[float, np.ndarray]],
+        states: MetricStateT,
     ) -> None:
         """Aggregate provided state variables into self ones.
 
+        This method is DEPRECATED as of DecLearn v2.4, in favor of
+        merely aggregating `MetricState` instances, using either
+        their `aggregate` method or the overloaded `+` operator.
+        It will be removed in DecLearn 2.6 and/or 3.0.
+
         This method is designed to aggregate results from multiple
         similar metrics objects into a single one before computing
         its results.
 
         Parameters
         ----------
-        states: dict[str, float or numpy.ndarray]
-            Dict of states emitted by another instance of this class
+        states:
+            `MetricState` emitted by another instance of this class
             via its `get_states` method.
 
         Raises
         ------
-        KeyError
-            If any state variable is missing from `states`.
         TypeError
-            If any state variable is of unproper type.
-        ValueError
-            If any array state variable is of unproper shape.
+            If `states` is of improper type.
         """
-        final = {}  # type: Dict[str, Union[float, np.ndarray]]
-        # Iteratively compute sum-aggregated states, running sanity checks.
-        for name, own in self._states.items():
-            if name not in states:
-                raise KeyError(f"Missing required state variable: '{name}'.")
-            oth = states[name]
-            if not isinstance(oth, type(own)):
-                raise TypeError(f"Input state '{name}' is of unproper type.")
-            if isinstance(own, np.ndarray):
-                if own.shape != oth.shape:  # type: ignore
-                    msg = f"Input state '{name}' is of unproper shape."
-                    raise ValueError(msg)
-            final[name] = own + oth
-        # Assign the sum-aggregated states.
-        self._states = final
+        warnings.warn(
+            "'Metric.agg_states' was deprecated in DecLearn v2.4, in favor "
+            "of aggregating 'MetricState' instances directly, and setting "
+            "final aggregated states using 'Metric.set_state'. It will be "
+            "removed in DecLearn 2.6 and/or 3.0.",
+            DeprecationWarning,
+        )
+        if not isinstance(states, self.state_cls):
+            raise TypeError(
+                f"'{self.__class__.__name__}.set_states' expected "
+                f"'{self.state_cls}' inputs, got '{type(states)}'."
+            )
+        self.set_states(self._states + states)
 
     def __init_subclass__(
         cls,
         register: bool = True,
         **kwargs: Any,
     ) -> None:
         """Automatically type-register Metric subclasses."""
@@ -341,32 +376,7 @@
         s_wght = s_wght.squeeze()
         if s_wght.shape != (n_samples,) or np.any(s_wght < 0):
             raise ValueError(
                 "Improper shape for 's_wght': should be a 1-d array "
                 "of sample-wise positive scalar weights."
             )
         return s_wght
-
-    @staticmethod
-    def normalize_weights(  # pragma: no cover
-        s_wght: np.ndarray,
-    ) -> np.ndarray:
-        """Utility method to ensure weights sum to one.
-
-        Note that this method may or may not be used depending on
-        the actual `Metric` considered, and is merely provided as
-        a utility to metric developers.
-        """
-        warn = DeprecationWarning(
-            "'Metric.normalize_weights' is unfit for the iterative "
-            "nature of the metric-computation process. It will be "
-            "removed from the Metric API in declearn v3.0."
-        )
-        warnings.warn(warn)
-        if s_wght.sum():
-            s_wght /= s_wght.sum()
-        else:
-            raise ValueError(
-                "Weights provided sum to zero, please provide only "
-                "positive weights with at least one non-zero weight."
-            )
-        return s_wght
```

### Comparing `declearn-2.3.2/declearn/metrics/_classif.py` & `declearn-2.4.0/declearn/metrics/_classif.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,29 +13,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Iterative and federative classification evaluation metrics."""
 
-from typing import Any, ClassVar, Collection, Dict, Optional, Union
+import dataclasses
+from typing import Any, Collection, Dict, Optional, Union
 
 import numpy as np
 import sklearn  # type: ignore
 import sklearn.metrics  # type: ignore
 
-from declearn.metrics._api import Metric
+from declearn.metrics._api import Metric, MetricState
+from declearn.metrics._utils import safe_division
 
 __all__ = [
     "BinaryAccuracyPrecisionRecall",
     "MulticlassAccuracyPrecisionRecall",
 ]
 
 
-class BinaryAccuracyPrecisionRecall(Metric):
+@dataclasses.dataclass
+class BinaryConfmat(MetricState):
+    """Binary confusion matrix 'MetricState'."""
+
+    tpos: float = 0.0
+    tneg: float = 0.0
+    fpos: float = 0.0
+    fneg: float = 0.0
+
+
+class BinaryAccuracyPrecisionRecall(Metric[BinaryConfmat]):
     """Binary classification accuracy, precision and recall metrics.
 
     This metric applies to binary classifier, and computes the (opt.
     weighted) amount of true positives (TP), true negatives (TN),
     false positives (FP) and false negatives (FN) predictions over
     time, from which basic evaluation metrics may be derived.
 
@@ -53,15 +65,16 @@
     * f-score: float
         F1-score, i.e. harmonic mean of precision and recall.
         Formula: (2*TP) / (2*TP + FP + FN)
     * confusion: 2-d numpy.ndarray
         Confusion matrix of predictions. Values: [[TN, FP], [FN, TP]]
     """
 
-    name: ClassVar[str] = "binary-classif"
+    name = "binary-classif"
+    state_cls = BinaryConfmat
 
     def __init__(
         self,
         thresh: float = 0.5,
         label: Union[int, str] = 1,
     ) -> None:
         """Instantiate the binary accuracy / precision / recall metrics.
@@ -73,62 +86,78 @@
         label: int or str, default=1
             Value of the positive labels in input true-label arrays.
         """
         self.thresh = thresh
         self.label = label
         super().__init__()
 
-    def get_config(self) -> Dict[str, Any]:
+    def get_config(
+        self,
+    ) -> Dict[str, Any]:
         return {"thresh": self.thresh, "label": self.label}
 
-    def _build_states(
+    def build_initial_states(
         self,
-    ) -> Dict[str, Union[float, np.ndarray]]:
-        return {"tpos": 0.0, "tneg": 0.0, "fpos": 0.0, "fneg": 0.0}
+    ) -> BinaryConfmat:
+        return BinaryConfmat()
 
     def get_result(
         self,
     ) -> Dict[str, Union[float, np.ndarray]]:
         # Unpack state variables for code readability.
-        tpos = self._states["tpos"]
-        tneg = self._states["tneg"]
-        fpos = self._states["fpos"]
-        fneg = self._states["fneg"]
-        # Compute metrics, avoiding division-by-zero errors.
-        if tpos != 0:
-            scores = {
-                "accuracy": (tpos + tneg) / (tpos + tneg + fpos + fneg),
-                "precision": tpos / (tpos + fpos),
-                "recall": tpos / (tpos + fneg),
-                "f-score": (tpos + tpos) / (tpos + tpos + fpos + fneg),
-            }
-        else:
-            scores = {
-                k: 0.0 for k in ("accuracy", "precision", "recall", "f-score")
-            }
+        tpos = self._states.tpos
+        tneg = self._states.tneg
+        fpos = self._states.fpos
+        fneg = self._states.fneg
+        # Compute metrics, catching division-by-zero errors (replace with 0.0).
+        scores = {
+            "accuracy": safe_division(tpos + tneg, tpos + tneg + fpos + fneg),
+            "precision": safe_division(tpos, tpos + fpos),
+            "recall": safe_division(tpos, tpos + fneg),
+            "f-score": safe_division(tpos + tpos, tpos + tpos + fpos + fneg),
+        }  # type: Dict[str, Union[float, np.ndarray]]
         # Add the confusion matrix and return.
         scores["confusion"] = np.array([[tneg, fpos], [fneg, tpos]])
         return scores
 
     def update(
         self,
         y_true: np.ndarray,
         y_pred: np.ndarray,
         s_wght: Optional[np.ndarray] = None,
     ) -> None:
         pos = y_true.flatten() == self.label
         tru = (y_pred.flatten() >= self.thresh) == pos
         s_wght = np.ones_like(tru) if s_wght is None else s_wght.flatten()
-        self._states["tpos"] += float(sum(s_wght * (tru & pos)))
-        self._states["tneg"] += float(sum(s_wght * (tru & ~pos)))
-        self._states["fpos"] += float(sum(s_wght * ~(tru | pos)))
-        self._states["fneg"] += float(sum(s_wght * (~tru & pos)))
+        self._states.tpos += float(sum(s_wght * (tru & pos)))
+        self._states.tneg += float(sum(s_wght * (tru & ~pos)))
+        self._states.fpos += float(sum(s_wght * ~(tru | pos)))
+        self._states.fneg += float(sum(s_wght * (~tru & pos)))
+
+
+@dataclasses.dataclass
+class ClassifConfmat(MetricState):
+    """Multiclass confusion matrix 'MetricState'."""
+
+    confmat: np.ndarray
+
+    @staticmethod
+    def aggregate_confmat(
+        val_a: np.ndarray,
+        val_b: np.ndarray,
+    ) -> np.ndarray:
+        """Aggregate two confusion matrix arrays."""
+        if val_a.shape != val_b.shape:
+            raise ValueError(
+                "Cannot aggregate confusion matrices with distinct shapes."
+            )
+        return val_a + val_b
 
 
-class MulticlassAccuracyPrecisionRecall(Metric):
+class MulticlassAccuracyPrecisionRecall(Metric[ClassifConfmat]):
     """Multiclass classification accuracy, precision and recall metrics.
 
     This metric assumes that the evaluated classifier emits a score for
     each and every predictable label, and that the predicted label is
     that with the highest score. Alternatively, pre-selected labels (or
     one-hot encodings) may be passed as predictions.
 
@@ -144,15 +173,16 @@
         Label-wise f1-score, i.e. harmonic mean of precision and recall.
     * confusion: 2-d numpy.ndarray
         Confusion matrix of predictions, where C[i, j] indicates the
         (opt. weighted) number of samples belonging to label i that
         were predicted to belong to label j.
     """
 
-    name: ClassVar[str] = "multi-classif"
+    name = "multi-classif"
+    state_cls = ClassifConfmat
 
     def __init__(
         self,
         labels: Collection[Union[int, str]],
     ) -> None:
         """Instantiate the multiclass accuracy/precision/recall metrics.
 
@@ -163,38 +193,39 @@
         """
         self.labels = np.array(list(labels))
         super().__init__()
 
     def get_config(self) -> Dict[str, Any]:
         return {"labels": self.labels.tolist()}
 
-    def _build_states(
+    def build_initial_states(
         self,
-    ) -> Dict[str, Union[float, np.ndarray]]:
-        return {"confm": np.zeros((len(self.labels), len(self.labels)))}
+    ) -> ClassifConfmat:
+        matrix = np.zeros((len(self.labels), len(self.labels)))
+        return ClassifConfmat(matrix)
 
     def get_result(
         self,
     ) -> Dict[str, Union[float, np.ndarray]]:
         # Compute the metrics, silencing division-by-zero errors.
-        confm = self._states["confm"]  # type: np.ndarray  # type: ignore
-        diag = np.diag(confm)  # label-wise true positives
-        pred = confm.sum(axis=0)  # label-wise number of predictions
-        true = confm.sum(axis=1)  # label-wise number of labels (support)
+        confmat = self._states.confmat
+        diag = np.diag(confmat)  # label-wise true positives
+        pred = confmat.sum(axis=0)  # label-wise number of predictions
+        true = confmat.sum(axis=1)  # label-wise number of labels (support)
         with np.errstate(invalid="ignore"):
             scores = {
-                "accuracy": diag.sum() / confm.sum(),
+                "accuracy": diag.sum() / confmat.sum(),
                 "precision": diag / pred,
                 "recall": diag / true,
                 "f-score": 2 * diag / (pred + true),
             }
         # Convert NaNs resulting from zero-division to zero.
         scores = {k: np.nan_to_num(v, copy=False) for k, v in scores.items()}
         # Add a copy of the confusion matrix and return.
-        scores["confusion"] = confm.copy()
+        scores["confusion"] = confmat.copy()
         return scores
 
     def update(
         self,
         y_true: np.ndarray,
         y_pred: np.ndarray,
         s_wght: Optional[np.ndarray] = None,
@@ -213,10 +244,10 @@
         s_wght: numpy.ndarray or None, default=None
             Optional sample weights to take into account in scores.
         """
         if y_pred.ndim == 2:
             y_pred = self.labels[y_pred.argmax(axis=1)]
         elif y_pred.ndim != 1:
             raise TypeError("Expected 1-d or 2-d y_pred array.")
-        self._states["confm"] += sklearn.metrics.confusion_matrix(
+        self._states.confmat += sklearn.metrics.confusion_matrix(
             y_true, y_pred, labels=self.labels, sample_weight=s_wght
         )
```

### Comparing `declearn-2.3.2/declearn/metrics/_mean.py` & `declearn-2.4.0/declearn/metrics/_mean.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,30 +13,39 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Iterative and federative generic evaluation metrics."""
 
-from abc import ABCMeta, abstractmethod
-from typing import ClassVar, Dict, Optional, Union
+import abc
+import dataclasses
+from typing import Dict, Optional, Union
 
 import numpy as np
 
-from declearn.metrics._api import Metric
+from declearn.metrics._api import Metric, MetricState
 from declearn.metrics._utils import squeeze_into_identical_shapes
 
 __all__ = [
     "MeanMetric",
     "MeanAbsoluteError",
     "MeanSquaredError",
 ]
 
 
-class MeanMetric(Metric, register=False, metaclass=ABCMeta):
+@dataclasses.dataclass
+class MeanState(MetricState):
+    """Generic 'MetricState' for average-based scalar metrics."""
+
+    num_sum: float = 0.0
+    divisor: float = 0.0
+
+
+class MeanMetric(Metric[MeanState], register=False, metaclass=abc.ABCMeta):
     """Generic mean-aggregation metric template.
 
     This abstract class implements a template for Metric classes
     that rely on computing a sample-wise score and its average
     across iterative inputs.
 
     Abstract
@@ -49,15 +58,22 @@
         based retrieval. Also used to label output results.
     - metric_func(y_true: np.ndarray, y_pred: np.ndarray) -> np.ndarray:
         Method that computes a score from the predictions and labels
         associated with a given batch, that is to be aggregated into
         an average metric across all input batches.
     """
 
-    @abstractmethod
+    state_cls = MeanState
+
+    def build_initial_states(
+        self,
+    ) -> MeanState:
+        return MeanState()
+
+    @abc.abstractmethod
     def metric_func(
         self,
         y_true: np.ndarray,
         y_pred: np.ndarray,
     ) -> np.ndarray:
         """Compute the sample-wise metric for a single batch.
 
@@ -74,41 +90,36 @@
 
         Returns
         -------
         scores: numpy.ndarray
             Sample-wise metric value.
         """
 
-    def _build_states(
-        self,
-    ) -> Dict[str, Union[float, np.ndarray]]:
-        return {"current": 0.0, "divisor": 0.0}
-
     def get_result(
         self,
     ) -> Dict[str, Union[float, np.ndarray]]:
-        if self._states["divisor"] == 0:
+        if self._states.divisor == 0:
             return {self.name: 0.0}
-        result = self._states["current"] / self._states["divisor"]
-        return {self.name: float(result)}
+        result = self._states.num_sum / self._states.divisor
+        return {self.name: result}
 
     def update(
         self,
         y_true: np.ndarray,
         y_pred: np.ndarray,
         s_wght: Optional[np.ndarray] = None,
     ) -> None:
         scores = self.metric_func(y_true, y_pred)
         if s_wght is None:
-            self._states["current"] += scores.sum()
-            self._states["divisor"] += len(y_pred)
+            self._states.num_sum += float(scores.sum())
+            self._states.divisor += len(y_pred)
         else:
             s_wght = self._prepare_sample_weights(s_wght, len(y_pred))
-            self._states["current"] += (s_wght * scores).sum()
-            self._states["divisor"] += np.sum(s_wght)
+            self._states.num_sum += float((s_wght * scores).sum())
+            self._states.divisor += float(np.sum(s_wght))
 
 
 class MeanAbsoluteError(MeanMetric):
     """Mean Absolute Error (MAE) metric.
 
     This metric applies to a regression model, and computes the (opt.
     weighted) mean sample-wise absolute error. Note that for inputs
@@ -118,15 +129,15 @@
     Computed metric is the following:
 
     * mae: float
         Mean absolute error, averaged across samples (possibly
         summed over channels for (>=2)-dimensional inputs).
     """
 
-    name: ClassVar[str] = "mae"
+    name = "mae"
 
     def metric_func(
         self,
         y_true: np.ndarray,
         y_pred: np.ndarray,
     ) -> np.ndarray:
         # Sample-wise (sum of) absolute error function.
@@ -148,15 +159,15 @@
     Computed metric is the following:
 
     * mse: float
         Mean squared error, averaged across samples (possibly
         summed over channels for (>=2)-dimensional inputs).
     """
 
-    name: ClassVar[str] = "mse"
+    name = "mse"
 
     def metric_func(
         self,
         y_true: np.ndarray,
         y_pred: np.ndarray,
     ) -> np.ndarray:
         # Sample-wise (sum of) squared error function.
```

### Comparing `declearn-2.3.2/declearn/metrics/_roc_auc.py` & `declearn-2.4.0/declearn/metrics/_roc_auc.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,28 +13,176 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Iterative and federative ROC AUC evaluation metrics."""
 
-from typing import Any, ClassVar, Dict, Optional, Tuple, Union
+import dataclasses
+from typing import Any, Dict, Optional, Tuple, Type, Union
 
 import numpy as np
 import sklearn  # type: ignore
 import sklearn.metrics  # type: ignore
+from typing_extensions import Self  # future: import from typing (py>= 3.11)
 
-from declearn.metrics._api import Metric
+from declearn.metrics._api import Metric, MetricState
 
 __all__ = [
     "BinaryRocAUC",
 ]
 
 
-class BinaryRocAUC(Metric):
+@dataclasses.dataclass
+class AurocState(MetricState):
+    """Dataclass for Binary AUROC metric states with fixed thresholds."""
+
+    tpos: np.ndarray
+    tneg: np.ndarray
+    fpos: np.ndarray
+    fneg: np.ndarray
+    thresh: np.ndarray
+
+    @staticmethod
+    def aggregate_thresh(
+        val_a: np.ndarray,
+        val_b: np.ndarray,
+    ) -> np.ndarray:
+        """Raise if thresholds differ, otherwise return them."""
+        if (len(val_a) != len(val_b)) or np.any(val_a != val_b):
+            raise ValueError(
+                "Cannot aggregate AUROC states with distinct thresholds. "
+                "To do so, use `AurocStateUnbound` containers."
+            )
+        return val_a
+
+    def prepare_for_secagg(
+        self,
+    ) -> Tuple[Dict[str, Any], Optional[Dict[str, Any]]]:
+        secagg = self.to_dict()
+        clrtxt = {"thresh": secagg.pop("thresh")}
+        return secagg, clrtxt
+
+
+@dataclasses.dataclass
+class AurocStateUnbound(AurocState):
+    """Dataclass for Binary AUROC metric states with adaptive thresholds."""
+
+    tpos: np.ndarray
+    tneg: np.ndarray
+    fpos: np.ndarray
+    fneg: np.ndarray
+    thresh: np.ndarray
+
+    def aggregate(
+        self,
+        other: Self,
+    ) -> Self:
+        """Aggregate two binary AUROC metric states."""
+        if not isinstance(other, AurocState):
+            raise TypeError(
+                f"'{self.__class__.__name__}.aggregate' expected a similar "
+                f"type instance as input, received '{type(other)}'."
+            )
+        # Case when both states have the same thresholds.
+        if (len(self.thresh) == len(other.thresh)) and np.all(
+            self.thresh == other.thresh
+        ):
+            return self.__class__(
+                tpos=self.tpos + other.tpos,
+                tneg=self.tneg + other.tneg,
+                fpos=self.fpos + other.fpos,
+                fneg=self.fneg + other.fneg,
+                thresh=self.thresh,
+            )
+        # Case when thresholds need to be combined and values interpolated.
+        thresh = np.union1d(self.thresh, other.thresh)
+        s_keys = ("tpos", "tneg", "fpos", "fneg")
+        states_a = self._interpolate_roc_states(
+            thresh_r=thresh,
+            thresh_p=self.thresh,
+            states_p={key: getattr(self, key) for key in s_keys},
+        )
+        states_b = self._interpolate_roc_states(
+            thresh_r=thresh,
+            thresh_p=other.thresh,
+            states_p={key: getattr(other, key) for key in s_keys},
+        )
+        states = {key: states_a[key] + states_b[key] for key in s_keys}
+        return self.__class__(**states, thresh=thresh)
+
+    @staticmethod
+    def _interpolate_roc_states(
+        thresh_r: np.ndarray,
+        thresh_p: np.ndarray,
+        states_p: Dict[str, np.ndarray],
+    ) -> Dict[str, np.ndarray]:
+        """Interpolate ROC states values to fit given thresholds.
+
+        Parameters
+        ----------
+        thresh_r: 1d-array
+            1-d array of unique and sorted reference thresholds.
+        thresh_p: 1d-array
+            1-d array of unique and sorted partial thresholds.
+            `thresh_p` must be a subset of `thresh_r`.
+        states_p: dict[str, 1d-array]
+            Dict of named 1-d arrays of state values, aligned on
+            `thresh_p` and monotonically increasing or decreasing.
+
+        Returns
+        -------
+        states_r: dict[str, 1d-array]
+            Dict of names 1-d arrays of interpolated state values,
+            aligned on `thresh_r`.
+        """
+        keys = {"tpos", "tneg", "fpos", "fneg"}.intersection(states_p)
+        states_r = {key: np.zeros_like(thresh_r) for key in keys}
+        max_p = len(thresh_p) - 1
+        idp = 0
+        for idr, thr in enumerate(thresh_r):
+            # Case when the threshold exists in the partial subset.
+            if thresh_p[idp] == thr:
+                for key in states_r:
+                    states_r[key][idr] = states_p[key][idp]
+                idp = min(idp + 1, max_p)
+            # Case when the threshold is below the subset's minimum.
+            elif idp == 0:
+                for key in states_r:
+                    states_r[key][idr] = states_p[key][idp]
+            # Case when the threshold is above the subset's maximum.
+            elif thresh_p[max_p] < thr:
+                for key in states_r:
+                    states_r[key][idr] = states_p[key][max_p]
+            # Case when the threshold-indexed values must be interpolated.
+            else:
+                t_inf = thresh_p[idp - 1]
+                t_sup = thresh_p[idp]
+                for key in states_r:
+                    v_inf = states_p[key][idp - 1]
+                    v_sup = states_p[key][idp]
+                    states_r[key][idr] = thr * (
+                        (v_sup - v_inf) / (t_sup - t_inf)
+                    )
+        # Return the interpolated states.
+        return states_r
+
+    def prepare_for_secagg(
+        self,
+    ) -> Tuple[Dict[str, Any], Optional[Dict[str, Any]]]:
+        raise NotImplementedError(
+            f"'{self.__class__.__name__}' does not support Secure Aggregation."
+            " To use Secure Aggregation over AUROC curves, please set the "
+            "initiating 'BinaryRocAUC' instance's 'bound' parameter to a "
+            "tuple of bounding values (with an associated 'scale'), and use "
+            "the same across all peers."
+        )
+
+
+class BinaryRocAUC(Metric[AurocState]):
     """ROC AUC metric for binary classification.
 
     This metric applies to a binary classifier, and computes the (opt.
     weighted) amount of true positives (TP), true negatives (TN), false
     positives (FP) and false negatives (FN) predictions over time around
     a variety of thresholds; from which TP rate, FP rate and finally ROC
     AUC metrics are eventually derived.
@@ -55,15 +203,16 @@
     Note that this class supports aggregating states from another
     BinaryRocAUC instance with different hyper-parameters into it,
     unless its `bound` parameter is set - in which case thresholds
     are not authorized to be dynamically updated, either at samples
     processing or states-aggregating steps.
     """
 
-    name: ClassVar[str] = "binary-roc"
+    name = "binary-roc"
+    state_cls = AurocState
 
     def __init__(
         self,
         scale: float = 0.1,
         label: Union[int, str] = 1,
         bound: Optional[Tuple[float, float]] = None,
     ) -> None:
@@ -94,31 +243,37 @@
           of thresholds.
         """
         self.scale = scale
         self.label = label
         self.bound = bound
         super().__init__()
 
-    def get_config(self) -> Dict[str, Any]:
+    def get_config(
+        self,
+    ) -> Dict[str, Any]:
         return {"scale": self.scale, "label": self.label, "bound": self.bound}
 
     @property
     def prec(self) -> int:
         """Numerical precision of threshold values."""
         return int(f"{self.scale:.1e}".rsplit("-", 1)[-1])
 
-    def _build_states(
+    def build_initial_states(
         self,
-    ) -> Dict[str, Union[float, np.ndarray]]:
-        bounds = (0, 1) if self.bound is None else self.bound
+    ) -> AurocState:
+        if self.bound is None:
+            bounds = (0.0, 1.0)
+            aggcls = AurocStateUnbound  # type: Type[AurocState]
+        else:
+            bounds = self.bound
+            aggcls = AurocState
         thresh = self._build_thresholds(*bounds)
         names = ("tpos", "tneg", "fpos", "fneg")
         states = {key: np.zeros_like(thresh) for key in names}
-        states["thr"] = thresh
-        return states  # type: ignore
+        return aggcls(**states, thresh=thresh)
 
     def _build_thresholds(
         self,
         lower: float,
         upper: float,
     ) -> np.ndarray:
         """Return a 1-d array of increasing threshold values."""
@@ -126,181 +281,80 @@
         t_max = np.ceil(upper / self.scale)
         return (np.arange(t_min, t_max + 1) * self.scale).round(self.prec)
 
     def get_result(
         self,
     ) -> Dict[str, Union[float, np.ndarray]]:
         # Unpack state variables for code readability.
-        tpos = self._states["tpos"][::-1]  # type: ignore
-        tneg = self._states["tneg"][::-1]  # type: ignore
-        fpos = self._states["fpos"][::-1]  # type: ignore
-        fneg = self._states["fneg"][::-1]  # type: ignore
+        tpos = self._states.tpos[::-1]
+        tneg = self._states.tneg[::-1]
+        fpos = self._states.fpos[::-1]
+        fneg = self._states.fneg[::-1]
         # Compute true- and false-positive rates and derive AUC.
         with np.errstate(invalid="ignore"):
             tpr = np.nan_to_num(tpos / (tpos + fneg), copy=False)
             fpr = np.nan_to_num(fpos / (fpos + tneg), copy=False)
         auc = sklearn.metrics.auc(fpr, tpr)
         return {
             "tpr": tpr,
             "fpr": fpr,
-            "thr": self._states["thr"][::-1],  # type: ignore
+            "thresh": self._states.thresh[::-1],
             "roc_auc": auc,
         }
 
     def update(
         self,
         y_true: np.ndarray,
         y_pred: np.ndarray,
         s_wght: Optional[np.ndarray] = None,
     ) -> None:
         # Set up the scaled set of thresholds at which to estimate states.
-        thresh = self._states["thr"]  # type: np.ndarray  # type: ignore
+        thresh = self._states.thresh
         if self.bound is None:
             thresh = self._build_thresholds(
                 min(y_pred.min(), thresh[0]),
                 max(y_pred.max(), thresh[-1]),
             )
+            aggcls = AurocStateUnbound  # type: Type[AurocState]
+        else:
+            aggcls = AurocState
         # Adjust inputs' shape if needed.
         y_pred = y_pred.reshape((-1, 1))
         y_true = y_true.reshape((-1, 1))
         s_wght = (
             np.ones_like(y_pred) if s_wght is None else s_wght.reshape((-1, 1))
         )
         # Compute threshold-wise prediction truthness values.
         pos = y_true == self.label
         tru = (y_pred >= thresh) == pos
         # Aggregate the former into threshold-wise TP/TN/FP/FN scores.
-        states = {
-            "tpos": (s_wght * (tru & pos)).sum(axis=0),
-            "tneg": (s_wght * (tru & ~pos)).sum(axis=0),
-            "fpos": (s_wght * ~(tru | pos)).sum(axis=0),
-            "fneg": (s_wght * (~tru & pos)).sum(axis=0),
-        }
-        # Aggregate these scores into the retained states.
-        thresh, states = _combine_roc_states(
-            thresh,
-            states,
-            self._states["thr"],  # type: ignore
-            self._states,  # type: ignore
+        states = aggcls(
+            tpos=(s_wght * (tru & pos)).sum(axis=0),
+            tneg=(s_wght * (tru & ~pos)).sum(axis=0),
+            fpos=(s_wght * ~(tru | pos)).sum(axis=0),
+            fneg=(s_wght * (~tru & pos)).sum(axis=0),
+            thresh=thresh,
         )
-        self._states = states  # type: ignore
-        self._states["thr"] = thresh
+        # Aggregate these scores into the retained states.
+        self._states += states
 
-    def agg_states(
+    def set_states(
         self,
-        states: Dict[str, Union[float, np.ndarray]],
+        states: AurocState,
     ) -> None:
-        # Run sanity check on input states.
-        for name in ("tpos", "tneg", "fpos", "fneg", "thr"):
-            if name not in states:
-                raise KeyError(f"Missing required state variable: '{name}'.")
-            if not isinstance(states[name], np.ndarray):
-                raise TypeError(f"Input state '{name}' is of unproper type.")
-            if states[name].ndim != 1:  # type: ignore
-                raise ValueError(f"Input state array '{name}' should be 1-d.")
-        # Gather thresholds. Raise if they differ and self is locked.
-        thr_own = self._states["thr"]  # type: np.ndarray  # type: ignore
-        thr_oth = states["thr"]  # type: np.ndarray  # type: ignore
+        # Prevent bounded instances from assigning unmatching inputs.
         if self.bound:
-            if (len(thr_own) != len(thr_oth)) or np.any(thr_own != thr_oth):
-                msg = "Input thresholds differ from bounded self ones."
-                raise ValueError(msg)
-        # Combine input states with self ones.
-        thresh, states = _combine_roc_states(  # type: ignore
-            thr_own, self._states, thr_oth, states  # type: ignore
-        )
-        self._states = states
-        self._states["thr"] = thresh
-
-
-def _combine_roc_states(
-    thresh_a: np.ndarray,
-    states_a: Dict[str, np.ndarray],
-    thresh_b: np.ndarray,
-    states_b: Dict[str, np.ndarray],
-) -> Tuple[np.ndarray, Dict[str, np.ndarray]]:
-    """Combine ROC states values, re-indexing them to thresholds if needed.
-
-    Parameters
-    ----------
-    thresh_a: 1d-array
-        1-d array of unique and sorted thresholds indexing `states_a`.
-    states_a: dict[str, 1d-array]
-        Dict of named 1-d arrays of state values, aligned on `thresh_a`.
-    thresh_b: 1d-array
-        1-d array of unique and sorted thresholds indexing `states_b`.
-    states_b: dict[str, 1d-array]
-        Dict of named 1-d arrays of state values, aligned on `thresh_b`.
-
-    Returns
-    -------
-    thresh: 1d-array
-        1-d array of unique and sorted thresholds computed as the union
-        of `thresh_a` and `thresh_b`.
-    states: dict[str, 1d-array]
-        Dict of named 1-d arrays of state values, aligned on `thresh`,
-        that are the sum of (interpolated) `states_a` and `states_b`.
-    """
-    # Case when thresholds are the same: simply sum up values and return.
-    if (len(thresh_a) == len(thresh_b)) and np.all(thresh_a == thresh_b):
-        states = {key: states_a[key] + states_b[key] for key in states_a}
-        return thresh_a, states
-    # Case when thresholds need alignment.
-    thresh = np.union1d(thresh_a, thresh_b)
-    states_a = _interpolate_roc_states(thresh, thresh_a, states_a)
-    states_b = _interpolate_roc_states(thresh, thresh_b, states_b)
-    states = {key: states_a[key] + states_b[key] for key in states_a}
-    return thresh, states
-
-
-def _interpolate_roc_states(
-    thresh_r: np.ndarray,
-    thresh_p: np.ndarray,
-    states_p: Dict[str, np.ndarray],
-) -> Dict[str, np.ndarray]:
-    """Interpolate ROC states values to fit given thresholds.
-
-    Parameters
-    ----------
-    thresh_r: 1d-array
-        1-d array of unique and sorted reference thresholds.
-    thresh_p: 1d-array
-        1-d array of unique and sorted partial thresholds.
-        `thresh_p` must be a subset of `thresh_r`.
-    states_p: dict[str, 1d-array]
-        Dict of named 1-d arrays of state values, aligned on
-        `thresh_p` and monotonically increasing or decreasing.
-
-    Returns
-    -------
-    states_r: dict[str, 1d-array]
-        Dict of names 1-d arrays of interpolated state values,
-        aligned on `thresh_r`.
-    """
-    keys = {"tpos", "tneg", "fpos", "fneg"}.intersection(states_p)
-    states_r = {key: np.zeros_like(thresh_r) for key in keys}
-    max_p = len(thresh_p) - 1
-    idp = 0
-    for idr, thr in enumerate(thresh_r):
-        # Case when the threshold exists in the partial subset.
-        if thresh_p[idp] == thr:
-            for key in states_r:
-                states_r[key][idr] = states_p[key][idp]
-            idp = min(idp + 1, max_p)
-        # Case when the threshold is below the subset's minimum.
-        elif idp == 0:
-            for key in states_r:
-                states_r[key][idr] = states_p[key][idp]
-        # Case when the threshold is above the subset's maximum.
-        elif thresh_p[max_p] < thr:
-            for key in states_r:
-                states_r[key][idr] = states_p[key][max_p]
-        # Case when the threshold-indexed values must and can be interpolated.
-        else:
-            t_inf = thresh_p[idp - 1]
-            t_sup = thresh_p[idp]
-            for key in states_r:
-                v_inf = states_p[key][idp - 1]
-                v_sup = states_p[key][idp]
-                states_r[key][idr] = thr * ((v_sup - v_inf) / (t_sup - t_inf))
-    # Return the interpolated states.
-    return states_r
+            if isinstance(states, AurocStateUnbound):
+                states = AurocState.from_dict(states.to_dict())
+            if not (
+                (len(self._states.thresh) == len(states.thresh))
+                and np.all(self._states.thresh == states.thresh)
+            ):
+                raise TypeError(
+                    f"Cannot assign '{self.__class__.__name__}' states with "
+                    "unmatching thresholds to an instance with bounded ones."
+                )
+        # Prevent unbounded instances from switching to bouded states.
+        elif self.bound is None and not isinstance(states, AurocStateUnbound):
+            states = AurocStateUnbound.from_dict(states.to_dict())
+        # Delegate assignment to parent call (that raises on wrong type).
+        return super().set_states(states)
```

### Comparing `declearn-2.3.2/declearn/metrics/_rsquared.py` & `declearn-2.4.0/declearn/metrics/_rsquared.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,27 +13,38 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Iterative and federative R-Squared evaluation metric."""
 
-from typing import ClassVar, Dict, Optional, Union
+import dataclasses
+from typing import Dict, Optional, Union
 
 import numpy as np
 
-from declearn.metrics._api import Metric
+from declearn.metrics._api import Metric, MetricState
 from declearn.metrics._utils import squeeze_into_identical_shapes
 
 __all__ = [
     "RSquared",
 ]
 
 
-class RSquared(Metric):
+@dataclasses.dataclass
+class R2State(MetricState):
+    """MetricState subclass for RSquared computations."""
+
+    sum_of_squared_errors: float = 0.0
+    sum_of_squared_labels: float = 0.0
+    sum_of_labels: float = 0.0
+    sum_of_weights: float = 0.0
+
+
+class RSquared(Metric[R2State]):
     """R^2 (R-Squared, coefficient of determination) regression metric.
 
     This metric applies to a regression model, and computes the (opt.
     weighted) R^2 score, also known as coefficient of determination.
 
     Computed metric is the following:
 
@@ -72,39 +83,34 @@
         - Decomposed weighted total sum of squares:
             $$\\sum_{i=1}^n w_i \\left(y_i-\\bar{y}\\right)^2 =
                 \\sum_i w_i y_i^2
                 - \\frac{\\left(\\sum_i w_i y_i\\right)^2}{\\sum_i w_i}
             $$
     """
 
-    name: ClassVar[str] = "r2"
+    name = "r2"
+    state_cls = R2State
 
-    def _build_states(
+    def build_initial_states(
         self,
-    ) -> Dict[str, Union[float, np.ndarray]]:
-        return {
-            "sum_of_squared_errors": 0.0,
-            "sum_of_squared_labels": 0.0,
-            "sum_of_labels": 0.0,
-            "sum_of_weights": 0.0,
-        }
+    ) -> R2State:
+        return R2State()
 
     def get_result(
         self,
     ) -> Dict[str, Union[float, np.ndarray]]:
         # Case when no samples were seen: return 0. by convention.
-        if self._states["sum_of_weights"] == 0:
+        if self._states.sum_of_weights == 0:
             return {self.name: 0.0}
         # Compute the (weighted) total sum of squares.
         ss_tot = (  # wSSt = sum(w * y^2) - (sum(w * y))^2 / sum(w)
-            self._states["sum_of_squared_labels"]
-            - self._states["sum_of_labels"] ** 2
-            / self._states["sum_of_weights"]
+            self._states.sum_of_squared_labels
+            - self._states.sum_of_labels**2 / self._states.sum_of_weights
         )
-        ss_res = self._states["sum_of_squared_errors"]
+        ss_res = self._states.sum_of_squared_errors
         # Handle the edge case where SSt is null.
         if ss_tot == 0:
             return {self.name: 1.0 if ss_res == 0 else 0.0}
         # Otherwise, compute and return the R-squared metric.
         result = 1 - ss_res / ss_tot
         return {self.name: float(result)}
 
@@ -115,21 +121,21 @@
         s_wght: Optional[np.ndarray] = None,
     ) -> None:
         y_true, y_pred = squeeze_into_identical_shapes(y_true, y_pred)
         # Verify sample weights' shape, or set up 1-valued ones.
         s_wght = self._prepare_sample_weights(s_wght, n_samples=len(y_pred))
         # Update the residual sum of squares. wSSr = sum(w * (y - p)^2)
         ss_res = (s_wght * self._sum_to_1d(y_true - y_pred) ** 2).sum()
-        self._states["sum_of_squared_errors"] += ss_res
+        self._states.sum_of_squared_errors += ss_res
         # Update states that compose the total sum of squares.
         # wSSt = sum(w * y^2) - (sum(w * y))^2 / sum(w)
         y_true = self._sum_to_1d(y_true)
-        self._states["sum_of_squared_labels"] += (s_wght * y_true**2).sum()
-        self._states["sum_of_labels"] += (s_wght * y_true).sum()
-        self._states["sum_of_weights"] += s_wght.sum()
+        self._states.sum_of_squared_labels += (s_wght * y_true**2).sum()
+        self._states.sum_of_labels += (s_wght * y_true).sum()
+        self._states.sum_of_weights += s_wght.sum()
 
     @staticmethod
     def _sum_to_1d(val: np.ndarray) -> np.ndarray:
         "Utility method to reduce an array of any shape to a 1-d array"
         while val.ndim > 1:
             val = val.sum(axis=-1)
         return val
```

### Comparing `declearn-2.3.2/declearn/metrics/_wrapper.py` & `declearn-2.4.0/declearn/metrics/_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Wrapper for an ensemble of Metric objects."""
 
+import warnings
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
-from declearn.metrics._api import Metric
+from declearn.metrics._api import Metric, MetricState
 
 __all__ = [
     "MetricInputType",
     "MetricSet",
 ]
 
 
@@ -114,15 +115,15 @@
         -------
         metricset: MetricSet
             MetricSet instance, type-checked or instantiated from inputs.
 
         Raises
         ------
         TypeError
-            If `metrics` is of unproper type.
+            If `metrics` is of improper type.
 
         Other exceptions may be raised when calling this class's `__init__`.
         """
         if metrics is None:
             metrics = cls([])
         if isinstance(metrics, list):
             metrics = cls(metrics)
@@ -174,35 +175,61 @@
     ) -> None:
         """Reset the metric to its initial state."""
         for metric in self.metrics:
             metric.reset()
 
     def get_states(
         self,
-    ) -> Dict[str, Dict[str, Union[float, np.ndarray]]]:
+    ) -> Dict[str, MetricState]:
         """Return a copy of the current state variables.
 
         This method is designed to expose and share partial results
         that may be aggregated with those of other instances of the
         same metric before computing overall results.
 
         Returns
         -------
-        states: dict[str, dict[str, float or numpy.ndarray]]
-            Dict of states that may be fed to another instance of
-            this class via its `agg_states` method.
+        states:
+            Dict of metric states that may be aggregated with their
+            counterparts and re-assigned for finalization using the
+            `set_states` then `get_result` methods of this object.
         """
         return {metric.name: metric.get_states() for metric in self.metrics}
 
+    def set_states(
+        self,
+        states: Dict[str, MetricState],
+    ) -> None:
+        """Replace internal states with a copy of incoming ones.
+
+        Parameters
+        ----------
+        states:
+            Replacement states, as a compatible `MetricState` instance.
+
+        Raises
+        ------
+        TypeError
+            If any metric states are of improper type.
+        """
+        for metric in self.metrics:
+            if metric.name in states:
+                metric.set_states(states[metric.name])
+
     def agg_states(
         self,
-        states: Dict[str, Dict[str, Union[float, np.ndarray]]],
+        states: Dict[str, MetricState],
     ) -> None:
         """Aggregate provided state variables into self ones.
 
+        This method is DEPRECATED as of DecLearn v2.4, in favor of
+        merely aggregating `MetricState` instances, using either
+        their `aggregate` method or the overloaded `+` operator.
+        It will be removed in DecLearn 2.6 and/or 3.0.
+
         This method is designed to aggregate results from multiple
         similar metrics objects into a single one before computing
         its results.
 
         Parameters
         ----------
         states: dict[str, float or numpy.ndarray]
@@ -210,21 +237,30 @@
             via its `get_states` method.
 
         Raises
         ------
         KeyError
             If any state variable is missing from `states`.
         TypeError
-            If any state variable is of unproper type.
+            If any state variable is of improper type.
         ValueError
-            If any array state variable is of unproper shape.
+            If any array state variable is of improper shape.
         """
-        for metric in self.metrics:
-            if metric.name in states:
-                metric.agg_states(states[metric.name])
+        warnings.warn(
+            "'MetricSet.agg_states' was deprecated in DecLearn v2.4, in favor "
+            "of aggregating 'MetricState' instances directly, and setting "
+            "final aggregated states using 'MetricSet.set_state'. It will be "
+            "removed in DecLearn 2.6 and/or 3.0.",
+            DeprecationWarning,
+        )
+        with warnings.catch_warnings():
+            warnings.simplefilter(action="ignore", category=DeprecationWarning)
+            for metric in self.metrics:
+                if metric.name in states:
+                    metric.agg_states(states[metric.name])
 
     def get_config(
         self,
     ) -> Dict[str, Any]:
         """Return a JSON-serializable configuration dict for this MetricSet."""
         cfg = [(metric.name, metric.get_config()) for metric in self.metrics]
         return {"metrics": cfg}
```

### Comparing `declearn-2.3.2/declearn/model/__init__.py` & `declearn-2.4.0/declearn/model/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/model/api/__init__.py` & `declearn-2.4.0/declearn/model/api/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,13 +19,15 @@
 
 This submodules exports the building blocks of the Model and Vector APIs:
 
 * [Model][declearn.model.api.Model]:
     Abstract class defining an API to interface a ML model.
 * [Vector][declearn.model.api.Vector]:
     Abstract class defining an API to manipulate (sets of) data arrays.
+* [VectorSpec][declearn.model.api.VectorSpec]:
+    Metadata container to specify a Vector for its (un)flattening.
 * [register_vector_type][declearn.model.api.register_vector_type]:
     Decorate a Vector subclass to make it buildable with `Vector.build`.
 """
 
-from ._vector import Vector, register_vector_type
+from ._vector import Vector, VectorSpec, register_vector_type
 from ._model import Model
```

### Comparing `declearn-2.3.2/declearn/model/api/_model.py` & `declearn-2.4.0/declearn/model/api/_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Model abstraction API."""
 
 from abc import ABCMeta, abstractmethod
-from typing import Any, Dict, Generic, Optional, Set, Tuple, TypeVar
+from typing import Any, Dict, Generic, List, Optional, Set, Tuple, TypeVar
 
 import numpy as np
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.model.api._vector import Vector
 from declearn.typing import Batch
 from declearn.utils import DevicePolicy, create_types_registry
@@ -58,14 +58,16 @@
 
     def __init__(
         self,
         model: Any,
     ) -> None:
         """Instantiate a Model interface wrapping a 'model' object."""
         self._model = model
+        # Declare a private list where to record batch-wise training losses.
+        self._loss_history = []  # type: List[float]
 
     def get_wrapped_model(self) -> Any:
         """Getter to access the wrapped framework-specific model object.
 
         This getter should be used sparingly, so as to avoid undesirable
         side effects. In particular, it should not be used in declearn
         backend code (but may be in examples or tests), as it is merely
@@ -198,14 +200,18 @@
     ) -> VectorT:
         """Compute and return gradients computed over a given data batch.
 
         Compute the average gradients of the model's loss with respect
         to its trainable parameters for the given data batch.
         Optionally clip sample-wise gradients before batch-averaging.
 
+        Record the loss value over the batch, which may be collected
+        (and thereof purged from the internal memory) by calling the
+        `collect_training_losses` method.
+
         Parameters
         ----------
         batch: declearn.typing.Batch
             Tuple wrapping input data, (opt.) target values and (opt.)
             sample weights to be applied to the loss function.
         max_norm: float or None, default=None
             Maximum L2-norm of sample-wise gradients, beyond which to
@@ -223,14 +229,33 @@
     @abstractmethod
     def apply_updates(
         self,
         updates: VectorT,
     ) -> None:
         """Apply updates to the model's weights."""
 
+    def collect_training_losses(
+        self,
+    ) -> List[float]:
+        """Collect batch-wise training losses accumulated over time.
+
+        Return all recorded batch-averaged loss values computed a
+        part of `compute_batch_gradients` calls, and clear them
+        from memory, so that next time this method is called, only
+        new values are returned.
+
+        Returns
+        -------
+        losses:
+            List of bath-averaged loss values computed over inputs
+            to the `compute_batch_gradients` method.
+        """
+        losses, self._loss_history = self._loss_history, []
+        return losses
+
     @abstractmethod
     def compute_batch_predictions(
         self,
         batch: Batch,
     ) -> Tuple[np.ndarray, np.ndarray, Optional[np.ndarray]]:
         """Compute and return model predictions on given inputs.
```

### Comparing `declearn-2.3.2/declearn/model/api/_vector.py` & `declearn-2.4.0/declearn/model/api/_vector.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,43 +13,84 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Vector abstraction API."""
 
+import dataclasses
 import operator
+import warnings
 from abc import ABCMeta, abstractmethod
 from typing import (
     # fmt: off
-    Any, Callable, Dict, Generic, Optional, Set, Tuple, Type, TypeVar, Union
+    Any, Callable, Dict, Generic, List, Optional,
+    Set, Tuple, Type, TypeVar, Union
 )
 
 from typing_extensions import Self  # future: import from typing (Py>=3.11)
 
 from declearn.utils import (
+    access_registered,
+    access_registration_info,
     add_json_support,
     create_types_registry,
     register_type,
 )
 
 __all__ = [
     "Vector",
+    "VectorSpec",
     "register_vector_type",
 ]
 
 
 VECTOR_TYPES = {}  # type: Dict[Type[Any], Type[Vector]]
 """Private constant holding registered Vector types."""
 
 
 T = TypeVar("T")
 """Type-annotation for the data structures proper to a given Vector class."""
 
 
+@dataclasses.dataclass
+class VectorSpec:
+    """Metadata container to specify a Vector for its (un)flattening.
+
+    Fields
+    ------
+    names:
+        List of names of the coefficient tensors.
+    shapes:
+        Dict associating shapes (as tuples of int) to coefficient names.
+    dtypes:
+        Dict associating dtypes (as string values) to coefficient names.
+    v_type:
+        Optional (name, group) tuple of strings containing registration
+        information enabling to recover the `Vector` subclass.
+    kwargs:
+        Dict containing any subclass-specific metadata useful in building
+        back a Vector from its specifications and flattened values.
+    """
+
+    names: List[str]
+    shapes: Dict[str, Tuple[int, ...]]
+    dtypes: Dict[str, str]
+    v_type: Optional[Tuple[str, str]] = None
+    kwargs: Dict[str, Any] = dataclasses.field(default_factory=dict)
+
+
+add_json_support(
+    cls=VectorSpec,
+    pack=dataclasses.asdict,
+    unpack=lambda x: VectorSpec(**x),
+    name="VectorSpec",
+)
+
+
 @create_types_registry
 class Vector(Generic[T], metaclass=ABCMeta):
     """Abstract class defining an API to manipulate (sets of) data arrays.
 
     A Vector is an abstraction used to wrap a collection of data
     structures (numpy arrays, tensorflow or torch tensors, etc.).
     It enables writing algorithms and operations on such structures,
@@ -437,14 +478,165 @@
 
     @abstractmethod
     def sum(
         self,
     ) -> Self:
         """Compute coefficient-wise sum of elements."""
 
+    def get_vector_specs(
+        self,
+    ) -> VectorSpec:
+        """Return a VectorSpec instance storing metadata on this Vector.
+
+        This method is mostly meant to be called by the `flatten` class
+        method, and is merely implemented to define some common grounds
+        across all Vector subclasses.
+        """
+        try:
+            v_type = access_registration_info(type(self))
+        except KeyError:  # pragma: no cover
+            v_type = None
+            warnings.warn(
+                "Accessing specs of an unregistered Vector subclass.",
+                UserWarning,
+            )
+        return VectorSpec(
+            names=list(self.coefs),
+            shapes=self.shapes(),
+            dtypes=self.dtypes(),
+            v_type=v_type,
+        )
+
+    @abstractmethod
+    def flatten(
+        self,
+    ) -> Tuple[List[float], VectorSpec]:
+        """Flatten this Vector into a list of float and a metadata dict.
+
+        If this Vector contains any sparse data structure, it is expected
+        that zero-valued coefficients *are* part of the output values, as
+        the (un)flattening methods are aimed at enabling SecAgg features,
+        that may involve summing up tensors with distinct sparsity, which
+        cannot be easily anticipated in a decentralized fashin.
+
+        Returns
+        -------
+        values:
+            List of concatenated float (or int) values from this Vector.
+        v_spec:
+            VectorSpec instance storing metadata enabling to convert the
+            flattened values into a Vector instance similar to this one.
+        """
+
+    @classmethod
+    @abstractmethod
+    def unflatten(
+        cls,
+        values: List[float],
+        v_spec: VectorSpec,
+    ) -> Self:
+        """Unflatten a Vector from a list of float and a metadata dict.
+
+        This is the counterpart method to `flatten` and is defined at
+        the level of each Vector subclass. You may alternatively use
+        the `Vector.build_from_specs` generic method to automate the
+        identification of the target Vector subclass and pass inputs
+        to its `unflatten` method.
+
+        Parameters
+        ----------
+        values:
+            List of concatenated float (or int) values of the Vector.
+        v_spec:
+            VectorSpec instance storing metadata enabling to convert the
+            flattened values into an instance of this Vector class, with
+            proper data shapes and dtypes.
+
+        Returns
+        -------
+        vector:
+            Recovered Vector matching the one that was flattened into
+            the input arguments.
+
+        Raises
+        ------
+        KeyError
+            If the input specifications do not match expectations from
+            this specific Vector subclass.
+        ValueError
+            If the input values cannot be turned back into the shapes
+            and dtypes specified by input vector specs.
+        """
+
+    @staticmethod
+    def build_from_specs(
+        values: List[float],
+        v_spec: VectorSpec,
+    ) -> "Vector":
+        """Unflatten a Vector from a list of float and a metadata dict.
+
+        This staticmethod is a more generic version of the `unflatten`
+        classmethod, that may be called from the `Vector` ABC directly
+        in order to recreate a Vector from its specifications without
+        prior knowledge of the output Vector subclass, retrieved from
+        the `v_spec` information rather than from end-user knowledge.
+
+        Parameters
+        ----------
+        values:
+            List of concatenated float (or int) values of the Vector.
+        v_spec:
+            VectorSpec instance storing metadata enabling to convert
+            the flattened values into a Vector instance of a proper
+            type and with proper data shapes and dtypes.
+
+        Returns
+        -------
+        vector:
+            Recovered Vector matching the one that was flattened into
+            the input arguments.
+
+        Raises
+        ------
+        KeyError
+            If the input specifications do not enable retrieving the
+            Vector subclass constructor to use.
+            If the input specifications do not match expectations from
+            that target Vector subclass.
+        TypeError
+            If the inputs do not match type expectations.
+        ValueError
+            If the input values cannot be turned back into the shapes
+            and dtypes specified by input vector specs.
+        """
+        if not isinstance(v_spec, VectorSpec):
+            raise TypeError(
+                f"Expected 'v_spec' to be a VectorSpec, not '{type(v_spec)}'."
+            )
+        if v_spec.v_type is None:
+            raise KeyError(
+                "'Vector.build_from_specs' requires the input VectorSpec "
+                "to specify registration information of the target Vector "
+                "subclass."
+            )
+        try:
+            cls = access_registered(*v_spec.v_type)
+        except KeyError as exc:
+            raise KeyError(
+                "'Vector.build_from_specs' could not retrieve the target "
+                "Vector subclass based on provided registration information."
+            ) from exc
+        if not (isinstance(cls, type) and issubclass(cls, Vector)):
+            raise TypeError(
+                "'Vector.build_from_specs' retrieved something that is not a "
+                "Vector subclass based on provided registration information: "
+                f"'{cls}'."
+            )
+        return cls.unflatten(values, v_spec)
+
 
 def register_vector_type(
     v_type: Type[Any],
     *types: Type[Any],
     name: Optional[str] = None,
 ) -> Callable[[Type[Vector]], Type[Vector]]:
     """Decorate a Vector subclass to make it buildable with `Vector.build`.
```

### Comparing `declearn-2.3.2/declearn/model/haiku/__init__.py` & `declearn-2.4.0/declearn/model/haiku/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/model/haiku/_model.py` & `declearn-2.4.0/declearn/model/haiku/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,31 +381,37 @@
         train_params, fixed_params = hk.data_structures.partition(
             predicate=lambda l, w, _: f"{l}:{w}" in self._trainable,
             structure=self._params,
         )
         rng = next(self._rng_gen)
         # Compute batch-averaged gradients, opt. clipped on a per-sample basis.
         if max_norm:
-            grads = self._clipped_grad_fn(
+            grads, loss = self._clipped_grads_and_loss_fn(
                 train_params, fixed_params, rng, inputs, max_norm
             )
             grads = [value.mean(0) for value in grads]
         else:
-            grads = jax.tree_util.tree_leaves(
-                self._grad_fn(train_params, fixed_params, rng, inputs)
+            loss, grads_tree = self._loss_and_grads_fn(
+                train_params, fixed_params, rng, inputs
             )
+            grads = jax.tree_util.tree_leaves(grads_tree)
+        # Record the batch-averaged loss value.
+        self._loss_history.append(float(np.array(loss).mean()))
         # Return the gradients, flattened into a JaxNumpyVector container.
         return JaxNumpyVector(dict(zip(self._trainable, grads)))
 
     @functools.cached_property
-    def _grad_fn(
+    def _loss_and_grads_fn(
         self,
-    ) -> Callable[[hk.Params, hk.Params, jax.Array, JaxBatch], hk.Params]:
+    ) -> Callable[
+        [hk.Params, hk.Params, jax.Array, JaxBatch],
+        Tuple[jax.Array, hk.Params],
+    ]:
         """Lazy-built jax function to compute batch-averaged gradients."""
-        return jax.jit(jax.grad(self._forward))
+        return jax.jit(jax.value_and_grad(self._forward))
 
     def _forward(
         self,
         train_params: hk.Params,
         fixed_params: hk.Params,
         rng: jax.Array,
         batch: JaxBatch,
@@ -432,48 +438,49 @@
         y_pred = self._model.apply(params, rng, *inputs)
         s_loss = self._loss_fn(y_pred, y_true)  # type: ignore
         if s_wght is not None:
             s_loss = s_loss * s_wght
         return jnp.mean(s_loss)
 
     @functools.cached_property
-    def _clipped_grad_fn(
+    def _clipped_grads_and_loss_fn(
         self,
     ) -> Callable[
-        [hk.Params, hk.Params, jax.Array, JaxBatch, float], List[jax.Array]
+        [hk.Params, hk.Params, jax.Array, JaxBatch, float],
+        Tuple[List[jax.Array], jax.Array],
     ]:
         """Lazy-built jax function to compute clipped sample-wise gradients.
 
         Note: The vmap in_axis parameters work thank to the jax feature of
         applying optional parameters to pytrees.
         """
 
-        def clipped_grad_fn(
+        def clipped_grads_and_loss_fn(
             train_params: hk.Params,
             fixed_params: hk.Params,
             rng: jax.Array,
             batch: JaxBatch,
             max_norm: float,
-        ) -> List[jax.Array]:
+        ) -> Tuple[List[jax.Array], jax.Array]:
             """Compute and clip gradients wrt parameters for a sample."""
             inputs, y_true, s_wght = batch
             batch = (inputs, y_true, None)
-            grads = jax.grad(self._forward)(
+            loss, grads = jax.value_and_grad(self._forward)(
                 train_params, fixed_params, rng, batch
             )
             grads_flat = [
                 grad / jnp.maximum(jnp.linalg.norm(grad) / max_norm, 1.0)
                 for grad in jax.tree_util.tree_leaves(grads)
             ]
             if s_wght is not None:
                 grads_flat = [g * s_wght for g in grads_flat]
-            return grads_flat
+            return grads_flat, loss
 
         in_axes = [None, None, None, 0, None]  # map on inputs' first dimension
-        return jax.jit(jax.vmap(clipped_grad_fn, in_axes))
+        return jax.jit(jax.vmap(clipped_grads_and_loss_fn, in_axes))
 
     def _unpack_batch(
         self,
         batch: Batch,
     ) -> JaxBatch:
         """Unpack and enforce jnp.array conversion to an input data batch."""
```

### Comparing `declearn-2.3.2/declearn/model/haiku/_vector.py` & `declearn-2.4.0/declearn/model/haiku/_vector.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """JaxNumpyVector data arrays container."""
 
 import warnings
-from typing import Any, Callable, Dict, Optional, Set, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
 
 import jax
 import jax.numpy as jnp
 import jaxlib
 import numpy as np
 from typing_extensions import Self  # future: import from typing (Py>=3.11)
 
-from declearn.model.api import Vector, register_vector_type
+from declearn.model.api import Vector, VectorSpec, register_vector_type
 from declearn.model.haiku.utils import select_device
 from declearn.model.sklearn import NumpyVector
+from declearn.model._utils import flatten_numpy_arrays, unflatten_numpy_arrays
 from declearn.utils import get_device_policy
 
 __all__ = [
     "JaxNumpyVector",
 ]
 
 
@@ -119,15 +120,18 @@
             other = JaxNumpyVector(coefs)
         return super()._apply_operation(other, func)
 
     def __eq__(self, other: Any) -> bool:
         valid = isinstance(other, JaxNumpyVector)
         valid = valid and (self.coefs.keys() == other.coefs.keys())
         return valid and all(
-            jnp.array_equal(self.coefs[k], other.coefs[k]) for k in self.coefs
+            jnp.array_equal(
+                val, jax.device_put(other.coefs[key], val.device())
+            )
+            for key, val in self.coefs.items()
         )
 
     def sign(
         self,
     ) -> Self:
         return self.apply_func(jnp.sign)
 
@@ -175,7 +179,30 @@
         cls,
         data: Dict[str, Any],
     ) -> Self:
         policy = get_device_policy()
         device = select_device(gpu=policy.gpu, idx=policy.idx)
         coefs = {k: jax.device_put(arr, device) for k, arr in data.items()}
         return cls(coefs)
+
+    # similar code to that of TorchVector; pylint: disable=duplicate-code
+
+    def flatten(
+        self,
+    ) -> Tuple[List[float], VectorSpec]:
+        v_spec = self.get_vector_specs()
+        arrays = self.pack()
+        values = flatten_numpy_arrays([arrays[name] for name in v_spec.names])
+        return values, v_spec
+
+    @classmethod
+    def unflatten(
+        cls,
+        values: List[float],
+        v_spec: VectorSpec,
+    ) -> Self:
+        shapes = [v_spec.shapes[name] for name in v_spec.names]
+        dtypes = [v_spec.dtypes[name] for name in v_spec.names]
+        arrays = unflatten_numpy_arrays(values, shapes, dtypes)
+        return cls.unpack(dict(zip(v_spec.names, arrays)))
+
+    # pylint: enable=duplicate-code
```

### Comparing `declearn-2.3.2/declearn/model/haiku/utils/__init__.py` & `declearn-2.4.0/declearn/model/haiku/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/model/haiku/utils/_gpu.py` & `declearn-2.4.0/declearn/model/haiku/utils/_gpu.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/model/sklearn/__init__.py` & `declearn-2.4.0/declearn/model/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/model/sklearn/_np_vec.py` & `declearn-2.4.0/declearn/model/sklearn/_np_vec.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """NumpyVector data arrays container."""
 
 import warnings
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from typing_extensions import Self  # future: import from typing (Py>=3.11)
 
-from declearn.model.api._vector import Vector, register_vector_type
+from declearn.model.api._vector import Vector, VectorSpec, register_vector_type
+from declearn.model._utils import flatten_numpy_arrays, unflatten_numpy_arrays
 
 
 __all__ = [
     "NumpyVector",
 ]
 
 
@@ -131,7 +132,27 @@
                 DeprecationWarning,
             )
         coefs = {
             key: np.array(np.sum(val, axis=axis, keepdims=keepdims))
             for key, val in self.coefs.items()
         }
         return self.__class__(coefs)
+
+    def flatten(
+        self,
+    ) -> Tuple[List[float], VectorSpec]:
+        v_spec = self.get_vector_specs()
+        values = flatten_numpy_arrays(
+            [self.coefs[name] for name in v_spec.names]
+        )
+        return values, v_spec
+
+    @classmethod
+    def unflatten(
+        cls,
+        values: List[float],
+        v_spec: VectorSpec,
+    ) -> Self:
+        shapes = [v_spec.shapes[name] for name in v_spec.names]
+        dtypes = [v_spec.dtypes[name] for name in v_spec.names]
+        arrays = unflatten_numpy_arrays(values, shapes, dtypes)
+        return cls(dict(zip(v_spec.names, arrays)))
```

### Comparing `declearn-2.3.2/declearn/model/sklearn/_sgd.py` & `declearn-2.4.0/declearn/model/sklearn/_sgd.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,14 +393,19 @@
             for vec in grad:
                 for arr in vec.coefs.values():
                     norm = np.sqrt(np.sum(np.square(arr)))
                     arr *= min(max_norm / norm, 1)
         # Optionally re-weight gradients based on sample weights.
         if s_wght is not None:
             grad = [g * w for g, w in zip(grad, s_wght)]
+        # Compute and record the loss value on the entire batch.
+        loss = self.loss_function(
+            y_data, self._predict(x_data)  # type: ignore
+        )
+        self._loss_history.append(float(loss.mean()))
         # Batch-average the gradients and return them.
         return sum(grad) / len(grad)  # type: ignore
 
     def _unpack_batch(
         self,
         batch: Batch,
     ) -> Tuple[DataArray, DataArray, Optional[DataArray]]:
@@ -480,20 +485,21 @@
         return self._loss_fn(y_true, y_pred)
 
     def _setup_loss_fn(
         self,
     ) -> Callable[[np.ndarray, np.ndarray], np.ndarray]:
         """Return a function to compute point-wise loss for a given batch."""
         # fmt: off
-        # Gather / instantiate a loss function from the wrapped model's specs.
-        if hasattr(self._model, "loss_function_"):
-            loss_smp = self._model.loss_function_.py_loss
-        else:
-            loss_cls, *args = self._model.loss_functions[self._model.loss]
-            loss_smp = loss_cls(*args).py_loss
+        # Instantiate a loss function from the wrapped model's specs.
+        loss_cls, *args = self._model.loss_functions[self._model.loss]
+        if self._model.loss in (
+            "huber", "epsilon_insensitive", "squared_epsilon_insensitive"
+        ):
+            args = (self._model.epsilon,)
+        loss_smp = loss_cls(*args).py_loss
         # Wrap it to support batched inputs.
         def loss_1d(y_true: np.ndarray, y_pred: np.ndarray) -> np.ndarray:
             return np.array([loss_smp(*smp) for smp in zip(y_pred, y_true)])
         # For multiclass classifiers, further wrap to support 2d predictions.
         if len(getattr(self._model, "classes_", [])) > 2:
             def loss_fn(y_true: np.ndarray, y_pred: np.ndarray) -> np.ndarray:
                 return np.sum([
```

### Comparing `declearn-2.3.2/declearn/model/tensorflow/__init__.py` & `declearn-2.4.0/declearn/model/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/model/tensorflow/_model.py` & `declearn-2.4.0/declearn/model/tensorflow/_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,20 @@
 
 """Model subclass to wrap TensorFlow models."""
 
 from copy import deepcopy
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, Union
 
 import numpy as np
+# fmt: off
+# pylint: disable=import-error,no-name-in-module
 import tensorflow as tf  # type: ignore
+import tensorflow.keras as tf_keras  # type: ignore
+# pylint: enable=import-error,no-name-in-module
+# fmt: on
 from numpy.typing import ArrayLike
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.data_info import aggregate_data_info
 from declearn.model._utils import raise_on_stringsets_mismatch
 from declearn.model.api import Model
 from declearn.model.tensorflow._vector import TensorflowVector
@@ -42,15 +47,15 @@
 ]
 
 
 @register_type(name="TensorflowModel", group="Model")
 class TensorflowModel(Model):
     """Model wrapper for TensorFlow Model instances.
 
-    This `Model` subclass is designed to wrap a `tf.keras.Model` instance
+    This `Model` subclass is designed to wrap a `tf_keras.Model` instance
     to be trained federatively.
 
     Notes regarding device management (CPU, GPU, etc.):
 
     - By default, tensorflow places data and operations on GPU whenever one
       is available.
     - Our `TensorflowModel` instead consults the device-placement policy (via
@@ -65,17 +70,17 @@
       `update_device_policy` method.
     - You may consult the device policy enforced by a TensorflowModel
       instance by accessing its `device_policy` property.
     """
 
     def __init__(
         self,
-        model: tf.keras.layers.Layer,
-        loss: Union[str, tf.keras.losses.Loss],
-        metrics: Optional[List[Union[str, tf.keras.metrics.Metric]]] = None,
+        model: tf_keras.layers.Layer,
+        loss: Union[str, tf_keras.losses.Loss],
+        metrics: Optional[List[Union[str, tf_keras.metrics.Metric]]] = None,
         _from_config: bool = False,
         **kwargs: Any,
     ) -> None:
         """Instantiate a Model interface wrapping a tensorflow.keras model.
 
         Parameters
         ----------
@@ -88,27 +93,27 @@
             is provided, it will be converted to a Loss instance, and
             an exception may be raised if that fails.
         metrics: list[str or tf.keras.metrics.Metric] or None
             List of keras Metric instances, or their names. These are
             compiled with the model and computed using the `evaluate`
             method of the returned TensorflowModel instance.
         **kwargs: Any
-            Any additional keyword argument to `tf.keras.Model.compile`
+            Any additional keyword argument to `tf_keras.Model.compile`
             may be passed.
         """
         # Type-check the input Model and wrap it up.
-        if not isinstance(model, tf.keras.layers.Layer):
+        if not isinstance(model, tf_keras.layers.Layer):
             raise TypeError(
-                "'model' should be a tf.keras.layers.Layer instance."
+                "'model' should be a tf_keras.layers.Layer instance."
             )
-        if not isinstance(model, tf.keras.Model):
-            model = tf.keras.Sequential([model])
+        if not isinstance(model, tf_keras.Model):
+            model = tf_keras.Sequential([model])
         super().__init__(model)
         # Ensure the loss is a keras.Loss object and set its reduction to none.
-        loss = build_keras_loss(loss, reduction=tf.keras.losses.Reduction.NONE)
+        loss = build_keras_loss(loss, reduction=tf_keras.losses.Reduction.NONE)
         # Select the device where to place computations and move the model.
         policy = get_device_policy()
         self._device = select_device(gpu=policy.gpu, idx=policy.idx)
         if not _from_config:
             self._model = move_layer_to_device(self._model, self._device)
         # Finalize initialization using the selected device.
         # Compile the wrapped model and retain compilation arguments.
@@ -146,17 +151,17 @@
             # Build the model using the specified input shape.
             with tf.device(self._device):
                 self._model.build((None, *data_info["features_shape"]))
 
     def get_config(
         self,
     ) -> Dict[str, Any]:
-        config = tf.keras.layers.serialize(self._model)  # type: Dict[str, Any]
+        config = tf_keras.layers.serialize(self._model)  # type: Dict[str, Any]
         kwargs = deepcopy(self._kwargs)
-        loss = tf.keras.losses.serialize(kwargs.pop("loss"))
+        loss = tf_keras.losses.serialize(kwargs.pop("loss"))
         return {"model": config, "loss": loss, "kwargs": kwargs}
 
     @classmethod
     def from_config(
         cls,
         config: Dict[str, Any],
     ) -> Self:
@@ -165,39 +170,51 @@
             if key not in config.keys():
                 raise KeyError(f"Missing key '{key}' in the config dict.")
         # Set up the device policy.
         policy = get_device_policy()
         device = select_device(gpu=policy.gpu, idx=policy.idx)
         # Deserialize the model and loss keras objects on the device.
         with tf.device(device):
-            model = tf.keras.layers.deserialize(config["model"])
-            loss = tf.keras.losses.deserialize(config["loss"])
+            model = tf_keras.layers.deserialize(config["model"])
+            loss = tf_keras.losses.deserialize(config["loss"])
         # Instantiate the TensorflowModel, avoiding device-to-device copies.
         return cls(model, loss, **config["kwargs"], _from_config=True)
 
     def get_weights(
         self,
         trainable: bool = False,
     ) -> TensorflowVector:
+        variables = self._get_weight_variables(trainable)
+        return TensorflowVector({var.name: var.value() for var in variables})
+
+    def _get_weight_variables(
+        self,
+        trainable: bool,
+    ) -> Iterable[tf.Variable]:
+        """Access TensorFlow Variables wrapping model weight tensors."""
         variables = (
             self._model.trainable_weights if trainable else self._model.weights
         )
-        return TensorflowVector({var.name: var.value() for var in variables})
+        if hasattr(tf_keras, "version") and tf_keras.version().startswith("3"):
+            variables = (var.value for var in variables)
+        return variables
 
     def set_weights(
         self,
         weights: TensorflowVector,
         trainable: bool = False,
     ) -> None:
         if not isinstance(weights, TensorflowVector):
             raise TypeError(
                 "TensorflowModel requires TensorflowVector weights."
             )
         self._verify_weights_compatibility(weights, trainable=trainable)
-        variables = {var.name: var for var in self._model.weights}
+        variables = {
+            var.name: var for var in self._get_weight_variables(trainable)
+        }
         with tf.device(self._device):
             for name, value in weights.coefs.items():
                 variables[name].assign(value, read_value=False)
 
     def _verify_weights_compatibility(
         self,
         vector: TensorflowVector,
@@ -216,36 +233,35 @@
 
         Raises
         ------
         KeyError
             In case some expected keys are missing, or additional keys
             are present. Be verbose about the identified mismatch(es).
         """
-        variables = (
-            self._model.trainable_weights if trainable else self._model.weights
-        )
+        variables = self._get_weight_variables(trainable)
         raise_on_stringsets_mismatch(
             received=set(vector.coefs),
             expected={var.name for var in variables},
             context="model weights",
         )
 
     def compute_batch_gradients(
         self,
         batch: Batch,
         max_norm: Optional[float] = None,
     ) -> TensorflowVector:
         with tf.device(self._device):
             data = self._unpack_batch(batch)
             if max_norm is None:
-                grads = self._compute_batch_gradients(*data)
+                grads, loss = self._compute_batch_gradients(*data)
             else:
                 norm = tf.constant(max_norm)
-                grads = self._compute_clipped_gradients(*data, norm)
-        grads_and_vars = zip(grads, self._model.trainable_weights)
+                grads, loss = self._compute_clipped_gradients(*data, norm)
+        self._loss_history.append(float(loss.numpy()))
+        grads_and_vars = zip(grads, self._get_weight_variables(trainable=True))
         return TensorflowVector(
             {var.name: grad for grad, var in grads_and_vars}
         )
 
     def _unpack_batch(
         self,
         batch: Batch,
@@ -263,50 +279,50 @@
 
     @tf.function  # optimize tensorflow runtime
     def _compute_batch_gradients(
         self,
         inputs: tf.Tensor,
         y_true: Optional[tf.Tensor],
         s_wght: Optional[tf.Tensor],
-    ) -> List[tf.Tensor]:
+    ) -> Tuple[List[tf.Tensor], tf.Tensor]:
         """Compute and return batch-averaged gradients of trainable weights."""
         with tf.GradientTape() as tape:
             y_pred = self._model(inputs, training=True)
             loss = self._model.compute_loss(inputs, y_true, y_pred, s_wght)
             loss = tf.reduce_mean(loss)
             grad = tape.gradient(loss, self._model.trainable_weights)
-        return grad
+        return grad, loss
 
     @tf.function  # optimize tensorflow runtime
     def _compute_clipped_gradients(
         self,
         inputs: tf.Tensor,
         y_true: Optional[tf.Tensor],
         s_wght: Optional[tf.Tensor],
         max_norm: Union[tf.Tensor, float],
-    ) -> List[tf.Tensor]:
+    ) -> Tuple[List[tf.Tensor], tf.Tensor]:
         """Compute and return sample-wise-clipped batch-averaged gradients."""
-        grad = self._compute_samplewise_gradients(inputs, y_true)
+        grad, loss = self._compute_samplewise_gradients(inputs, y_true)
         if s_wght is None:
             s_wght = tf.cast(1, grad[0].dtype)
         grad = self._clip_and_average_gradients(grad, max_norm, s_wght)
-        return grad
+        return grad, loss
 
     @tf.function  # optimize tensorflow runtime
     def _compute_samplewise_gradients(
         self,
         inputs: tf.Tensor,
         y_true: Optional[tf.Tensor],
-    ) -> List[tf.Tensor]:
+    ) -> Tuple[List[tf.Tensor], tf.Tensor]:
         """Compute and return sample-wise gradients for a given batch."""
         with tf.GradientTape() as tape:
             y_pred = self._model(inputs, training=True)
             loss = self._model.compute_loss(inputs, y_true, y_pred)
             grad = tape.jacobian(loss, self._model.trainable_weights)
-        return grad
+        return grad, tf.reduce_mean(loss)
 
     @staticmethod
     @tf.function  # optimize tensorflow runtime
     def _clip_and_average_gradients(
         gradients: List[tf.Tensor],
         max_norm: Union[tf.Tensor, float],
         s_wght: tf.Tensor,
@@ -321,15 +337,15 @@
 
     def apply_updates(
         self,
         updates: TensorflowVector,
     ) -> None:
         self._verify_weights_compatibility(updates, trainable=True)
         with tf.device(self._device):
-            for var in self._model.trainable_weights:
+            for var in self._get_weight_variables(trainable=True):
                 updt = updates.coefs[var.name]
                 if isinstance(updt, tf.IndexedSlices):
                     var.scatter_add(updt)
                 else:
                     var.assign_add(updt, read_value=False)
 
     def evaluate(
```

### Comparing `declearn-2.3.2/declearn/model/tensorflow/_optim.py` & `declearn-2.4.0/declearn/model/tensorflow/_optim.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Hacky OptiModule subclass enabling the use of a keras Optimizer."""
 
-from typing import Any, Dict, Union
+from typing import Any, Dict, List, Union
 
+# fmt: off
+# pylint: disable=import-error,no-name-in-module
 import tensorflow as tf  # type: ignore
+import tensorflow.keras as tf_keras  # type: ignore
+# pylint: enable=import-error,no-name-in-module
+# fmt: on
 
 from declearn.model.api import Vector
 from declearn.model.tensorflow.utils import select_device
 from declearn.model.tensorflow._vector import TensorflowVector
 from declearn.optimizer.modules import OptiModule
 from declearn.utils import get_device_policy
 
@@ -77,15 +82,15 @@
     instead of a declearn one can lead to diverging results.
     """
 
     name = "tensorflow-optim"
 
     def __init__(
         self,
-        optim: Union[tf.keras.optimizers.Optimizer, str, Dict[str, Any]],
+        optim: Union[tf_keras.optimizers.Optimizer, str, Dict[str, Any]],
     ) -> None:
         """Instantiate a hacky tensorflow optimizer plug-in module.
 
         Parameters
         ----------
         optim: tf.keras.optimizers.Optimizer or dict[str, any] or str
             Keras optimizer instance that needs wrapping, or configuration
@@ -101,15 +106,15 @@
         plug-in.
         """
         # Select the device where to place the wrapped states and computations.
         policy = get_device_policy()
         self._device = select_device(gpu=policy.gpu, idx=policy.idx)
         # Wrap the provided optimizer, enforcing a fixed learning rate of 1.
         # Also prevent the use of weight-decay or built-in ema (~momentum).
-        self.optim = tf.keras.optimizers.get(optim)
+        self.optim = tf_keras.optimizers.get(optim)
         config = self.optim.get_config()
         config["weight_decay"] = 0
         config["use_ema"] = False
         if "learning_rate" in config:
             config["learning_rate"] = 1.0
         # Force the use of a brand-new optimizer instance.
         with tf.device(self._device):
@@ -180,15 +185,15 @@
     def _init_variables(self, gradients: TensorflowVector) -> None:
         """Create zero-valued variables based on input gradients' specs."""
         with tf.device(self._device):
             self._vars = {
                 key: tf.Variable(tf.zeros_like(grad), name=key)
                 for key, grad in gradients.coefs.items()
             }
-            self.optim.build(self._vars.values())
+            self.optim.build(list(self._vars.values()))
 
     def reset(self) -> None:
         """Reset this module to its uninitialized state.
 
         Discard the wrapped tensorflow Variables (that define a required
         specification of input gradients), and replace the optimizer with
         a new, uninitialized one. As a consequence, the next call to `run`
@@ -197,35 +202,44 @@
         This method also updates the device-placement policy of the states
         and computations wrapped by this OptiModule, based on the global
         policy accessed via `declearn.utils.get_device_policy`.
         """
         policy = get_device_policy()
         self._device = select_device(gpu=policy.gpu, idx=policy.idx)
         with tf.device(self._device):
-            self._vars = {}
+            self._vars.clear()
             self.optim = self.optim.from_config(self.optim.get_config())
 
     def get_config(
         self,
     ) -> Dict[str, Any]:
-        optim = tf.keras.optimizers.serialize(self.optim)
+        optim = tf_keras.optimizers.serialize(self.optim)
         return {"optim": optim}
 
     def get_state(
         self,
     ) -> Dict[str, Any]:
         specs = {
             key: (val.shape.as_list(), val.dtype.name)
             for key, val in self._vars.items()
         }
+        variables = self._get_optimizer_variables()
         state = TensorflowVector(
-            {var.name: var.value() for var in self.optim.variables()}
+            {str(i): v.value() for i, v in enumerate(variables)}
         )
         return {"specs": specs, "state": state}
 
+    def _get_optimizer_variables(
+        self,
+    ) -> List[tf.Variable]:
+        """Access wrapped optimizer's variables as 'tf.Variable' instances."""
+        if hasattr(tf_keras, "version") and tf_keras.version().startswith("3"):
+            return [var.value for var in self.optim.variables]
+        return self.optim.variables()
+
     def set_state(
         self,
         state: Dict[str, Any],
     ) -> None:
         for key in ("specs", "state"):
             if key not in state:
                 raise KeyError(
@@ -235,13 +249,13 @@
         # Restore weight variables' specifications from the input state dict.
         self.reset()  # note: this also updates the device policy
         with tf.device(self._device):
             self._vars = {
                 key: tf.Variable(tf.zeros(shape, dtype), name=key)
                 for key, (shape, dtype) in state["specs"].items()
             }
-            self.optim.build(self._vars.values())
+            self.optim.build(list(self._vars.values()))
         # Restore optimizer variables' values from the input state dict.
-        opt_vars = {var.name: var for var in self.optim.variables()}
+        opt_vars = self._get_optimizer_variables()
         with tf.device(self._device):
-            for key, val in state["state"].coefs.items():
-                opt_vars[key].assign(val, read_value=False)
+            for var, val in zip(opt_vars, state["state"].coefs.values()):
+                var.assign(val, read_value=False)
```

### Comparing `declearn-2.3.2/declearn/model/tensorflow/_vector.py` & `declearn-2.4.0/declearn/model/tensorflow/_vector.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,33 +16,34 @@
 # limitations under the License.
 
 """TensorflowVector data arrays container."""
 
 import warnings
 from typing import (
     # fmt: off
-    Any, Callable, Dict, Optional, Set, Tuple, Type, TypeVar, Union
+    Any, Callable, Dict, List, Optional, Set, Tuple, Type, TypeVar, Union
 )
 
 # fmt: off
 import numpy as np
 import tensorflow as tf  # type: ignore
 # false-positive; pylint: disable=no-name-in-module
 from tensorflow.python.framework.ops import EagerTensor  # type: ignore
 # pylint: enable=no-name-in-module
 from typing_extensions import Self  # future: import from typing (Py>=3.11)
 # fmt: on
 
-from declearn.model.api import Vector, register_vector_type
+from declearn.model.api import Vector, VectorSpec, register_vector_type
 from declearn.model.sklearn import NumpyVector
 from declearn.model.tensorflow.utils import (
     add_indexed_slices_support,
     preserve_tensor_device,
     select_device,
 )
+from declearn.model._utils import flatten_numpy_arrays, unflatten_numpy_arrays
 from declearn.utils import get_device_policy
 
 
 __all__ = [
     "TensorflowVector",
 ]
 
@@ -308,7 +309,77 @@
         # than tf.pow as results tend to differ for small values.
         if isinstance(other, (int, float)):
             if other == 2:
                 return self.apply_func(tf_op_sqre)
             if other == 0.5:
                 return self.apply_func(tf_op_sqrt)
         return super().__pow__(other)
+
+    def get_vector_specs(
+        self,
+    ) -> VectorSpec:
+        # Add IndexedSlices information to the base specs.
+        specs = super().get_vector_specs()
+        slices = [
+            name
+            for name in specs.names
+            if isinstance(self.coefs[name], tf.IndexedSlices)
+        ]
+        if slices:
+            specs.kwargs["slices"] = slices
+        return specs
+
+    def flatten(
+        self,
+    ) -> Tuple[List[float], VectorSpec]:
+        v_spec = self.get_vector_specs()
+        arrays = []  # type: List[np.ndarray]
+        for name in v_spec.names:
+            if isinstance(self.coefs[name], tf.IndexedSlices):
+                warnings.warn(
+                    "Flattening a 'tf.IndexedSlices' structure into an "
+                    "exhaustive list of floats. This may result in a high "
+                    "memory cost.",
+                    UserWarning,
+                )
+                arrays.append(
+                    np.array(tf.convert_to_tensor(self.coefs[name]).numpy())
+                )
+            else:
+                arrays.append(np.array(self.coefs[name].numpy()))
+        values = flatten_numpy_arrays(arrays)
+        return values, v_spec
+
+    @classmethod
+    def unflatten(
+        cls,
+        values: List[float],
+        v_spec: VectorSpec,
+    ) -> Self:
+        # Convert values to numpy arrays.
+        shapes = [v_spec.shapes[name] for name in v_spec.names]
+        dtypes = [v_spec.dtypes[name] for name in v_spec.names]
+        arrays = unflatten_numpy_arrays(values, shapes, dtypes)
+        # Gather information about IndexedSlices and prepare a list of tensors.
+        slices = v_spec.kwargs.get("slices", [])
+        tf_dat = {}  # Dict[str, Union[tf.Tensor, tf.IndexedSlices]]
+        # Convert numpy arrays back to tensorflow structures.
+        # Operate under the current device-placement policy.
+        policy = get_device_policy()
+        device = select_device(gpu=policy.gpu, idx=policy.idx)
+        with tf.device(device):
+            for name, array in zip(v_spec.names, arrays):
+                # Recover IndexedSlices structures from dense arrays.
+                if name in slices:
+                    non_zero = np.any(
+                        array != 0.0, axis=tuple(range(1, array.ndim))
+                    )
+                    ind = np.where(non_zero)[0].astype("int32")
+                    tf_dat[name] = tf.IndexedSlices(
+                        values=tf.convert_to_tensor(array[non_zero]),
+                        indices=tf.convert_to_tensor(ind),
+                        dense_shape=tf.convert_to_tensor(array.shape),
+                    )
+                # Otherwise, merely convert arrays to tensors.
+                else:
+                    tf_dat[name] = tf.convert_to_tensor(array)
+        return cls(tf_dat)
```

### Comparing `declearn-2.3.2/declearn/model/tensorflow/utils/__init__.py` & `declearn-2.4.0/declearn/model/tensorflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/model/tensorflow/utils/_gpu.py` & `declearn-2.4.0/declearn/model/tensorflow/utils/_gpu.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,20 @@
 
 """Utils for GPU support and device management in tensorflow."""
 
 import functools
 import warnings
 from typing import Any, Callable, Optional, Union
 
+# fmt: off
+# pylint: disable=import-error,no-name-in-module
 import tensorflow as tf  # type: ignore
+import tensorflow.keras as tf_keras  # type: ignore
+# pylint: enable=import-error,no-name-in-module
+# fmt: on
 
 
 __all__ = [
     "move_layer_to_device",
     "preserve_tensor_device",
     "select_device",
 ]
@@ -78,17 +83,17 @@
         )
         idx = 0
     # Return the selected device.
     return devices[idx]
 
 
 def move_layer_to_device(
-    layer: tf.keras.layers.Layer,
+    layer: tf_keras.layers.Layer,
     device: Union[tf.config.LogicalDevice, str],
-) -> tf.keras.layers.Layer:
+) -> tf_keras.layers.Layer:
     """Create a copy of an input keras layer placed on a given device.
 
     This functions creates a copy of the input layer and of all its weights.
     It may therefore be costful and should be used sparingly, to move away
     variables on a device where all further computations are expected to be
     run.
 
@@ -97,21 +102,21 @@
     layer: tf.keras.layers.Layer
         Keras layer that needs moving to another device.
     device: tf.config.LogicalDevice or str
         Device where to place the layer's weights.
 
     Returns
     -------
-    layer: tf.keras.layers.Layer
+    layer: tf_keras.layers.Layer
         Copy of the input layer, with its weights backed on `device`.
     """
-    config = tf.keras.layers.serialize(layer)
+    config = tf_keras.layers.serialize(layer)
     weights = layer.get_weights()
     with tf.device(device):
-        layer = tf.keras.layers.deserialize(config)
+        layer = tf_keras.layers.deserialize(config)
         layer.set_weights(weights)
     return layer
 
 
 def preserve_tensor_device(
     func: Callable[..., tf.Tensor],
 ) -> Callable[..., tf.Tensor]:
```

### Comparing `declearn-2.3.2/declearn/model/tensorflow/utils/_loss.py` & `declearn-2.4.0/declearn/model/tensorflow/utils/_loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,107 +17,112 @@
 
 """Function to parse and/or wrap a keras loss for use with declearn."""
 
 import inspect
 
 from typing import Any, Callable, Dict, Optional, Union
 
+# fmt: off
+# pylint: disable=import-error,no-name-in-module
 import tensorflow as tf  # type: ignore
+import tensorflow.keras as tf_keras  # type: ignore
+# pylint: enable=import-error,no-name-in-module
+# fmt: on
 
 
 __all__ = [
     "build_keras_loss",
 ]
 
 
 # alias for loss functions' signature in keras
 CallableLoss = Callable[[tf.Tensor, tf.Tensor], tf.Tensor]
 
 
-@tf.keras.utils.register_keras_serializable(package="declearn")
-class LossFunction(tf.keras.losses.Loss):
+@tf_keras.utils.register_keras_serializable(package="declearn")
+class LossFunction(tf_keras.losses.Loss):
     """Generic loss function container enabling reduction strategy control."""
 
     def __init__(
         self,
         loss_fn: Union[str, CallableLoss],
-        reduction: str = tf.keras.losses.Reduction.NONE,
+        reduction: str = tf_keras.losses.Reduction.NONE,
         name: Optional[str] = None,
     ) -> None:
-        super().__init__(reduction, name)
-        self.loss_fn = tf.keras.losses.deserialize(loss_fn)
+        super().__init__(reduction=reduction, name=name)
+        self.loss_fn = tf_keras.losses.deserialize(loss_fn)
 
     def call(
         self,
         y_true: tf.Tensor,
         y_pred: tf.Tensor,
     ) -> tf.Tensor:
         # inherited docstring; pylint: disable=missing-docstring
         return self.loss_fn(y_true, y_pred)
 
     def get_config(
         self,
     ) -> Dict[str, Any]:
         # inherited docstring; pylint: disable=missing-docstring
         config = super().get_config()  # type: Dict[str, Any]
-        config["loss_fn"] = tf.keras.losses.serialize(self.loss_fn)
+        config["loss_fn"] = tf_keras.losses.serialize(self.loss_fn)
         return config
 
 
 def build_keras_loss(
-    loss: Union[str, tf.keras.losses.Loss, CallableLoss],
-    reduction: str = tf.keras.losses.Reduction.NONE,
-) -> tf.keras.losses.Loss:
+    loss: Union[str, tf_keras.losses.Loss, CallableLoss],
+    reduction: str = tf_keras.losses.Reduction.NONE,
+) -> tf_keras.losses.Loss:
     """Type-check, deserialize and/or wrap a keras loss into a Loss object.
 
     Parameters
     ----------
     loss: str or tf.keras.losses.Loss or function(y_true, y_pred)->loss
         Either a keras Loss object, the name of a keras loss, or a loss
         function that needs wrapping into a Loss object.
     reduction: str, default=`tf.keras.losses.Reduction.NONE`
         Reduction scheme to apply on point-wise loss values.
 
     Returns
     -------
-    loss_obj: tf.keras.losses.Loss
+    loss_obj: tf_keras.losses.Loss
         Loss object, configured to apply the `reduction` scheme.
     """
     # Case when 'loss' is already a Loss object.
-    if isinstance(loss, tf.keras.losses.Loss):
+    if isinstance(loss, tf_keras.losses.Loss):
         loss.reduction = reduction
     # Case when 'loss' is a string: deserialize and/or wrap into a Loss object.
     elif isinstance(loss, str):
         loss = get_keras_loss_from_string(name=loss, reduction=reduction)
     # Case when 'loss' is a function: wrap it up using LossFunction.
     elif inspect.isfunction(loss):
         loss = LossFunction(loss, reduction=reduction)
     # Case when 'loss' is of invalid type: raise a TypeError.
-    if not isinstance(loss, tf.keras.losses.Loss):
+    if not isinstance(loss, tf_keras.losses.Loss):
         raise TypeError(
             "'loss' should be a keras Loss object or the name of one."
         )
     # Otherwise, properly configure the reduction scheme and return.
     return loss
 
 
 def get_keras_loss_from_string(
     name: str,
     reduction: str,
-) -> tf.keras.losses.Loss:
+) -> tf_keras.losses.Loss:
     """Instantiate a keras Loss object from a registered string identifier.
 
     - If `name` matches a Loss registration name, return an instance.
     - If it matches a loss function registration name, return either
       an instance from its name-matching Loss subclass, or a custom
       Loss subclass instance wrapping the function.
     - If it does not match anything, raise a ValueError.
     """
-    loss = tf.keras.losses.deserialize(name)
-    if isinstance(loss, tf.keras.losses.Loss):
+    loss = tf_keras.losses.deserialize(name)
+    if isinstance(loss, tf_keras.losses.Loss):
         loss.reduction = reduction
         return loss
     if inspect.isfunction(loss):
         try:
             name = "".join(word.capitalize() for word in name.split("_"))
             return get_keras_loss_from_string(name, reduction)
         except ValueError:
```

### Comparing `declearn-2.3.2/declearn/model/tensorflow/utils/_slices.py` & `declearn-2.4.0/declearn/model/tensorflow/utils/_slices.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/model/torch/__init__.py` & `declearn-2.4.0/declearn/model/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/model/torch/_model.py` & `declearn-2.4.0/declearn/model/torch/_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -249,14 +249,15 @@
         # Unpack inputs and clear gradients' history.
         inputs, y_true, s_wght = self._unpack_batch(batch)
         self._model.zero_grad()
         # Run the forward and backward pass to compute gradients.
         y_pred = self._model(*inputs)
         loss = self._compute_loss(y_pred, y_true, s_wght)
         loss.backward()
+        self._loss_history.append(float(loss.detach().cpu().numpy().mean()))
         # Collect weights' gradients and return them in a Vector container.
         grads = {
             k: p.grad.detach().clone()
             for k, p in self._raw_model.named_parameters()
             if p.requires_grad
         }
         return TorchVector(grads)
@@ -269,15 +270,15 @@
     ]:
         """Unpack and enforce Tensor conversion to an input data batch."""
         # fmt: off
         # Define an array-to-tensor conversion routine.
         def convert(data: Any) -> Optional[torch.Tensor]:
             if (data is None) or isinstance(data, torch.Tensor):
                 return data
-            return torch.from_numpy(data)  # pylint: disable=no-member
+            return torch.from_numpy(data)
         # Ensure inputs is a list.
         inputs, y_true, s_wght = batch
         if not isinstance(inputs, (tuple, list)):
             inputs = [inputs]
         # Ensure output data was converted to Tensor.
         output = (list(map(convert, inputs)), convert(y_true), convert(s_wght))
         return output  # type: ignore
@@ -316,15 +317,18 @@
         inputs, y_true, s_wght = self._unpack_batch(batch)
         grads_fn = self._build_samplewise_grads_fn(
             inputs=len(inputs),
             y_true=(y_true is not None),
             s_wght=(s_wght is not None),
         )
         with torch.no_grad():
-            grads = grads_fn(inputs, y_true, s_wght, clip=clip)  # type: ignore
+            grads, loss = grads_fn(
+                inputs, y_true, s_wght, clip=clip
+            )  # type: ignore
+            self._loss_history.append(float(loss.cpu().numpy().mean()))
         return TorchVector(grads)
 
     @functools.lru_cache
     def _build_samplewise_grads_fn(
         self,
         inputs: int,
         y_true: bool,
@@ -365,15 +369,15 @@
             for key, upd in updates.coefs.items():
                 tns = self._raw_model.get_parameter(key)
                 tns.add_(upd.to(tns.device))
 
     def compute_batch_predictions(
         self,
         batch: Batch,
-    ) -> Tuple[np.ndarray, np.ndarray, Optional[np.ndarray],]:
+    ) -> Tuple[np.ndarray, np.ndarray, Optional[np.ndarray]]:
         inputs, y_true, s_wght = self._unpack_batch(batch)
         if y_true is None:
             raise TypeError(
                 "`TorchModel.compute_batch_predictions` received a "
                 "batch with `y_true=None`, which is unsupported. Please "
                 "correct the inputs, or override this method to support "
                 "creating labels from the base inputs."
@@ -406,16 +410,16 @@
         setattr(self, "__eval_called", True)
 
     def loss_function(
         self,
         y_true: np.ndarray,
         y_pred: np.ndarray,
     ) -> np.ndarray:
-        tns_pred = torch.from_numpy(y_pred)  # pylint: disable=no-member
-        tns_true = torch.from_numpy(y_true)  # pylint: disable=no-member
+        tns_pred = torch.from_numpy(y_pred)
+        tns_true = torch.from_numpy(y_true)
         s_loss = self._loss_fn(tns_pred, tns_true)
         return s_loss.cpu().numpy().squeeze()
 
     def update_device_policy(
         self,
         policy: Optional[DevicePolicy] = None,
     ) -> None:
```

### Comparing `declearn-2.3.2/declearn/model/torch/_optim.py` & `declearn-2.4.0/declearn/model/torch/_optim.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,14 @@
 
     def _init_optimizer(self, gradients: TorchVector) -> torch.optim.Optimizer:
         """Instantiate and return a torch Optimizer to make use of.
 
         Place the artifical parameters and optimizer states on the
         same device as the input gradients.
         """
-        # false-positive on torch.zeros_like; pylint: disable=no-member
         self._params = {
             key: torch.nn.Parameter(torch.zeros_like(grad))
             for key, grad in gradients.coefs.items()
         }
         return self.optim_cls(list(self._params.values()), **self.kwargs)
 
     def reset(self) -> None:
@@ -296,27 +295,27 @@
             return None
         # Consult the global device policy to place the variables and states.
         policy = get_device_policy()
         device = select_device(gpu=policy.gpu, idx=policy.idx)
         # Restore weight variables' specifications from the input state dict.
         self._params = {}
         for key, (shape, dtype) in state["specs"].items():
-            zeros = torch.zeros(  # false-positive; pylint: disable=no-member
+            zeros = torch.zeros(
                 tuple(shape), dtype=getattr(torch, dtype), device=device
             )
             self._params[key] = torch.nn.Parameter(zeros)
         self._optim = self.optim_cls(
             list(self._params.values()), **self.kwargs
         )
         # Restore optimizer variables' values from the input state dict.
         sdict = self._optim.state_dict()
         sdict["state"] = {
             key: {
                 k: (
-                    torch.from_numpy(v).to(device)  # pylint: disable=no-member
+                    torch.from_numpy(v).to(device)
                     if isinstance(v, np.ndarray)
                     else v
                 )
                 for k, v in group.items()
             }
             for key, group in state["state"]
         }
```

### Comparing `declearn-2.3.2/declearn/model/torch/_samplewise/__init__.py` & `declearn-2.4.0/declearn/model/torch/_samplewise/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,18 +58,20 @@
     y_true: bool
         Whether a true labels tensor is provided.
     s_wght: bool
         Whether a sample weights tensor is provided.
 
     Returns
     -------
-    grads_fn: callable[[inputs, y_true, s_wght, clip], grads]
+    grads_fn: callable[[inputs, y_true, s_wght, clip], (grads, loss)]
         Function that efficiently computes and returns sample-wise gradients
         wrt trainable model parameters based on a batch of inputs, with opt.
         clipping based on a maximum l2-norm value `clip`.
+        It returns the sample-wise gradients as a dict of tensors with their
+        parameter name as key, plus the sample-wise loss values as a tensor.
 
     Note
     ----
     The underlying backend code depends on your Torch version, so as to
     enable optimizing operations using either `functorch` for torch 1.1X
     or `torch.func` for torch 2.X.
     """
```

### Comparing `declearn-2.3.2/declearn/model/torch/_samplewise/functorch.py` & `declearn-2.4.0/declearn/model/torch/_samplewise/functorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,21 +51,21 @@
             s_loss.mul_(s_wght.to(s_loss.device))
         return s_loss.mean()
 
     def grads_fn(inputs, y_true, s_wght, clip=None):
         """Compute gradients and optionally clip them."""
         params, idxgrd, pnames = get_params(model)
         buffers = list(model.buffers())
-        gfunc = functorch.grad(run_forward, argnums=tuple(idxgrd))
-        grads = gfunc(
+        gfunc = functorch.grad_and_value(run_forward, argnums=tuple(idxgrd))
+        grads, loss = gfunc(
             inputs, y_true, (None if clip else s_wght), buffers, *params
         )
         if clip:
             clip_and_scale_grads_inplace(grads, clip, s_wght)
-        return dict(zip(pnames, grads))
+        return dict(zip(pnames, grads)), loss.detach()
 
     # Wrap the former function to compute and clip sample-wise gradients.
     in_dims = ([0] * inputs, 0 if y_true else None, 0 if s_wght else None)
     return functorch.vmap(grads_fn, in_dims, randomness="same")
 
 
 def get_params(
```

### Comparing `declearn-2.3.2/declearn/model/torch/_samplewise/shared.py` & `declearn-2.4.0/declearn/model/torch/_samplewise/shared.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Shared code for torch-version-dependent backend code."""
 
-from typing import Callable, Dict, Iterable, List, Optional
+from typing import Callable, Dict, Iterable, List, Optional, Tuple
 
 import torch
 
 __all__ = [
     "GetGradientsFunction",
     "clip_and_scale_grads_inplace",
 ]
@@ -30,15 +30,15 @@
 GetGradientsFunction = Callable[
     [
         List[torch.Tensor],
         Optional[torch.Tensor],
         Optional[torch.Tensor],
         Optional[float],
     ],
-    Dict[str, torch.Tensor],
+    Tuple[Dict[str, torch.Tensor], torch.Tensor],
 ]
 """Signature for sample-wise gradients computation functions."""
 
 
 def clip_and_scale_grads_inplace(
     grads: Iterable[torch.Tensor],
     clip: float,
@@ -46,11 +46,10 @@
 ) -> None:
     """Clip a collection of tensors in-place, based on their euclidean norm.
 
     Also apply an optional weight tensor to scale the clipped gradients.
     """
     for grad in grads:
         norm = torch.norm(grad, p=2, keepdim=True)
-        # false-positive; pylint: disable=no-member
         grad.mul_(torch.clamp(clip / norm, max=1))
         if wght is not None:
             grad.mul_(wght.to(grad.device))
```

### Comparing `declearn-2.3.2/declearn/model/torch/_samplewise/torchfunc.py` & `declearn-2.4.0/declearn/model/torch/_samplewise/torchfunc.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,30 +47,32 @@
             model, [params, frozen, buffers], *inputs
         )
         s_loss = loss_fn(y_pred, y_true)
         if s_wght is not None:
             s_loss.mul_(s_wght.to(s_loss.device))
         return s_loss.mean()
 
-    get_grads = torch.func.grad(run_forward, argnums=0)
+    get_grads_and_loss = torch.func.grad_and_value(run_forward, argnums=0)
 
-    def get_clipped_grads(inputs, y_true, s_wght, clip=None):
+    def get_clipped_grads_and_loss(inputs, y_true, s_wght, clip=None):
         """Compute gradients and optionally clip them."""
         params, frozen = get_params(model)
         buffers = dict(model.named_buffers())
-        grads = get_grads(
+        grads, loss = get_grads_and_loss(
             params, frozen, buffers, inputs, y_true, None if clip else s_wght
         )
         if clip:
             clip_and_scale_grads_inplace(grads.values(), clip, s_wght)
-        return grads
+        return grads, loss.detach()
 
     # Wrap the former function to compute and clip sample-wise gradients.
     in_dims = ([0] * inputs, 0 if y_true else None, 0 if s_wght else None)
-    return torch.func.vmap(get_clipped_grads, in_dims, randomness="same")
+    return torch.func.vmap(
+        get_clipped_grads_and_loss, in_dims, randomness="same"
+    )
 
 
 def get_params(
     model: torch.nn.Module,
 ) -> Tuple[Dict[str, torch.nn.Parameter], Dict[str, torch.nn.Parameter]]:
     """Return a model's parameters, split between trainable and frozen ones."""
     params = {}  # type: Dict[str, torch.nn.Parameter]
```

### Comparing `declearn-2.3.2/declearn/model/torch/_vector.py` & `declearn-2.4.0/declearn/model/torch/_vector.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """TorchVector data arrays container."""
 
 import warnings
-from typing import Any, Callable, Dict, Optional, Set, Tuple, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
 
 import numpy as np
 import torch
 from typing_extensions import Self  # future: import from typing (Py>=3.11)
 
-from declearn.model.api import Vector, register_vector_type
+from declearn.model.api import Vector, VectorSpec, register_vector_type
 from declearn.model.sklearn import NumpyVector
 from declearn.model.torch.utils import select_device
+from declearn.model._utils import flatten_numpy_arrays, unflatten_numpy_arrays
 from declearn.utils import get_device_policy
 
 
 __all__ = [
     "TorchVector",
 ]
 
@@ -67,31 +68,31 @@
       (accessed via `declearn.utils.get_device_policy`). Thus it may
       have a different device-placement schema than at dump time but
       should be coherent with that of `TorchModel` computations.
     """
 
     @property
     def _op_add(self) -> Callable[[Any, Any], Any]:
-        return torch.add  # pylint: disable=no-member
+        return torch.add
 
     @property
     def _op_sub(self) -> Callable[[Any, Any], Any]:
-        return torch.sub  # pylint: disable=no-member
+        return torch.sub
 
     @property
     def _op_mul(self) -> Callable[[Any, Any], Any]:
-        return torch.mul  # pylint: disable=no-member
+        return torch.mul
 
     @property
     def _op_div(self) -> Callable[[Any, Any], Any]:
-        return torch.div  # pylint: disable=no-member
+        return torch.div
 
     @property
     def _op_pow(self) -> Callable[[Any, Any], Any]:
-        return torch.pow  # pylint: disable=no-member
+        return torch.pow
 
     @property
     def compatible_vector_types(self) -> Set[Type[Vector]]:
         types = super().compatible_vector_types
         return types.union({NumpyVector, TorchVector})
 
     def __init__(self, coefs: Dict[str, torch.Tensor]) -> None:
@@ -100,15 +101,14 @@
     def _apply_operation(
         self,
         other: Any,
         func: Callable[[Any, Any], Any],
     ) -> Self:
         # Convert 'other' NumpyVector to a (CPU-backed) TorchVector.
         if isinstance(other, NumpyVector):
-            # false-positive; pylint: disable=no-member
             coefs = {
                 key: torch.from_numpy(val) for key, val in other.coefs.items()
             }
             other = TorchVector(coefs)
         # Ensure 'other' TorchVector shares this vector's device placement.
         if isinstance(other, TorchVector):
             coefs = {
@@ -140,17 +140,15 @@
     def unpack(
         cls,
         data: Dict[str, Any],
     ) -> Self:
         policy = get_device_policy()
         device = select_device(gpu=policy.gpu, idx=policy.idx)
         coefs = {
-            # false-positive on `torch.from_numpy`; pylint: disable=no-member
-            key: torch.from_numpy(dat).to(device)
-            for key, dat in data.items()
+            key: torch.from_numpy(dat).to(device) for key, dat in data.items()
         }
         return cls(coefs)
 
     def __eq__(
         self,
         other: Any,
     ) -> bool:
@@ -162,38 +160,61 @@
                 # false-positive on 'torch.equal'; pylint: disable=no-member
                 torch.equal(tns, other.coefs[key].to(tns.device))
                 for key, tns in self.coefs.items()
             )
         return valid
 
     def sign(self) -> Self:
-        # false-positive; pylint: disable=no-member
         return self.apply_func(torch.sign)
 
     def minimum(
         self,
         other: Union[Self, float],
     ) -> Self:
-        # false-positive; pylint: disable=no-member
         if isinstance(other, Vector):
             return self._apply_operation(other, torch.minimum)
         if isinstance(other, float):
-            other = torch.Tensor([other])  # type: ignore  # scalar Tensor
-        return self.apply_func(torch.minimum, other)
+            return self._operate_with_float(torch.minimum, other)
+        raise TypeError(  # pragma: no cover
+            f"Unsupported input type to '{self.__class__.__name__}.minimum'."
+        )
 
     def maximum(
         self,
         other: Union[Self, float],
     ) -> Self:
-        # false-positive; pylint: disable=no-member
         if isinstance(other, Vector):
             return self._apply_operation(other, torch.maximum)
         if isinstance(other, float):
-            other = torch.Tensor([other])  # type: ignore  # scalar Tensor
-        return self.apply_func(torch.maximum, other)
+            return self._operate_with_float(torch.maximum, other)
+        raise TypeError(  # pragma: no cover
+            f"Unsupported input type to '{self.__class__.__name__}.maximum'."
+        )
+
+    def _operate_with_float(
+        self,
+        func: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
+        other: float,
+    ) -> Self:
+        """Apply an operation on coefficients with a single float.
+
+        Handle tensor-conversion and device-placement issues that are
+        specific to (some) Torch (functions).
+        """
+        # Create Tensors wrapping the scalar on each required device.
+        device_other = {
+            device: torch.Tensor([other]).to(device)
+            for device in {val.device for val in self.coefs.values()}
+        }
+        # Apply the function to coefficients and re-wrap as a TorchVector.
+        coefs = {
+            key: func(val, device_other[val.device])
+            for key, val in self.coefs.items()
+        }
+        return self.__class__(coefs)
 
     def sum(
         self,
         axis: Optional[int] = None,
         keepdims: bool = False,
     ) -> Self:
         if isinstance(axis, int) or keepdims:
@@ -204,7 +225,26 @@
                 DeprecationWarning,
             )
         coefs = {
             key: val.sum(dim=axis, keepdims=keepdims)
             for key, val in self.coefs.items()
         }
         return self.__class__(coefs)
+
+    def flatten(
+        self,
+    ) -> Tuple[List[float], VectorSpec]:
+        v_spec = self.get_vector_specs()
+        arrays = self.pack()
+        values = flatten_numpy_arrays([arrays[name] for name in v_spec.names])
+        return values, v_spec
+
+    @classmethod
+    def unflatten(
+        cls,
+        values: List[float],
+        v_spec: VectorSpec,
+    ) -> Self:
+        shapes = [v_spec.shapes[name] for name in v_spec.names]
+        dtypes = [v_spec.dtypes[name] for name in v_spec.names]
+        arrays = unflatten_numpy_arrays(values, shapes, dtypes)
+        return cls.unpack(dict(zip(v_spec.names, arrays)))
```

### Comparing `declearn-2.3.2/declearn/model/torch/utils/__init__.py` & `declearn-2.4.0/declearn/model/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/model/torch/utils/_gpu.py` & `declearn-2.4.0/declearn/model/torch/utils/_gpu.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "select_device",
 ]
 
 
 def select_device(
     gpu: bool,
     idx: Optional[int] = None,
-) -> torch.device:  # pylint: disable=no-member
+) -> torch.device:
     """Select a backing device to use based on inputs and availability.
 
     Parameters
     ----------
     gpu: bool
         Whether to select a GPU device rather than the CPU one.
     idx: int or None, default=None
@@ -53,22 +53,22 @@
     Returns
     -------
     device: torch.device
         Selected torch device, with type "cpu" or "cuda".
     """
     # Case when instructed to use the CPU device.
     if not gpu:
-        return torch.device("cpu")  # pylint: disable=no-member
+        return torch.device("cpu")
     # Case when no GPU is available: warn and use the CPU instead.
     if gpu and not torch.cuda.is_available():
         warnings.warn(
             "Cannot use a GPU device: either CUDA is unavailable "
             "or no GPU is visible to torch."
         )
-        return torch.device("cpu")  # pylint: disable=no-member
+        return torch.device("cpu")
     # Case when the desired GPU is invalid: select another one.
     if (idx or 0) >= torch.cuda.device_count():
         warnings.warn(
             f"Cannot use GPU device n°{idx}: index is out-of-range.\n"
             f"Using GPU device n°{torch.cuda.current_device()} instead.",
             RuntimeWarning,
         )
```

### Comparing `declearn-2.3.2/declearn/optimizer/__init__.py` & `declearn-2.4.0/declearn/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/optimizer/_base.py` & `declearn-2.4.0/declearn/optimizer/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # fmt: off
     Any, Dict, List, Optional, Sequence, Tuple, Type, TypeVar, Union
 )
 
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.model.api import Model, Vector
-from declearn.optimizer.modules import OptiModule
+from declearn.optimizer.modules import AuxVar, OptiModule
 from declearn.optimizer.regularizers import Regularizer
 from declearn.typing import Batch
 
 __all__ = [
     "Optimizer",
 ]
 
@@ -89,19 +89,19 @@
         List of plug-in loss regularization modules composed into
         the optimizer's gradients-to-updates computation algorithm.
 
     API methods
     -----------
     - apply_gradients(Model, Vector) -> None:
         Update a Model based on a pre-computed Vector of gradients.
-    - collect_aux_var() -> Dict[str, Dict[str, Any]]:
+    - collect_aux_var() -> Dict[str, AuxVar]:
         Collect and package plug-in modules' auxiliary variables.
     - compute_updates_from_gradients(Model, Vector) -> Vector:
         Compute and return model updates based on pre-computed gradients.
-    - process_aux_var(Dict[str, Dict[str, Any]]) -> None:
+    - process_aux_var(Dict[str, AuxVar]) -> None:
         Pass auxiliary variables to plug-in modules for processing.
     - run_train_step(Model, batch) -> None:
         Compute gradients of a Model over a Batch and apply updates.
     - start_round() -> None:
         Signal that a new training round is starting to wrapped regularizers.
 
     References
@@ -306,62 +306,64 @@
         if self.w_decay:
             updates += self.w_decay * weights
         # Return ready-to-apply model updates.
         return -1.0 * updates
 
     def collect_aux_var(
         self,
-    ) -> Dict[str, Dict[str, Any]]:
+    ) -> Dict[str, AuxVar]:
         """Return auxiliary variables that need to be shared between nodes.
 
         Returns
         -------
-        aux_var: dict[str, dict[str, ...]]
+        aux_var:
             Dict that associates `module.collect_aux_var()` values
             to `module.name` keys for each and every module plugged
-            in this optimizer that does produce auxiliary variables.
+            in this optimizer that produces auxiliary variables.
         """
-        aux_var = {}  # type: Dict[str, Dict[str, Any]]
+        aux_var = {}  # type: Dict[str, AuxVar]
         for module in self.modules:
             auxv = module.collect_aux_var()
-            if auxv:
+            if auxv is not None:
                 name = module.aux_name or module.name
                 aux_var[name] = auxv
         return aux_var
 
     def process_aux_var(
         self,
-        aux_var: Dict[str, Dict[str, Any]],
+        aux_var: Dict[str, AuxVar],
     ) -> None:
         """Update plug-in modules based on received shared auxiliary variables.
 
         Received auxiliary variables will be passed to this optimizer's
         modules' `process_aux_var` method, mapped based on `module.name`.
 
         Parameters
         ----------
-        aux_var: dict[str, dict[str, ...]]
+        aux_var: dict[str, AuxVar]
             Auxiliary variables received from the counterpart optimizer
             (on the other side of the client/server relationship), that
-            are to be a {`module.name`: `module.collect_aux_var()`} *or*
-            a {`module.name`: {client: `module.collect_aux_var()`}} dict
-            (depending on which side this optimizer is on).
+            are packed as a `{module.name: module.auxvar_cls}` dict for
+            modules that do use auxiliary variables.
+            When auxiliary variables from multiple peers are due to be
+            processed, they must be aggregated prior to being passed to
+            this method.
 
         Raises
         ------
         KeyError
             If a key from `aux_var` does not match the name of any module
             plugged in this optimizer (i.e. if received variables cannot
             be mapped to a destinatory module).
         """
         modules = {
             (module.aux_name or module.name): module for module in self.modules
         }
         for name, auxv in aux_var.items():
-            module = modules.get(name)
+            module = modules.get(name, None)
             if module is None:
                 raise KeyError(
                     f"No module with name '{name}' is available to receive "
                     "auxiliary variables."
                 )
             module.process_aux_var(auxv)
```

### Comparing `declearn-2.3.2/declearn/optimizer/_utils.py` & `declearn-2.4.0/declearn/optimizer/_utils.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/optimizer/modules/__init__.py` & `declearn-2.4.0/declearn/optimizer/modules/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Optimizer gradients-alteration algorithms, implemented as plug-in modules.
 
-API base class
---------------
+API base classes
+----------------
+* [AuxVar][declearn.optimizer.modules.AuxVar]:
+    Abstract base class for OptiModule auxiliary variables.
 * [OptiModule][declearn.optimizer.modules.OptiModule]:
     Abstact base class for optimizer plug-in algorithms.
 
 Adaptive learning-rate algorithms
 ---------------------------------
 * [AdaGradModule][declearn.optimizer.modules.AdaGradModule]:
     AdaGrad algorithm.
@@ -60,17 +62,20 @@
 ------------------
 Scaffold is implemented as a pair of complementary modules:
 
 * [ScaffoldClientModule][declearn.optimizer.modules.ScaffoldClientModule]:
     Client-side Scaffold module.
 * [ScaffoldServerModule][declearn.optimizer.modules.ScaffoldServerModule]:
     Server-side Scaffold module.
+* [ScaffoldAuxVar][declearn.optimizer.modules.ScaffoldAuxVar]:
+    AuxVar subclass for Scaffold modules.
 """
 
 from ._api import (
+    AuxVar,
     OptiModule,
 )
 from ._adaptive import (
     AdaGradModule,
     AdamModule,
     RMSPropModule,
     YogiModule,
@@ -85,10 +90,11 @@
     YogiMomentumModule,
 )
 from ._noise import (
     GaussianNoiseModule,
     NoiseModule,
 )
 from ._scaffold import (
+    ScaffoldAuxVar,
     ScaffoldClientModule,
     ScaffoldServerModule,
 )
```

### Comparing `declearn-2.3.2/declearn/optimizer/modules/_adaptive.py` & `declearn-2.4.0/declearn/optimizer/modules/_adaptive.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/optimizer/modules/_api.py` & `declearn-2.4.0/declearn/optimizer/modules/_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,36 +13,64 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Base API for plug-in gradients-alteration algorithms."""
 
-from abc import ABCMeta, abstractmethod
-from typing import Any, ClassVar, Dict, Optional, TypeVar
+import abc
+import dataclasses
+from typing import Any, ClassVar, Dict, Generic, Optional, Type, TypeVar
 
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.model.api import Vector
 from declearn.utils import (
+    Aggregate,
     access_registered,
     create_types_registry,
     register_type,
 )
 
 __all__ = [
+    "AuxVar",
     "OptiModule",
 ]
 
 
 T = TypeVar("T")
 
 
+@dataclasses.dataclass
+class AuxVar(Aggregate, base_cls=True, register=False, metaclass=abc.ABCMeta):
+    """Abstract base class for OptiModule auxiliary variables.
+
+    Each and every `OptiModule` subclass that requires information to be
+    exchanged is expected to be coupled with one (or multiple) `AuxVar`
+    subtype(s). These may be used to transmit information from a server
+    to its clients, and/or to exchange and aggregate data from clients
+    into a single `AuxVar` instance to be processed by the server.
+
+    This class also defines whether contents are compatible with secure
+    aggregation, and whether some fields should remain in cleartext no
+    matter what.
+
+    Note that subclasses are automatically type-registered, and should be
+    decorated as `dataclasses.dataclass`. To prevent registration, simply
+    pass `register=False` at inheritance.
+    """
+
+    _group_key = "AuxVar"
+
+
+AuxVarT = TypeVar("AuxVarT", bound=AuxVar)
+
+
 @create_types_registry
-class OptiModule(metaclass=ABCMeta):
+class OptiModule(Generic[AuxVarT], metaclass=abc.ABCMeta):
     """Abstract class defining an API to implement gradients adaptation tools.
 
     The aim of this abstraction (which itself operates on the Vector
     abstraction, so as to provide framework-agnostic algorithms) is
     to enable implementing unitary gradients-adaptation bricks that
     can easily and modularly be composed into complex algorithms.
 
@@ -70,26 +98,29 @@
     Overridable
     -----------
     The following methods may be overridden to implement information-
     passing and parallel behaviors between client/server module pairs.
     As defined at `OptiModule` level, they have no effect and may thus
     be safely ignored when implementing self-contained algorithms.
 
-    - collect_aux_var() -> Optional[Dict[str, Any]]:
-        Emit a JSON-serializable dict of auxiliary variables,
-        to be received by a counterpart of this module on the
+    - collect_aux_var() -> Optional[AuxVar]:
+        Emit an `AuxVar` instance holding auxiliary variables,
+        that may be shared with peers, aggregated across them,
+        and eventually processed by a counterpart module on the
         other side of the client/server relationship.
-    - process_aux_var(Dict[str, Any]) -> None:
-        Process a dict of auxiliary variables, received from
-        a counterpart to this module on the other side of the
-        client/server relationship.
+    - process_aux_var(AuxVar) -> None:
+        Process auxiliary variables received from a counterpart
+        module on the other side of the client/server relationship.
     - aux_name: optional[str] class attribute, default=None
         Name to use when sending or receiving auxiliary variables
         between synchronous client/server modules, that therefore
         need to share the *same* `aux_name`.
+    - auxvar_cls: optional[type[AuxVar]] class attribute, default=None
+        Type of `AuxVar` used by this module (defining the actual
+        signature of `collect_aux_var` and `process_aux_var`).
 
     Inheritance
     -----------
     When a subclass inheriting from `OptiModule` is declared, it is
     automatically registered under the "OptiModule" group using its
     class-attribute `name`. This can be prevented by adding `register=False`
     to the inheritance specs (e.g. `class MyCls(OptiModule, register=False)`).
@@ -103,25 +134,28 @@
     """Optional aux-var-sharing identifier of the class.
 
     This name may be shared by a pair of OptiModule classes, designed
     to operate on the client and server side respectively. It should
     be unique to that pair of classes across all OptiModule classes.
     """
 
+    auxvar_cls: Optional[Type[AuxVar]] = None
+    """Optional `AuxVar` subtype used by this module and its counterpart."""
+
     def __init_subclass__(
         cls,
         register: bool = True,
         **kwargs: Any,
     ) -> None:
         """Automatically type-register OptiModule subclasses."""
         super().__init_subclass__(**kwargs)
         if register:
             register_type(cls, cls.name, group="OptiModule")
 
-    @abstractmethod
+    @abc.abstractmethod
     def run(
         self,
         gradients: Vector[T],
     ) -> Vector[T]:
         """Apply the module's algorithm to input gradients.
 
         Please refer to the module's main docstring for details
@@ -139,87 +173,83 @@
             Modified input gradients. The output Vector should be
             fully compatible with the input one - only the values
             of the wrapped coefficients may have changed.
         """
 
     def collect_aux_var(
         self,
-    ) -> Optional[Dict[str, Any]]:
+    ) -> Optional[AuxVarT]:
         """Return auxiliary variables that need to be shared between nodes.
 
         Returns
         -------
-        aux_var: Optional[Dict[str, Any]]
-            Optional JSON-serializable dict of auxiliary variables that
-            are to be shared with a similarly-named OptiModule on the
-            other side of the client-server relationship.
+        aux_var: Optional[AuxVar]
+            Optional `AuxVar` instance holding auxiliary variables that
+            are to be shared with a counterpart OptiModule on the other
+            side of the client-server relationship.
 
         Notes
         -----
-        Specfications for the output and calling context depend on whether
-        the module is part of a client's optimizer or of the server's one:
+        The calling context depend ons whether the module is part of a
+        client's optimizer or of the server's one:
 
         - Client:
-            - `aux_var` is dict[str, any] or None.
             - `collect_aux_var` is expected to happen after taking a series
               of local optimization steps, before sending the local updates
               to the server for aggregation and further processing.
         - Server:
-            - `aux_var` may be None ; dict[str, any] (to send the same values
-              to each and every client) ; or dict[str, dict[str, any]] with
-              clients' names as keys and client-wise new aux_var as values
-              so as to send distinct values to the clients.
             - `collect_aux_var` is expected to happen when the global model
-              weights are ready to be shared with clients, i.e. at the very
-              end of a training round or at the beginning of the training
-              process.
+              weights are ready to be shared with clients, i.e. either at
+              the very end or very beginning of a training round.
         """
         return None
 
     def process_aux_var(
         self,
-        aux_var: Dict[str, Any],
+        aux_var: AuxVarT,
     ) -> None:
         """Update this module based on received shared auxiliary variables.
 
         Parameters
         ----------
-        aux_var: dict[str, any]
-            JSON-serializable dict of auxiliary variables that are to be
-            processed by this module at the start of a training round (on
-            the client side) or before processing global updates (on the
-            server side).
+        aux_var:
+            Auxiliary variables that are to be processed by this module,
+            emitted by a counterpart OptiModule on the other side of the
+            client-server relationship.
 
         Notes
         -----
-        Specfications for the inputs and calling context depend on whether
-        the module is part of a client's optimizer or of the server's one:
+        The calling context depends on whether the module is part of a
+        client's optimizer or of the server's one:
 
         - Client:
-            - `aux_var` is dict[str, any] and may be client-specific.
             - `process_aux_var` is expected to happen at the beginning of
               a training round to define gradients' processing during the
               local optimization steps taken through that round.
         - Server:
-            - `aux_var` is dict[str, dict[str, any]] with clients' names as
-              primary keys and client-wise collected aux_var as values.
             - `process_aux_var` is expected to happen upon receiving local
               updates (and, thus, aux_var), before the aggregated updates
               are computed and passed through the server optimizer (which
               comprises this module).
 
         Raises
         ------
         KeyError
-            If an expected auxiliary variable is missing.
+            If received auxiliary variables lack some required data.
+        NotImplementedError
+            If auxiliary variables are passed to a module that is not meant
+            to receive any.
         TypeError
-            If a variable is of unproper type, or if aux_var
-            is not formatted as it should be.
+            If `aux_var` or one of its fields has unproper type.
         """
-        # API-defining method; pylint: disable=unused-argument
+        if aux_var is not None:  # pragma: no cover
+            raise NotImplementedError(
+                f"'{self.__class__.__name__}.process_aux_var' was called, but"
+                " this class is not designed to receive auxiliary variables."
+            )
 
     def get_config(
         self,
     ) -> Dict[str, Any]:
         """Return a JSON-serializable dict with this module's parameters.
 
         The counterpart to this method is the `from_config` classmethod.
@@ -307,8 +337,12 @@
             state variables.
 
         Raises
         ------
         KeyError
             If an expected state variable is missing from `state`.
         """
-        # API-defining method; pylint: disable=unused-argument
+        if state:
+            raise KeyError(
+                f"'{self.__class__.__name__}.set_state' received some data, "
+                "but it is not implemented to actually use any."
+            )
```

### Comparing `declearn-2.3.2/declearn/optimizer/modules/_clipping.py` & `declearn-2.4.0/declearn/optimizer/modules/_clipping.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/optimizer/modules/_momentum.py` & `declearn-2.4.0/declearn/optimizer/modules/_momentum.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/optimizer/modules/_noise.py` & `declearn-2.4.0/declearn/optimizer/modules/_noise.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/optimizer/modules/_scaffold.py` & `declearn-2.4.0/declearn/optimizer/modules/_scaffold.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,58 +28,132 @@
 References
 ----------
 [1] Karimireddy et al., 2019.
     SCAFFOLD: Stochastic Controlled Averaging for Federated Learning.
     https://arxiv.org/abs/1910.06378
 """
 
+import dataclasses
+import uuid
 import warnings
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 from declearn.model.api import Vector
-from declearn.optimizer.modules._api import OptiModule
+from declearn.optimizer.modules._api import AuxVar, OptiModule
 
 __all__ = [
+    "ScaffoldAuxVar",
     "ScaffoldClientModule",
     "ScaffoldServerModule",
 ]
 
 
-class ScaffoldClientModule(OptiModule):
+@dataclasses.dataclass
+class ScaffoldAuxVar(AuxVar):
+    """AuxVar subclass for Scaffold.
+
+    - In Server -> Client direction, `state` should be specified.
+    - In Client -> Server direction, `delta` should be specified.
+    """
+
+    state: Union[Vector, float, None] = None
+    delta: Union[Vector, float, None] = None
+    clients: Set[str] = dataclasses.field(default_factory=set)
+
+    def __post_init__(
+        self,
+    ) -> None:
+        if ((self.state is None) + (self.delta is None)) != 1:
+            raise ValueError(
+                "'ScaffoldAuxVar' should have exactly one of 'state' or "
+                "'delta' specified as a Vector or conventional 0.0 value."
+            )
+        if isinstance(self.clients, list):
+            self.clients = set(self.clients)
+
+    @staticmethod
+    def aggregate_clients(
+        val_a: Set[str],
+        val_b: Set[str],
+    ) -> Set[str]:
+        """Custom aggregation rule for 'clients' field."""
+        return val_a.union(val_b)
+
+    @classmethod
+    def aggregate_state(
+        cls,
+        val_a: Union[Vector, float, None],
+        val_b: Union[Vector, float, None],
+    ) -> None:
+        """Custom aggregation rule for 'state' field, raising when due."""
+        if (val_a is not None) or (val_b is not None):
+            raise NotImplementedError(
+                "'ScaffoldAuxVar' should not be aggregating 'state' values."
+            )
+
+    def to_dict(
+        self,
+    ) -> Dict[str, Any]:
+        output = {}  # type: Dict[str, Any]
+        if self.state is not None:
+            output["state"] = self.state
+        if self.delta is not None:
+            output["delta"] = self.delta
+        if self.clients:
+            output["clients"] = list(self.clients)
+        return output
+
+    def prepare_for_secagg(
+        self,
+    ) -> Tuple[Dict[str, Any], Optional[Dict[str, Any]]]:
+        if self.state is not None:
+            raise NotImplementedError(
+                "'ScaffoldAuxVar' with 'state' should not undergo SecAgg."
+            )
+        return {"delta": self.delta}, {"clients": self.clients}
+
+
+class ScaffoldClientModule(OptiModule[ScaffoldAuxVar]):
     """Client-side Stochastic Controlled Averaging (SCAFFOLD) module.
 
     This module is to be added to the optimizer used by a federated-
     learning client, and expects that the server's optimizer use its
     counterpart module:
     [`ScaffoldServerModule`][declearn.optimizer.modules.ScaffoldServerModule].
 
     This module implements the following algorithm:
 
         Init:
+            state = 0
+            local = 0
             delta = 0
             _past = 0
             _step = 0
         Step(grads):
             _past += grads
             _step += 1
             grads = grads - delta
-        Send:
-            state = (_past / _step)
-        Receive(delta):
-            delta = delta
+        Send -> l_upd:
+            loc_n = (_past / _step)
+            l_upd = loc_n - local
+            local = loc_n
+        Receive(state):
+            state = state
+            delta = local - state
             reset(_past, _step) to 0
 
-    In other words, this module receives a "delta" variable from the
-    server instance which is set as the difference between a client-
-    specific state and a shared one, and corrects input gradients by
-    adding this delta to it. At the end of a training round (made of
-    multiple steps) it computes an updated client state based on the
-    accumulated sum of corrected gradients. This value is to be sent
-    to the server, that will emit a new value for the local delta in
-    return.
+    In other words, this module applies a correction term to each
+    and every input gradient, which is defined as the difference
+    between a local (node-specific) state and a global one, which
+    is received from a paired server-side module. At the end of a
+    training round (made of multiple steps) it computes an updated
+    local state based on the accumulated sum of raw input gradients.
+    The difference between the new and previous local states is then
+    shared with the server, that aggregates client-wise updates into
+    the new global state and emits it towards nodes in return.
 
     The SCAFFOLD algorithm is described in reference [1].
     The server-side correction of aggregated gradients, the storage
     of raw local and shared states, and the computation of the updated
     shared state and derived client-wise delta values are deferred to
     `ScaffoldServerModule`.
 
@@ -94,22 +168,25 @@
     References
     ----------
     [1] Karimireddy et al., 2019.
         SCAFFOLD: Stochastic Controlled Averaging for Federated Learning.
         https://arxiv.org/abs/1910.06378
     """
 
-    name: ClassVar[str] = "scaffold-client"
-    aux_name: ClassVar[str] = "scaffold"
+    name = "scaffold-client"
+    aux_name = "scaffold"
 
     def __init__(
         self,
     ) -> None:
         """Instantiate the client-side SCAFFOLD gradients-correction module."""
+        self.uuid = str(uuid.uuid4())
+        self.state = 0.0  # type: Union[Vector, float]
         self.delta = 0.0  # type: Union[Vector, float]
+        self.sglob = 0.0  # type: Union[Vector, float]
         self._grads = 0.0  # type: Union[Vector, float]
         self._steps = 0
 
     def run(
         self,
         gradients: Vector,
     ) -> Vector:
@@ -117,41 +194,53 @@
         self._grads = self._grads + gradients
         self._steps += 1
         # Apply state-based correction to outputs.
         return gradients - self.delta
 
     def collect_aux_var(
         self,
-    ) -> Dict[str, Any]:
+    ) -> Optional[ScaffoldAuxVar]:
         """Return auxiliary variables that need to be shared between nodes.
 
         Compute and package (without applying it) the updated value
         of the local state variable, so that the server may compute
         the updated shared state variable.
 
         Returns
         -------
-        aux_var: dict[str, any]
-            JSON-serializable dict of auxiliary variables that
-            are to be shared with a ScaffoldServerModule held
-            by the orchestrating server.
+        aux_var:
+            Auxiliary variables that are to be shared, aggregated and
+            eventually passed to a server-held `ScaffoldServerModule`.
 
         Warns
         -----
         RuntimeWarning
             If called on an instance that has not processed any gradients
             (via a call to `run`) since the last call to `process_aux_var`
             (or its instantiation).
         """
-        state = self._compute_updated_state()
-        return {"state": state}
+        # Warn and return an empty dict if no steps were run.
+        if not self._steps:
+            warnings.warn(
+                "Collecting auxiliary variables from a scaffold module "
+                "that was not run. The local state update was skipped, "
+                "and empty auxiliary variables are emitted.",
+                RuntimeWarning,
+            )
+            return None
+        # Compute the updated local state and assign it.
+        state_next = self._compute_updated_state()
+        state_updt = state_next - self.state
+        self.state = state_next
+        # Send the local state's update.
+        return ScaffoldAuxVar(delta=state_updt, clients={self.uuid})
 
     def _compute_updated_state(
         self,
-    ) -> Union[Vector, float]:
+    ) -> Vector:
         """Compute and return the updated value of the local state.
 
         Note: the computed update is *not* applied by this method.
 
         The computation implemented here is equivalent to "Option II"
         of the SCAFFOLD paper. In that paper, authors write that:
             c_i^+ = (c_i - c) + (x - y_i) / (K * eta_l)
@@ -160,247 +249,234 @@
         c is the shared global state and c_i is the local state.
 
         Noting that (x - y_i) is in fact the difference between the
         local model's weights before and after running K training
         steps, we rewrite it as eta_l * Sum_k(grad(y_i^k) - D_i),
         where we define D_i = (c_i - c). Thus we rewrite c_i^+ as:
             c_i^+ = D_i + (1/K)*Sum_k(grad(y_i^k) - D_i)
-        When then note that D_i is constant and can be taken out
-        of the summation term, leaving us with:
-            c_i^+ = Avg_k(grad(y_i^k))
+        Noting that D_i is constant across steps, we take it out of
+        the summation term, leaving us with:
+            c_i^+ = (1/K)*Sum_k(grad(y_i^k))
 
         Hence the new local state can be computed by averaging the
         gradients input to this module along the training steps.
         """
-        if not self._steps:
-            warnings.warn(
-                "Collecting auxiliary variables from a scaffold module "
-                "that was not run. Returned zero-valued scalar updates.",
-                category=RuntimeWarning,
+        if not self._steps:  # pragma: no cover
+            raise ValueError(
+                "Cannot compute an updated state when no steps were run."
+            )
+        if not isinstance(self._grads, Vector):  # pragma: no cover
+            raise TypeError(
+                "Internal gradients accumulator is not a Vector instance. "
+                "This seems to indicate that the Scaffold module received "
+                "improper-type inputs, which should not be possible."
             )
-            return 0.0
         return self._grads / self._steps
 
     def process_aux_var(
         self,
-        aux_var: Dict[str, Any],
+        aux_var: ScaffoldAuxVar,
     ) -> None:
         """Update this module based on received shared auxiliary variables.
 
         Collect the (local_state - shared_state) variable sent by server.
         Reset hidden variables used to compute the local state's updates.
 
         Parameters
         ----------
-        aux_var: dict[str, any]
-            JSON-serializable dict of auxiliary variables that are to be
-            processed by this module at the start of a training round (on
-            the client side).
-            Expected keys for this class: {"delta"}.
+        aux_var:
+            Auxiliary variables that are to be processed by this module,
+            emitted by a counterpart OptiModule on the other side of the
+            client-server relationship.
 
         Raises
         ------
         KeyError
-            If an expected auxiliary variable is missing.
+            If `aux_var` is empty.
         TypeError
-            If a variable is of unproper type, or if aux_var
-            is not formatted as it should be.
+            If `aux_var` has unproper type.
         """
-        # Expect a state variable and apply it.
-        delta = aux_var.get("delta", None)
-        if delta is None:
-            raise KeyError(
-                "Missing 'delta' key in ScaffoldClientModule's "
-                "received auxiliary variables."
-            )
-        if isinstance(delta, (float, Vector)):
-            self.delta = delta
-        else:
+        if not isinstance(aux_var, ScaffoldAuxVar):
             raise TypeError(
-                "Unsupported type for ScaffoldClientModule's "
-                "received auxiliary variable 'delta'."
+                f"'{self.__class__.__name__}.process_aux_var' received "
+                f"auxiliary variables of unproper type: '{type(aux_var)}'."
             )
-        # Reset local variables.
+        if aux_var.state is None:
+            raise KeyError(
+                "Missing 'state' data in auxiliary variables passed to "
+                f"'{self.__class__.__name__}.process_aux_var'."
+            )
+        # Assign new global state and update the local correction term.
+        self.sglob = aux_var.state
+        self.delta = self.state - self.sglob
+        # Reset internal local variables.
         self._grads = 0.0
         self._steps = 0
 
+    def get_state(
+        self,
+    ) -> Dict[str, Any]:
+        return {
+            "state": self.state,
+            "sglob": self.sglob,
+            "uuid": self.uuid,
+        }
 
-class ScaffoldServerModule(OptiModule):
+    def set_state(
+        self,
+        state: Dict[str, Any],
+    ) -> None:
+        for key in ("state", "sglob", "uuid"):
+            if key not in state:
+                raise KeyError(f"Missing required state variable '{key}'.")
+        # Assign received information.
+        self.state = state["state"]
+        self.sglob = state["sglob"]
+        self.uuid = state["uuid"]
+        # Reset correction state and internal local variables.
+        self.delta = self.state - self.sglob
+        self._grads = 0.0
+        self._steps = 0
+
+
+class ScaffoldServerModule(OptiModule[ScaffoldAuxVar]):
     """Server-side Stochastic Controlled Averaging (SCAFFOLD) module.
 
     This module is to be added to the optimizer used by a federated-
     learning server, and expects that the clients' optimizer use its
     counterpart module:
     [`ScaffoldClientModule`][declearn.optimizer.modules.ScaffoldClientModule].
 
     This module implements the following algorithm:
 
-        Init(clients):
-            state = 0
-            s_loc = {client: 0 for client in clients}
+        Init:
+            s_state = 0
+            clients = {}
         Step(grads):
             grads
-        Send:
-            delta = {client: (s_loc[client] - state); client in s_loc}
-        Receive(s_new = {client: state}):
-            s_upd = sum(s_new[client] - s_loc[client]; client in s_new)
-            s_loc.update(s_new)
-            state += s_upd / len(s_loc)
-
-    In other words, this module holds a shared state variable, and a
-    set of client-specific ones, which are zero-valued when created.
-    At the beginning of a training round it sends to each client its
-    delta variable, set to the difference between its current state
-    and the shared one, which is to be applied as a correction term
-    to local gradients. At the end of a training round, aggregated
-    gradients are corrected by substracting the shared state value
-    from them. Finally, updated local states received from clients
-    are recorded, and used to update the shared state variable, so
-    that new delta values can be sent to clients as the next round
-    of training starts.
+        Send -> state:
+            state = s_state / min(len(clients), 1)
+        Receive(delta=sum(state_i^t+1 - state_i^t), clients=set{uuid}):
+            s_state += delta
+            clients.update(clients)
+
+    In other words, this module holds a global state variable, set
+    to zero at instantiation. At the beginning of a training round
+    it sends it to all clients so that they can derive a correction
+    term for their processed gradients, based on a local state they
+    hold. At the end of a training round, client-wise local state
+    updates are sum-aggregated into an update for the global state
+    variable, which will be sent to clients at the start of the next
+    round. The sent state is always the average of the last known
+    local state from each and every known client.
 
     The SCAFFOLD algorithm is described in reference [1].
     The client-side correction of gradients and the computation of
     updated local states are deferred to `ScaffoldClientModule`.
 
     References
     ----------
     [1] Karimireddy et al., 2019.
         SCAFFOLD: Stochastic Controlled Averaging for Federated Learning.
         https://arxiv.org/abs/1910.06378
     """
 
-    name: ClassVar[str] = "scaffold-server"
-    aux_name: ClassVar[str] = "scaffold"
+    name = "scaffold-server"
+    aux_name = "scaffold"
+    auxvar_cls = ScaffoldAuxVar
 
     def __init__(
         self,
         clients: Optional[List[str]] = None,
     ) -> None:
         """Instantiate the server-side SCAFFOLD gradients-correction module.
 
         Parameters
         ----------
-        clients: list[str] or None, default=None
+        clients:
+            DEPRECATED and unused starting with declearn 2.4.
             Optional list of known clients' id strings.
-
-        Notes
-        -----
-        - If this module is used under a training strategy that has
-          participating clients vary across epochs, leaving `clients`
-          to None will affect the update rule for the shared state,
-          as it uses a (n_participating / n_total_clients) term, the
-          divisor of which will be incorrect (at least on the first
-          step, potentially on following ones as well).
-        - Similarly, listing clients that in fact do not participate
-          in training will have side effects on computations.
         """
-        self.state = 0.0  # type: Union[Vector, float]
-        self.s_loc = {}  # type: Dict[str, Union[Vector, float]]
-        if clients:
-            self.s_loc = {client: 0.0 for client in clients}
-
-    def get_config(
-        self,
-    ) -> Dict[str, Any]:
-        return {"clients": list(self.s_loc)}
+        self.s_state = 0.0  # type: Union[Vector, float]
+        self.clients = set()  # type: Set[str]
+        if clients:  # pragma: no cover
+            warnings.warn(
+                "ScaffoldServerModule's 'clients' argument has been deprecated"
+                " as of declearn v2.4, and no longer has any effect. It will"
+                " be removed in declearn 2.6 and/or 3.0.",
+                DeprecationWarning,
+            )
 
     def run(
         self,
         gradients: Vector,
     ) -> Vector:
         # Note: ScaffoldServer only manages auxiliary variables.
         return gradients
 
     def collect_aux_var(
         self,
-    ) -> Dict[str, Dict[str, Any]]:
+    ) -> ScaffoldAuxVar:
         """Return auxiliary variables that need to be shared between nodes.
 
-        Package client-wise `delta = (local_state - shared_state)` variables.
-
         Returns
         -------
         aux_var:
-            JSON-serializable dict of auxiliary variables that are to
-            be shared with the client-wise ScaffoldClientModule. This
-            dict has a `{client-name: {"delta": value}}` structure.
+            `ScaffoldAuxVar` instance holding auxiliary variables that are
+            to be shared with clients' `ScaffoldClientModule` instances.
         """
-        # Compute clients' delta variable, package them and return.
-        aux_var = {}  # type: Dict[str, Dict[str, Any]]
-        for client, state in self.s_loc.items():
-            delta = state - self.state
-            aux_var[client] = {"delta": delta}
-        return aux_var
+        # When un-initialized, send lightweight information.
+        if not self.clients:
+            return ScaffoldAuxVar(state=0.0)
+        # Otherwise, compute and return the current shared state.
+        return ScaffoldAuxVar(state=self.s_state / len(self.clients))
 
     def process_aux_var(
         self,
-        aux_var: Dict[str, Dict[str, Any]],
+        aux_var: ScaffoldAuxVar,
     ) -> None:
         """Update this module based on received shared auxiliary variables.
 
-        Collect updated local state variables sent by clients.
-        Update the global state variable based on the latter.
+        Update the global state variable based on the sum of client's
+        local state updates.
 
         Parameters
         ----------
-        aux_var: dict[str, dict[str, any]]
-            JSON-serializable dict of auxiliary variables that are to be
-            processed by this module before processing global updates.
-            This dict should have a `{client-name: {"state": value}}`
-            structure.
+        aux_var:
+            `ScaffoldAuxVar` resulting from the aggregation of clients'
+            `ScaffoldClientModule` auxiliary variables.
 
         Raises
         ------
         KeyError:
-            If an expected auxiliary variable is missing.
+            If `aux_var` is empty.
         TypeError:
-            If a variable is of unproper type, or if aux_var
-            is not formatted as it should be.
+            If `aux_var` is of unproper type.
         """
-        # Collect updated local states received from Scaffold client modules.
-        s_new = {}  # type: Dict[str, Union[Vector, float]]
-        for client, c_dict in aux_var.items():
-            if not isinstance(c_dict, dict):
-                raise TypeError(
-                    "ScaffoldServerModule requires auxiliary variables "
-                    "to be received as client-wise dictionaries."
-                )
-            if "state" not in c_dict:
-                raise KeyError(
-                    "Missing required 'state' key in auxiliary variables "
-                    f"received by ScaffoldServerModule from client '{client}'."
-                )
-            state = c_dict["state"]
-            if isinstance(state, float) and state == 0.0:
-                # Drop info from clients that have not processed gradients.
-                continue
-            if isinstance(state, (Vector, float)):
-                s_new[client] = state
-            else:
-                raise TypeError(
-                    "Unsupported type for auxiliary variable 'state' "
-                    f"received by ScaffoldServerModule from client '{client}'."
-                )
-        # Update the global and client-wise state variables.
-        update = sum(
-            state - self.s_loc.get(client, 0.0)
-            for client, state in s_new.items()
-        )
-        self.s_loc.update(s_new)
-        update = update / len(self.s_loc)
-        self.state = self.state + update
+        if not isinstance(aux_var, ScaffoldAuxVar):
+            raise TypeError(
+                f"'{self.__class__.__name__}.process_aux_var' received "
+                f"auxiliary variables of unproper type: '{type(aux_var)}'."
+            )
+        if aux_var.delta is None:
+            raise KeyError(
+                f"'{self.__class__.__name__}.process_aux_var' received "
+                "auxiliary variables with an empty 'delta' field."
+            )
+        # Update the list of known clients, and the sum of local states.
+        self.clients.update(aux_var.clients)
+        self.s_state += aux_var.delta
 
     def get_state(
         self,
     ) -> Dict[str, Any]:
-        return {"state": self.state, "s_loc": self.s_loc}
+        return {"s_state": self.s_state, "clients": list(self.clients)}
 
     def set_state(
         self,
         state: Dict[str, Any],
     ) -> None:
-        for key in ("state", "s_loc"):
+        for key in ("s_state", "clients"):
             if key not in state:
                 raise KeyError(f"Missing required state variable '{key}'.")
-        self.state = state["state"]
-        self.s_loc = state["s_loc"]
+        self.s_state = state["s_state"]
+        self.clients = set(state["clients"])
```

### Comparing `declearn-2.3.2/declearn/optimizer/regularizers/__init__.py` & `declearn-2.4.0/declearn/optimizer/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/optimizer/regularizers/_api.py` & `declearn-2.4.0/declearn/optimizer/regularizers/_api.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/optimizer/regularizers/_base.py` & `declearn-2.4.0/declearn/optimizer/regularizers/_base.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/quickrun/__init__.py` & `declearn-2.4.0/declearn/quickrun/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/quickrun/_config.py` & `declearn-2.4.0/declearn/quickrun/_config.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/quickrun/_parser.py` & `declearn-2.4.0/declearn/quickrun/_parser.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/quickrun/_run.py` & `declearn-2.4.0/declearn/quickrun/_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 If not provided with this, the script defaults to the MNIST example provided
 by declearn in `declearn.example.quickrun`.
 
 The script then locally runs the FL experiment as layed out in the TOML file,
 using privided model and data, and stores its result in the same folder.
 """
 
+import asyncio
 import importlib
 import logging
 import os
 from datetime import datetime
 from typing import Dict, Tuple
 
 import fire  # type: ignore
@@ -49,79 +50,82 @@
     ModelConfig,
 )
 from declearn.quickrun._parser import parse_data_folder
 from declearn.test_utils import make_importable
 from declearn.utils import (
     LOGGING_LEVEL_MAJOR,
     get_logger,
-    run_as_processes,
     set_device_policy,
 )
 
 __all__ = ["quickrun"]
 
 
 def get_model(folder: str, model_config: ModelConfig) -> Model:
-    "Return a model instance from a model config instance"
+    """Return a model instance from a model config instance."""
     path = model_config.model_file or os.path.join(folder, "model.py")
     path = os.path.abspath(path)
     if not os.path.isfile(path):
         raise FileNotFoundError("Model file not found: '{path}'.")
+    if not path.endswith(".py"):
+        raise TypeError(f"Model file at '{path}' is not a '.py' file.")
     with make_importable(os.path.dirname(path)):
         mod = importlib.import_module(os.path.basename(path)[:-3])
         model = getattr(mod, model_config.model_name)
+    if not isinstance(model, Model):
+        raise TypeError(
+            "Imported object from the model file is required to be a "
+            "'declearn.model.api.Model', but is a '{type(model)}'."
+        )
     return model
 
 
 def get_checkpoint(folder: str, expe_config: ExperimentConfig) -> str:
-    """Return the checkpoint folder, either default or as given in config"""
+    """Return the checkpoint folder, either default or as given in config."""
     if expe_config.checkpoint:
         checkpoint = expe_config.checkpoint
     else:
         timestamp = datetime.now().strftime("%y-%m-%d_%H-%M")
         checkpoint = os.path.join(folder, f"result_{timestamp}")
     return checkpoint
 
 
-def run_server(
+async def run_server(
     folder: str,
     network: NetworkServerConfig,
     model_config: ModelConfig,
     optim: FLOptimConfig,
     config: FLRunConfig,
     expe_config: ExperimentConfig,
 ) -> None:
-    """Routine to run a FL server, called by `run_declearn_experiment`."""
+    """Routine to run a FL server, called by `quickrun`."""
     # arguments serve modularity; pylint: disable=too-many-arguments
     set_device_policy(gpu=False)
     model = get_model(folder, model_config)
     checkpoint = get_checkpoint(folder, expe_config)
     checkpoint = os.path.join(checkpoint, "server")
     logger = get_logger("Server", fpath=os.path.join(checkpoint, "logger.txt"))
     server = FederatedServer(
         model, network, optim, expe_config.metrics, checkpoint, logger
     )
-    server.run(config)
+    await server.async_run(config)
 
 
-def run_client(
+async def run_client(
     folder: str,
     network: NetworkClientConfig,
-    model_config: ModelConfig,
     expe_config: ExperimentConfig,
     name: str,
     paths: Dict[str, str],
 ) -> None:
-    """Routine to run a FL client, called by `run_declearn_experiment`."""
-    # arguments serve modularity; pylint: disable=too-many-arguments
+    """Routine to run a FL client, called by `quickrun`."""
     # Overwrite client name based on folder name.
     network.name = name
     # Make the model importable and disable GPU use.
     set_device_policy(gpu=False)
-    _ = get_model(folder, model_config)
     # Add checkpointer.
     checkpoint = get_checkpoint(folder, expe_config)
     checkpoint = os.path.join(checkpoint, name)
     # Set up a logger: write everything to file, but filter console outputs.
     logger = get_logger(name, fpath=os.path.join(checkpoint, "logs.txt"))
     for handler in logger.handlers:
         if isinstance(handler, logging.StreamHandler):
@@ -132,16 +136,18 @@
         target=paths.get("train_target"),
         expose_classes=True,
     )
     valid = InMemoryDataset(
         paths.get("valid_data"),
         target=paths.get("valid_target"),
     )
-    client = FederatedClient(network, train, valid, checkpoint, logger=logger)
-    client.run()
+    client = FederatedClient(
+        network, train, valid, checkpoint, logger=logger, verbose=False
+    )
+    await client.async_run()
 
 
 def get_toml_folder(config: str) -> Tuple[str, str]:
     """Return the path to an experiment's folder and TOML config file.
 
     Parameters
     ----------
@@ -181,24 +187,24 @@
     client_dict = parse_data_folder(data_config, folder)
     return client_dict
 
 
 def server_to_client_network(
     network_cfg: NetworkServerConfig,
 ) -> NetworkClientConfig:
-    "Convert server network config to client network config."
+    """Convert server network config to client network config."""
     return NetworkClientConfig.from_params(
         protocol=network_cfg.protocol,
         server_uri=network_cfg.build_server().uri,
         name="replaceme",
     )
 
 
-def quickrun(config: str) -> None:
-    """Run a server and its clients using multiprocessing.
+async def quickrun(config: str) -> None:
+    """Run a server and its clients parallelly using asyncio.
 
     The script requires to be provided with the path to a TOML file
     with all the elements required to configurate an FL experiment,
     or the path to a folder containing :
 
     * A TOML file with all the elements required to configure an FL experiment.
     * A python file in which a declearn model is instantiated (in main scope).
@@ -227,45 +233,44 @@
       all clients operate under parallel python processes, and communicate over
       the localhost using un-encrypted websockets communications.
     - When run without any argument, this script/function operates on a basic
       MNIST example, for demonstration purposes.
     - You may refer to a more detailed MNIST example on our GitLab repository.
       See the `examples/mnist_quickrun` folder.
     """
-    # main script; pylint: disable=too-many-locals
     toml, folder = get_toml_folder(config)
-    # locate split data or split it if needed
+    # Locate split data or split it if needed.
     client_dict = locate_split_data(toml, folder)
-    # Parse toml files
+    # Parse toml files.
     ntk_server_cfg = NetworkServerConfig.from_toml(toml, False, "network")
     ntk_client_cfg = server_to_client_network(ntk_server_cfg)
     optim_cgf = FLOptimConfig.from_toml(toml, False, "optim")
     run_cfg = FLRunConfig.from_toml(toml, False, "run")
     model_cfg = ModelConfig.from_toml(toml, False, "model", True)
     expe_cfg = ExperimentConfig.from_toml(toml, False, "experiment", True)
-    # Set up a (func, args) tuple specifying the server process.
-    p_server = (
-        run_server,
-        (folder, ntk_server_cfg, model_cfg, optim_cgf, run_cfg, expe_cfg),
-    )
-    # Set up the (func, args) tuples specifying client-wise processes.
-    p_client = []
-    for name, data_dict in client_dict.items():
-        client = (
-            run_client,
-            (folder, ntk_client_cfg, model_cfg, expe_cfg, name, data_dict),
-        )
-        p_client.append(client)
-    # Run each and every process in parallel.
-    success, outputs = run_as_processes(p_server, *p_client)
-    assert success, "The FL process failed:\n" + "\n".join(
-        str(exc) for exc in outputs if isinstance(exc, RuntimeError)
+    # Set up the server and client-wise coroutines.
+    coro_server = run_server(
+        folder, ntk_server_cfg, model_cfg, optim_cgf, run_cfg, expe_cfg
     )
+    coro_clients = [
+        run_client(folder, ntk_client_cfg, expe_cfg, name, data_dict)
+        for name, data_dict in client_dict.items()
+    ]
+    # Run each and every coroutine in parallel.
+    await asyncio.gather(coro_server, *coro_clients)
+
+
+def fire_quickrun(config) -> None:
+    """Fire-wrappable caller to 'quickrun'."""
+    asyncio.run(quickrun(config))
+
+
+fire_quickrun.__doc__ = quickrun.__doc__
 
 
 def main() -> None:
     """Fire-wrapped `quickrun`."""
-    fire.Fire(quickrun)
+    fire.Fire(fire_quickrun)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `declearn-2.3.2/declearn/test_utils/__init__.py` & `declearn-2.4.0/declearn/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/test_utils/_argparse.py` & `declearn-2.4.0/declearn/test_utils/_argparse.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/test_utils/_assertions.py` & `declearn-2.4.0/declearn/test_utils/_assertions.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/test_utils/_convert.py` & `declearn-2.4.0/declearn/test_utils/_convert.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/test_utils/_gen_ssl.py` & `declearn-2.4.0/declearn/test_utils/_gen_ssl.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/test_utils/_imports.py` & `declearn-2.4.0/declearn/test_utils/_imports.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/test_utils/_vectors.py` & `declearn-2.4.0/declearn/test_utils/_vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,16 @@
             tensorflow = importlib.import_module("tensorflow")
             with tensorflow.device("CPU"):
                 return tensorflow.convert_to_tensor(array)
         if self.framework == "torch":
             torch = importlib.import_module("torch")
             return torch.from_numpy(array)
         if self.framework == "jax":
-            jnp = importlib.import_module("jax.numpy")
-            return jnp.asarray(array)
+            jax = importlib.import_module("jax")
+            return jax.device_put(array, jax.devices("cpu")[0])
         raise ValueError(f"Invalid framework '{self.framework}'")
 
     @property
     def mock_gradient(self) -> Vector:
         """Instantiate a Vector with random-valued mock gradients.
 
         Note: the RNG used to generate gradients has a fixed seed,
```

### Comparing `declearn-2.3.2/declearn/typing.py` & `declearn-2.4.0/declearn/typing.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/utils/__init__.py` & `declearn-2.4.0/declearn/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,24 +88,27 @@
     Access or create a logger, automating basic handlers' configuration.
 * [LOGGING_LEVEL_MAJOR][declearn.utils.LOGGING_LEVEL_MAJOR]:
     Custom "MAJOR" severity level, between stdlib "INFO" and "WARNING".
 
 Miscellaneous
 -------------
 
+* [Aggregate][declearn.utils.Aggregate]:
+    Abstract base dataclass for cross-peers data aggregation containers.
 * [TomlConfig][declearn.utils.TomlConfig]:
     Abstract base class to define TOML-parsable configuration containers.
 * [dataclass_from_func][declearn.utils.dataclass_from_func]:
     Automatically build a dataclass matching a function's signature.
 * [dataclass_from_init][declearn.utils.dataclass_from_init]:
     Automatically build a dataclass matching a class's init signature.
 * [run_as_processes][declearn.utils.run_as_processes]:
     Run coroutines concurrently within individual processes.
 """
 
+from ._aggregate import Aggregate
 from ._dataclass import (
     dataclass_from_func,
     dataclass_from_init,
 )
 from ._device_policy import (
     DevicePolicy,
     get_device_policy,
```

### Comparing `declearn-2.3.2/declearn/utils/_dataclass.py` & `declearn-2.4.0/declearn/utils/_dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 ) -> List[Tuple[str, Type, dataclasses.Field]]:
     """Parse function or method parameters into dataclass fields."""
     fields = []  # type: List[Tuple[str, Type, dataclasses.Field]]
     for param in params:
         # Parse out the parameter's name, annotated type and default value.
         fname = param.name
         ftype = Any if param.annotation is param.empty else param.annotation
-        field = dataclasses.field()
+        field = dataclasses.field()  # pylint: disable=invalid-field-call
         if param.default is not param.empty:
             field.default = param.default
         # Turn *args into a list and **kwargs into a dict.
         if param.kind is param.VAR_POSITIONAL:
             ftype = List[ftype]  # type: ignore
             field.default_factory = list
         elif param.kind is param.VAR_KEYWORD:
```

### Comparing `declearn-2.3.2/declearn/utils/_device_policy.py` & `declearn-2.4.0/declearn/utils/_device_policy.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/utils/_json.py` & `declearn-2.4.0/declearn/utils/_json.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/utils/_logging.py` & `declearn-2.4.0/declearn/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/utils/_numpy.py` & `declearn-2.4.0/declearn/utils/_numpy.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/utils/_register.py` & `declearn-2.4.0/declearn/utils/_register.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn/utils/_serialize.py` & `declearn-2.4.0/declearn/utils/_serialize.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 """Generic tools to (de-)serialize custom declearn objects to and from JSON."""
 
 import dataclasses
 from typing import Any, Dict, Optional, Type, TypedDict, Union
 
 from typing_extensions import Self  # future: import from typing (Py>=3.11)
 
+from declearn.typing import SupportsConfig
+from declearn.utils._json import json_dump, json_load
 from declearn.utils._register import (
     access_registered,
     access_registration_info,
 )
-from declearn.utils._json import json_dump, json_load
-from declearn.typing import SupportsConfig
 
 
 __all__ = [
     "ObjectConfig",
     "deserialize_object",
     "serialize_object",
 ]
```

### Comparing `declearn-2.3.2/declearn/utils/_toml_config.py` & `declearn-2.4.0/declearn/utils/_toml_config.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/declearn.egg-info/PKG-INFO` & `declearn-2.4.0/declearn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: declearn
-Version: 2.3.2
+Version: 2.4.0
 Summary: Declearn - a python package for private decentralized learning.
 Author-email: Paul Andrey <paul.andrey@inria.fr>, Nathan Bigaud <nathan.bigaud@inria.fr>
 Maintainer-email: Paul Andrey <paul.andrey@inria.fr>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -221,60 +221,62 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: cryptography>=35.0
-Requires-Dist: fire>=0.4
-Requires-Dist: pandas>=1.2
+Requires-Dist: fire~=0.4
+Requires-Dist: pandas<3.0,>=1.2
 Requires-Dist: requests~=2.18
-Requires-Dist: scikit-learn>=1.0
-Requires-Dist: tomli>=2.0; python_version < "3.11"
-Requires-Dist: typing_extensions>=4.0
+Requires-Dist: scikit-learn~=1.0
+Requires-Dist: tomli~=2.0; python_version < "3.11"
+Requires-Dist: tqdm~=4.62
+Requires-Dist: typing_extensions~=4.0
 Provides-Extra: all
-Requires-Dist: dm-haiku~=0.0.9; extra == "all"
-Requires-Dist: functorch<3.0,>=1.10; extra == "all"
+Requires-Dist: dm-haiku<=0.0.11,>=0.0.9; python_version > "3.8" and extra == "all"
+Requires-Dist: dm-haiku<=0.0.10,>=0.0.9; python_version == "3.8" and extra == "all"
 Requires-Dist: grpcio>=1.45; extra == "all"
 Requires-Dist: jax[cpu]~=0.4.1; extra == "all"
-Requires-Dist: opacus~=1.1; extra == "all"
+Requires-Dist: opacus~=1.4; extra == "all"
 Requires-Dist: protobuf>=3.19; extra == "all"
-Requires-Dist: tensorflow~=2.5; extra == "all"
-Requires-Dist: torch<3.0,>=1.10; extra == "all"
-Requires-Dist: websockets~=10.1; extra == "all"
+Requires-Dist: tensorflow~=2.11; extra == "all"
+Requires-Dist: torch<3.0,>=1.13; extra == "all"
+Requires-Dist: websockets<13.0,>=10.1; extra == "all"
 Provides-Extra: dp
-Requires-Dist: opacus~=1.1; extra == "dp"
+Requires-Dist: opacus~=1.4; extra == "dp"
 Provides-Extra: grpc
 Requires-Dist: grpcio>=1.45; extra == "grpc"
 Requires-Dist: protobuf>=3.19; extra == "grpc"
 Provides-Extra: haiku
-Requires-Dist: dm-haiku~=0.0.9; extra == "haiku"
+Requires-Dist: dm-haiku<=0.0.11,>=0.0.9; python_version > "3.8" and extra == "haiku"
+Requires-Dist: dm-haiku<=0.0.10,>=0.0.9; python_version == "3.8" and extra == "haiku"
 Requires-Dist: jax[cpu]~=0.4.1; extra == "haiku"
 Provides-Extra: tensorflow
-Requires-Dist: tensorflow~=2.5; extra == "tensorflow"
+Requires-Dist: tensorflow~=2.11; extra == "tensorflow"
 Provides-Extra: torch
 Requires-Dist: torch<3.0,>=1.13; extra == "torch"
 Provides-Extra: torch1
 Requires-Dist: torch~=1.13.0; extra == "torch1"
 Provides-Extra: torch2
 Requires-Dist: torch~=2.0; extra == "torch2"
 Provides-Extra: websockets
-Requires-Dist: websockets~=10.1; extra == "websockets"
+Requires-Dist: websockets<13.0,>=10.1; extra == "websockets"
 Provides-Extra: docs
-Requires-Dist: mkdocstrings[python]>=0.8; extra == "docs"
-Requires-Dist: mkdocs-autorefs; extra == "docs"
-Requires-Dist: mkdocs-literate-nav; extra == "docs"
-Requires-Dist: mkdocs-material>=9.1; extra == "docs"
+Requires-Dist: mkdocstrings[python]~=0.8; extra == "docs"
+Requires-Dist: mkdocs-autorefs~=0.4; extra == "docs"
+Requires-Dist: mkdocs-literate-nav~=0.4; extra == "docs"
+Requires-Dist: mkdocs-material~=9.1; extra == "docs"
 Provides-Extra: tests
-Requires-Dist: black~=23.0; extra == "tests"
+Requires-Dist: black~=24.0; extra == "tests"
 Requires-Dist: mypy~=1.0; extra == "tests"
-Requires-Dist: pylint>=2.14; extra == "tests"
-Requires-Dist: pytest>=6.1; extra == "tests"
-Requires-Dist: pytest-asyncio; extra == "tests"
-Requires-Dist: pytest-cov>=4.0; extra == "tests"
+Requires-Dist: pylint~=3.0; extra == "tests"
+Requires-Dist: pytest~=7.4; extra == "tests"
+Requires-Dist: pytest-asyncio~=0.20; extra == "tests"
+Requires-Dist: pytest-cov~=4.0; extra == "tests"
 
 # Declearn: a modular and extensible framework for Federated Learning
 
 - [Introduction](#introduction)
 - [Setup](#setup)
 - [Quickstart](#quickstart)
 - [Usage of the Python API](#usage-of-the-python-api)
```

### Comparing `declearn-2.3.2/declearn.egg-info/SOURCES.txt` & `declearn-2.4.0/declearn.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,49 @@
+.gitignore
 .gitlab-ci.yml
 AUTHORS
 LICENSE
 README.md
 mkdocs.yml
 pyproject.toml
 tox.ini
 declearn/__init__.py
 declearn/py.typed
 declearn/typing.py
+declearn/version.py
 declearn.egg-info/PKG-INFO
 declearn.egg-info/SOURCES.txt
 declearn.egg-info/dependency_links.txt
 declearn.egg-info/entry_points.txt
 declearn.egg-info/requires.txt
 declearn.egg-info/top_level.txt
 declearn/aggregator/__init__.py
 declearn/aggregator/_api.py
-declearn/aggregator/_base.py
+declearn/aggregator/_avg.py
 declearn/aggregator/_gma.py
 declearn/communication/__init__.py
-declearn/communication/_build.py
 declearn/communication/api/__init__.py
 declearn/communication/api/_client.py
 declearn/communication/api/_server.py
-declearn/communication/api/_service.py
+declearn/communication/api/backend/__init__.py
+declearn/communication/api/backend/_handler.py
+declearn/communication/api/backend/actions.py
+declearn/communication/api/backend/flags.py
 declearn/communication/grpc/__init__.py
 declearn/communication/grpc/_client.py
 declearn/communication/grpc/_server.py
 declearn/communication/grpc/protobufs/__init__.py
 declearn/communication/grpc/protobufs/message.proto
 declearn/communication/grpc/protobufs/message_pb2.py
 declearn/communication/grpc/protobufs/message_pb2_grpc.py
 declearn/communication/messaging/__init__.py
 declearn/communication/messaging/_messages.py
-declearn/communication/messaging/flags.py
+declearn/communication/utils/__init__.py
+declearn/communication/utils/_build.py
+declearn/communication/utils/_parse.py
 declearn/communication/websockets/__init__.py
 declearn/communication/websockets/_client.py
 declearn/communication/websockets/_server.py
 declearn/communication/websockets/_tools.py
 declearn/data_info/__init__.py
 declearn/data_info/_base.py
 declearn/data_info/_fields.py
@@ -68,14 +74,17 @@
 declearn/main/privacy/_dp_trainer.py
 declearn/main/utils/__init__.py
 declearn/main/utils/_checkpoint.py
 declearn/main/utils/_constraints.py
 declearn/main/utils/_data_info.py
 declearn/main/utils/_early_stop.py
 declearn/main/utils/_training.py
+declearn/messaging/__init__.py
+declearn/messaging/_api.py
+declearn/messaging/_base.py
 declearn/metrics/__init__.py
 declearn/metrics/_api.py
 declearn/metrics/_classif.py
 declearn/metrics/_mean.py
 declearn/metrics/_roc_auc.py
 declearn/metrics/_rsquared.py
 declearn/metrics/_utils.py
@@ -132,14 +141,15 @@
 declearn/test_utils/_argparse.py
 declearn/test_utils/_assertions.py
 declearn/test_utils/_convert.py
 declearn/test_utils/_gen_ssl.py
 declearn/test_utils/_imports.py
 declearn/test_utils/_vectors.py
 declearn/utils/__init__.py
+declearn/utils/_aggregate.py
 declearn/utils/_dataclass.py
 declearn/utils/_device_policy.py
 declearn/utils/_json.py
 declearn/utils/_logging.py
 declearn/utils/_multiprocess.py
 declearn/utils/_numpy.py
 declearn/utils/_register.py
@@ -165,18 +175,20 @@
 docs/release-notes/v2.1.1.md
 docs/release-notes/v2.2.0.md
 docs/release-notes/v2.2.1.md
 docs/release-notes/v2.2.2.md
 docs/release-notes/v2.3.0.md
 docs/release-notes/v2.3.1.md
 docs/release-notes/v2.3.2.md
+docs/release-notes/v2.4.0.md
 docs/user-guide/SUMMARY.md
 docs/user-guide/fl_process.md
 docs/user-guide/index.md
 docs/user-guide/local_dp.md
+docs/user-guide/optimizer.md
 docs/user-guide/package.md
 docs/user-guide/usage.md
 examples/adding_rmsprop/readme.md
 examples/heart-uci/client.py
 examples/heart-uci/data.py
 examples/heart-uci/gen_ssl.py
 examples/heart-uci/readme.md
@@ -187,23 +199,27 @@
 examples/mnist/readme.md
 examples/mnist/run_client.py
 examples/mnist/run_demo.py
 examples/mnist/run_server.py
 examples/mnist_quickrun/config.toml
 examples/mnist_quickrun/mnist.ipynb
 examples/mnist_quickrun/model.py
+examples/mnist_quickrun/model_torch.py
 examples/mnist_quickrun/readme.md
 scripts/gen_docs.py
 scripts/run_tests.sh
 test/conftest.py
 test/aggregator/test_aggregator.py
 test/communication/conftest.py
 test/communication/test_exchanges.py
 test/communication/test_grpc.py
 test/communication/test_server.py
+test/communication/test_utils.py
+test/communication/backend/test_actions.py
+test/communication/backend/test_messages_handler.py
 test/data_info/test_classes_field.py
 test/data_info/test_data_info_utils.py
 test/data_info/test_datatype_field.py
 test/data_info/test_nbsamples_field.py
 test/data_info/test_shape_field.py
 test/dataset/dataset_testbase.py
 test/dataset/test_dataset_utils.py
@@ -239,16 +255,18 @@
 test/optimizer/test_optimizer.py
 test/optimizer/test_regularizers.py
 test/optimizer/test_scaffold.py
 test/optimizer/test_tflow_optim.py
 test/optimizer/test_torch_optim.py
 test/quickrun/test_quickrun_utils.py
 test/utils/test_json.py
+test/utils/test_multiprocess.py
 test/utils/test_register.py
 test/utils/test_serialize.py
 test/utils/test_toml.py
+test/vector/conftest.py
 test/vector/test_generic_vector.py
 test/vector/test_jaxnp_vector.py
 test/vector/test_numpy_vector.py
 test/vector/test_tflow_vector.py
 test/vector/test_torch_vector.py
 test/vector/vector_testing.py
```

### Comparing `declearn-2.3.2/docs/devs-guide/contribute.md` & `declearn-2.4.0/docs/devs-guide/contribute.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
   coherent with the practices already at work in declearn.
 - Abide by [PEP 257](https://peps.python.org/pep-0257/), _i.e._ write
   docstrings **everywhere** (unless inheriting from a method, the behaviour
   and signature of which are unmodified). The formatting rules for docstrings
   are detailed in the [docstrings style guide](./docs-style.md).
 - Type-hint the code, abiding by [PEP 484](https://peps.python.org/pep-0484/);
   note that the use of Any and of "type: ignore" comments is authorized, but
-  should be remain sparse.
+  should remain parsimonious.
 - Lint your code with [mypy](http://mypy-lang.org/) (for static type checking)
   and [pylint](https://pylint.pycqa.org/en/latest/) (for more general linting);
   do use "type: ..." and "pylint: disable=..." comments where you think it
   relevant, preferably with some side explanations. (see dedicated sections:
   [pylint](./tests.md#running-pylint-to-check-the-code)
   and [mypy](./tests.md/#running-mypy-to-type-check-the-code))
 - Reformat your code using [black](https://github.com/psf/black); do use
```

### Comparing `declearn-2.3.2/docs/devs-guide/docs-build.md` & `declearn-2.4.0/docs/devs-guide/docs-build.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/devs-guide/docs-style.md` & `declearn-2.4.0/docs/devs-guide/docs-style.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/devs-guide/index.md` & `declearn-2.4.0/docs/devs-guide/index.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/devs-guide/tests.md` & `declearn-2.4.0/docs/devs-guide/tests.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/index.md` & `declearn-2.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/quickstart.md` & `declearn-2.4.0/docs/quickstart.md`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,18 @@
 [documentation][declearn.quickrun.ModelConfig] to see all available fields.
 
 **`[experiment]`: Optional section**, what to report during the experiment and
 where to report it. An example:
 
 ```python
 [experiment]
-metrics=[["multi-classif",{labels = [0,1,2,3,4,5,6,7,8,9]}]] # Accuracy metric
+metrics = [
+    # Multi-label Accuracy, Precision, Recall and F1-Score.
+    ["multi-classif", {labels = [0,1,2,3,4,5,6,7,8,9]}]
+]
 checkpoint = "./result_custom" # Custom location for results
 ```
 
 This section is parsed as the fields of a `ExperimentConfig` dataclass.
 Check its [documentation][declearn.quickrun.ExperimentConfig] to see all
 available fields.
```

### Comparing `declearn-2.3.2/docs/release-notes/v2.0.2.md` & `declearn-2.4.0/docs/release-notes/v2.0.2.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/release-notes/v2.0.3.md` & `declearn-2.4.0/docs/release-notes/v2.0.3.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/release-notes/v2.1.0.md` & `declearn-2.4.0/docs/release-notes/v2.1.0.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/release-notes/v2.1.1.md` & `declearn-2.4.0/docs/release-notes/v2.1.1.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/release-notes/v2.2.0.md` & `declearn-2.4.0/docs/release-notes/v2.2.0.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/release-notes/v2.2.1.md` & `declearn-2.4.0/docs/release-notes/v2.2.1.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/release-notes/v2.2.2.md` & `declearn-2.4.0/docs/release-notes/v2.2.2.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/release-notes/v2.3.0.md` & `declearn-2.4.0/docs/release-notes/v2.3.0.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/release-notes/v2.3.1.md` & `declearn-2.4.0/docs/release-notes/v2.3.1.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/release-notes/v2.3.2.md` & `declearn-2.4.0/docs/release-notes/v2.3.2.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/setup.md` & `declearn-2.4.0/docs/setup.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Installation guide
 
+This guide provides with all the required information to install `declearn`.
+
+**TL;DR**:<br/>
+If you want to install the latest stable version with all of its optional
+dependencies, simply run `pip install declearn[all]` from your desired
+python (preferably virtual) environment.
+
+**Important note**:<br/>
+When running a federated process with DecLearn, the server and all clients
+should use the same `major.minor` version; otherwise, clients' registration
+will fail verbosely, prompting to install the same version as the server's.
+
 ## Requirements
 
 - python >= 3.8
 - pip
 
 Third-party requirements are specified (and automatically installed) as part
 of the installation process, and may be consulted from the `pyproject.toml`
```

### Comparing `declearn-2.3.2/docs/user-guide/fl_process.md` & `declearn-2.4.0/docs/user-guide/fl_process.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 alternative overall algorithmic processes - notably by overriding
 or extending methods that define the sub-components of the process
 exposed here.
 
 ## Overall process orchestrated by the server
 
 - Initially:
-    - have the clients connect and register for training
-    - prepare model and optimizer objects on both sides
+    - the clients connect to the server and register for training
+    - the server may collect targetted metadata from clients when required
+    - the server sets up the model, optimizers, aggregator and metrics
+    - all clients receive instructions to set up these objects as well
 - Iteratively:
     - perform a training round
     - perform an evaluation round
     - decide whether to continue, based on the number of
       rounds taken or on the evolution of the global loss
 - Finally:
     - restore the model weights that yielded the lowest global loss
@@ -32,36 +34,48 @@
 - Server:
     - open up registration (stop rejecting all received messages)
     - handle and respond to client-emitted registration requests
     - await criteria to have been met (exact or min/max number of clients
       registered, optionally under a given timeout delay)
     - close registration (reject future requests)
 - Client:
-    - gather metadata about the local training dataset
-      (_e.g._ dimensions and unique labels)
-    - connect to the server and send a request to join training,
-      including the former information
+    - connect to the server and send a request to join training
     - await the server's response (retry after a timeout if the request
       came in too soon, i.e. registration is not opened yet)
-- messaging : (JoinRequest <-> JoinReply)
 
 ### Post-registration initialization
 
+#### (Optional) Metadata exchange
+
+This step is optional, and depends on the trained model's requirement
+for dataset information (typically, features shape and/or dtype).
+
+- Server:
+    - query clients for targetted metadata about the local training datasets
+- Client:
+    - collect and send back queried metadata
+- messaging: (MetadataQuery <-> MetadataReply)
 - Server:
-    - validate and aggregate clients-transmitted metadata
-    - finalize the model's initialization using those metadata
-    - send the model, local optimizer and evaluation metrics specs to clients
+    - validate and aggregate received information
+    - pass it to the model so as to finalize its initialization
+
+#### Initialization of the federated optimization problem
+
+- Server:
+    - set up the model, local and global optimizer, aggregator and metrics
+    - send specs to the clients so that they set up local counterpart objects
 - Client:
-    - instantiate the model, optimizer and metrics based on server instructions
-- messaging: (InitRequest <-> GenericMessage)
+    - instantiate the model, optimizer, aggregator and metrics based on specs
+- messaging: (InitRequest <-> InitReply)
+
+#### (Optional) Local differential privacy setup
 
-### (Optional) Local differential privacy setup
+This step is optional; a flag in the InitRequest at the previous step
+indicates to clients that it is to happen, as a secondary substep.
 
-- This step is optional; a flag in the InitRequest at the previous step
-  indicates to clients that it is to happen, as a secondary substep.
 - Server:
     - send hyper-parameters to set up local differential privacy, including
       dp-specific hyper-parameters and information on the planned training
 - Client:
     - adjust the training process to use sample-wise gradient clipping and
       add gaussian noise to gradients, implementing the DP-SGD algorithm
     - set up a privacy accountant to monitor the use of the privacy budget
@@ -87,16 +101,16 @@
     - run global updates through the server's optimizer to modify and finally
       apply them
 
 ### Evaluation round
 
 - Server:
     - select clients that are to participate
-    - send data-batching parameters and shared model trainable weights
-    - (_send effort constraints, unused for now_)
+    - send data-batching parameters and effort constraints
+    - send shared model trainable weights
 - Client:
     - update model weights
     - perform evaluation steps based on effort constraints
     - step: update evaluation metrics, including the model's loss, over a batch
     - optionally checkpoint the model, local optimizer and evaluation metrics
     - send results to the server: optionally prevent sharing detailed metrics;
       always include the scalar validation loss value
```

### Comparing `declearn-2.3.2/docs/user-guide/index.md` & `declearn-2.4.0/docs/user-guide/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,9 +8,11 @@
 
 - [Overview of the Federated Learning process](./fl_process.md):<br/>
     Description of the Federated Learning process implemented by declearn.
 - [Overview of the declearn API](./package.md):<br/>
     Description of the declearn code's structure and of the main APIs.
 - [Hands-on usage](./usage.md):<br/>
     Guide on how to set up your own federated learning task using declearn.
+- [Guide to the Optimizer API](./optimizer.md):<br/>
+    API, design principles and practical how-tos of the declearn Optimizer.
 - [Local Differential Privacy capabilities](./local_dp.md):<br/>
     Description of the local-DP features of declearn.
```

### Comparing `declearn-2.3.2/docs/user-guide/local_dp.md` & `declearn-2.4.0/docs/user-guide/local_dp.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/docs/user-guide/package.md` & `declearn-2.4.0/docs/user-guide/package.md`

 * *Files 26% similar despite different names*

```diff
@@ -10,118 +10,195 @@
   &emsp; Client-Server network communications API and implementations.
 - `data_info`:<br/>
   &emsp; Tools to write and extend shareable metadata fields specifications.
 - `dataset`:<br/>
   &emsp; Data interfacing API and implementations.
 - `main`:<br/>
   &emsp; Main classes implementing a Federated Learning process.
+- `messaging`:<br/>
+  &emsp; API and default classes to define parsable messages for applications.
 - `metrics`:<br/>
   &emsp; Iterative and federative evaluation metrics computation tools.
 - `model`:<br/>
   &emsp; Model interfacing API and implementations.
 - `optimizer`:<br/>
   &emsp; Framework-agnostic optimizer and algorithmic plug-ins API and tools.
 - `typing`:<br/>
   &emsp; Type hinting utils, defined and exposed for code readability purposes.
 - `utils`:<br/>
   &emsp; Shared utils used (extensively) across all of declearn.
+- `version`:<br/>
+  &emsp; DecLearn version information, as hard-coded constants.
 
 ## Main abstractions
 
 This section lists the main abstractions implemented as part of
 `declearn`, exposing their main object and usage, some examples
 of ready-to-use implementations that are part of `declearn`, as
 well as references on how to extend the support of `declearn`
 backend (notably, (de)serialization and configuration utils) to
 new custom concrete implementations inheriting the abstraction.
 
-### `Model`
+### Model and Tensors
+
+#### `Model`
 - Import: `declearn.model.api.Model`
 - Object: Interface framework-specific machine learning models.
 - Usage: Compute gradients, apply updates, compute loss...
 - Examples:
     - `declearn.model.sklearn.SklearnSGDModel`
     - `declearn.model.tensorflow.TensorflowModel`
     - `declearn.model.torch.TorchModel`
 - Extend: use `declearn.utils.register_type(group="Model")`
 
-### `Vector`
+#### `Vector`
 - Import: `declearn.model.api.Vector`
 - Object: Interface framework-specific data structures.
 - Usage: Wrap and operate on model weights, gradients, updates...
 - Examples:
     - `declearn.model.sklearn.NumpyVector`
     - `declearn.model.tensorflow.TensorflowVector`
     - `declearn.model.torch.TorchVector`
 - Extend: use `declearn.model.api.register_vector_type`
 
-### `OptiModule`
+### Federated Optimization
+
+You may learn more about our (non-abstract) `Optimizer` API by reading our
+[Optimizer guide](./optimizer.md).
+
+#### `Aggregator`
+- Import: `declearn.aggregator.Aggregator`
+- Object: Define model updates aggregation algorithms.
+- Usage: Post-process client updates; finalize aggregated global ones.
+- Examples:
+    - `declearn.aggregator.AveragingAggregator`
+    - `declearn.aggregator.GradientMaskedAveraging`
+- Extend:
+    - Simply inherit from `Aggregator` (registration is automated).
+    - To avoid it, use `class MyAggregator(Aggregator, register=False)`.
+
+#### `ModelUpdates`
+- Import: `declearn.aggregator.ModelUpdates`
+- Object: Define exchanged model updates data and their aggregation.
+- Usage: Share and aggregate client's updates for a given `Aggregator`.
+- Examples:
+    - Each `Aggregator` has its own dedicated/supported `ModelUpdates` type(s).
+- Extend:
+    - Simply inherit from `ModelUpdates` (registration is automated).
+    - Define a `name` class attribute and decorate as a `dataclass`.
+    - To avoid it, use `class MyModelUpdates(ModelUpdates, register=False)`.
+
+#### `OptiModule`
 - Import: `declearn.optimizer.modules.OptiModule`
 - Object: Define optimization algorithm bricks.
 - Usage: Plug into a `declearn.optimizer.Optimizer`.
 - Examples:
     - `declearn.optimizer.modules.AdagradModule`
     - `declearn.optimizer.modules.MomentumModule`
     - `declearn.optimizer.modules.ScaffoldClientModule`
     - `declearn.optimizer.modules.ScaffoldServerModule`
 - Extend:
     - Simply inherit from `OptiModule` (registration is automated).
     - To avoid it, use `class MyModule(OptiModule, register=False)`.
 
-### `Regularizer`
-- Import: `declearn.optimizer.modules.Regularizer`
+#### `Regularizer`
+- Import: `declearn.optimizer.regularizers.Regularizer`
 - Object: Define loss-regularization terms as gradients modifiers.
 - Usage: Plug into a `declearn.optimizer.Optimizer`.
 - Examples:
-    - `declearn.optimizer.regularizer.FedProxRegularizer`
-    - `declearn.optimizer.regularizer.LassoRegularizer`
-    - `declearn.optimizer.regularizer.RidgeRegularizer`
+    - `declearn.optimizer.regularizers.FedProxRegularizer`
+    - `declearn.optimizer.regularizers.LassoRegularizer`
+    - `declearn.optimizer.regularizers.RidgeRegularizer`
 - Extend:
     - Simply inherit from `Regularizer` (registration is automated).
     - To avoid it, use `class MyRegularizer(Regularizer, register=False)`.
 
-### `Metric`
+#### `AuxVar`
+- Import: `declearn.optimizer.modules.AuxVar`
+- Object: Define exchanged data between a pair of `OptiModules` across the
+  clients/server boundary, and their aggregation.
+- Usage: Share information from server to clients and reciprocally.
+- Examples:
+    - `declearn.optimizer.modules.ScaffoldAuxVar`
+- Extend:
+    - Simply inherit from `AuxVar` (registration is automated).
+    - Define a `name` class attribute and decorate as a `dataclass`.
+    - To avoid it, use `class MyAuxVar(AuxVar, register=False)`.
+
+### Evaluation Metrics
+
+#### `Metric`
 - Import: `declearn.metrics.Metric`
 - Object: Define evaluation metrics to compute iteratively and federatively.
 - Usage: Compute local and federated metrics based on local data streams.
 - Examples:
     - `declearn.metric.BinaryRocAuc`
     - `declearn.metric.MeanSquaredError`
     - `declearn.metric.MuticlassAccuracyPrecisionRecall`
 - Extend:
     - Simply inherit from `Metric` (registration is automated).
-    - To avoid it, use `class MyMetric(Metric, register=False)`
+    - To avoid it, use `class MyMetric(Metric, register=False)`.
+
+#### `MetricState`
+- Import: `declearn.metrics.MetricState`
+- Object: Define exchanged data to compute a `Metric` and their aggregation.
+- Usage: Share locally-computed metrics for their aggregation into global ones.
+- Examples:
+    - Each `Metric` has its own dedicated/supported `MetricState` type(s).
+- Extend:
+    - Simply inherit from `MetricState` (registration is automated).
+    - Define a `name` class attribute and decorate as a `dataclass`.
+    - To avoid it, use `class MyMetricState(MetricState, register=False)`.
+
+### Network communication
 
-### `NetworkClient`
+#### `NetworkClient`
 - Import: `declearn.communication.api.NetworkClient`
 - Object: Instantiate a network communication client endpoint.
 - Usage: Register for training, send and receive messages.
 - Examples:
     - `declearn.communication.grpc.GrpcClient`
     - `declearn.communication.websockets.WebsocketsClient`
 - Extend:
     - Simply inherit from `NetworkClient` (registration is automated).
     - To avoid it, use `class MyClient(NetworkClient, register=False)`.
 
-### `NetworkServer`
+#### `NetworkServer`
 - Import: `declearn.communication.api.NetworkServer`
 - Object: Instantiate a network communication server endpoint.
 - Usage: Receive clients' requests, send and receive messages.
 - Examples:
     - `declearn.communication.grpc.GrpcServer`
     - `declearn.communication.websockets.WebsocketsServer`
 - Extend:
     - Simply inherit from `NetworkServer` (registration is automated).
     - To avoid it, use `class MyServer(NetworkServer, register=False)`.
 
-### `Dataset`
+#### `Message`
+- Import: `declearn.messaging.Message`
+- Object: Define serializable/parsable message types and their data.
+- Usage: Exchanged via communication endpoints to transmit data and
+  trigger behaviors based on type analysis.
+- Examples:
+    - `declearn.messages.TrainRequest`
+    - `declearn.messages.TrainReply`
+    - `declearn.messages.Error`
+- Extend:
+    - Simply inherit from `Message` (registration is automated).
+    - To avoid it, use `class MyMessage(Message, register=False)`.
+
+### Dataset
+
+#### `Dataset`
 - Import: `declearn.dataset.Dataset`
 - Object: Interface data sources agnostic to their format.
 - Usage: Yield (inputs, labels, weights) data batches, expose metadata.
 - Examples:
     - `declearn.dataset.InMemoryDataset`
-- Extend: use `declearn.utils.register_type(group="Dataset")`
+    - `declearn.dataset.tensorflow.TensorflowDataset`
+    - `declearn.dataset.torch.TorchDataset`
+- Extend: use `declearn.utils.register_type(group="Dataset")`.
 
 ## Full API Reference
 
 The full API reference, which is generated automatically from the code's
 internal documentation, can be found [here](../api-reference/index.md).
```

### Comparing `declearn-2.3.2/docs/user-guide/usage.md` & `declearn-2.4.0/docs/user-guide/usage.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/examples/adding_rmsprop/readme.md` & `declearn-2.4.0/examples/adding_rmsprop/readme.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/examples/heart-uci/client.py` & `declearn-2.4.0/examples/heart-uci/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,39 +22,43 @@
 
 import numpy as np
 
 from declearn.communication import NetworkClientConfig
 from declearn.dataset import InMemoryDataset
 from declearn.dataset.examples import load_heart_uci
 from declearn.main import FederatedClient
-from declearn.test_utils import make_importable, setup_client_argparse
+from declearn.test_utils import setup_client_argparse
 
 
 FILEDIR = os.path.dirname(__file__)
 
 
 def run_client(
     name: Literal["cleveland", "hungarian", "switzerland", "va"],
     ca_cert: str,
     protocol: str = "websockets",
     serv_uri: str = "wss://localhost:8765",
+    verbose: bool = True,
 ) -> None:
     """Instantiate and run a given client.
 
     Arguments
     ---------
     name: str
         Name of the client (i.e. center data from which to use).
     ca_cert: str
         Path to the certificate authority file that was used to
         sign the server's SSL certificate.
     protocol: str, default="websockets"
         Name of the communication protocol to use.
     serv_uri: str, default="wss://localhost:8765"
         URI of the server to which to connect.
+    verbose: bool, default=True
+        Whether to be verbose in the displayed contents, including
+        all logger information and progress bars.
     """
 
     # (1-2) Interface training and optional validation data.
 
     # Load and randomly split the dataset. Note: target is a str (column name).
     data, target = load_heart_uci(name, folder=os.path.join(FILEDIR, "data"))
     data = data.loc[np.random.permutation(data.index)]
@@ -83,16 +87,19 @@
 
     # (4) Run any necessary import statement.
     #  => None are required in this example.
 
     # (5) Instantiate a FederatedClient and run it.
 
     client = FederatedClient(
-        # fmt: off
-        network, train, valid, checkpoint=f"{FILEDIR}/results/{name}"
+        netwk=network,
+        train_data=train,
+        valid_data=valid,
+        checkpoint=f"{FILEDIR}/results/{name}",
+        verbose=verbose,
         # Note: you may add `share_metrics=False` to prevent sending
         # evaluation metrics to the server, out of privacy concerns
     )
     client.run()
 
 
 # Called when the script is called directly (using `python client.py`).
```

### Comparing `declearn-2.3.2/examples/heart-uci/data.py` & `declearn-2.4.0/examples/heart-uci/data.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/examples/heart-uci/gen_ssl.py` & `declearn-2.4.0/examples/heart-uci/gen_ssl.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/examples/heart-uci/readme.md` & `declearn-2.4.0/examples/heart-uci/readme.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/examples/heart-uci/run.py` & `declearn-2.4.0/examples/heart-uci/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,20 +41,24 @@
     # Use a temporary directory for single-use self-signed SSL files.
     with tempfile.TemporaryDirectory() as folder:
         # Generate self-signed SSL certificates and gather their paths.
         ca_cert, sv_cert, sv_pkey = generate_ssl_certificates(folder)
         # Specify the server and client routines that need executing.
         server = (run_server, (nb_clients, sv_cert, sv_pkey))
         clients = [
-            (run_client, (name, ca_cert)) for name in NAMES[:nb_clients]
+            (run_client, {"name": name, "ca_cert": ca_cert, "verbose": False})
+            for name in NAMES[:nb_clients]
         ]
         # Run routines in isolated processes. Raise if any failed.
         success, outp = run_as_processes(server, *clients)
         if not success:
+            exceptions = "\n".join(
+                str(e) for e in outp if isinstance(e, RuntimeError)
+            )
             raise RuntimeError(
                 "Something went wrong during the demo. Exceptions caught:\n"
-                "\n".join(str(e) for e in outp if isinstance(e, RuntimeError))
+                + exceptions
             )
 
 
 if __name__ == "__main__":
     run_demo()
```

### Comparing `declearn-2.3.2/examples/heart-uci/server.py` & `declearn-2.4.0/examples/heart-uci/server.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/examples/mnist/generate_ssl.py` & `declearn-2.4.0/examples/mnist/generate_ssl.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/examples/mnist/prepare_data.py` & `declearn-2.4.0/examples/mnist/prepare_data.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/examples/mnist/readme.md` & `declearn-2.4.0/examples/mnist/readme.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/examples/mnist/run_client.py` & `declearn-2.4.0/examples/mnist/run_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 
     client = declearn.main.FederatedClient(
         netwk=network,
         train_data=train,
         valid_data=valid,
         checkpoint=checkpoint,
         logger=logger,
+        verbose=verbose,
     )
     client.run()
 
 
 # This part should not be altered: it provides with an argument parser
 # for `python client.py`.
```

### Comparing `declearn-2.3.2/examples/mnist/run_demo.py` & `declearn-2.4.0/examples/mnist/run_demo.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,34 +40,32 @@
     scheme: Literal["iid", "labels", "biased"] = "iid",
     seed: Optional[int] = None,
 ) -> None:
     """Run a server and its clients using multiprocessing.
 
     Parameters
     ------
-
     n_clients: int
         number of clients to run.
     data_folder: str
         Relative path to the folder holding client's data
-
     """
     # Generate the MNIST split data for this demo.
     data_folder = prepare_mnist(nb_clients, scheme, seed=seed)
     # Use a temporary directory for single-use self-signed SSL files.
     with tempfile.TemporaryDirectory() as folder:
         # Generate self-signed SSL certificates and gather their paths.
         ca_cert, sv_cert, sv_pkey = generate_ssl_certificates(folder)
         # Specify the server and client routines that need executing.
         server = (run_server, (nb_clients, sv_cert, sv_pkey))
-        client_args = tuple(
-            [data_folder, ca_cert, "websockets", "wss://localhost:8765", False]
-        )
+        client_kwargs = {
+            "data_folder": data_folder, "ca_cert": ca_cert, "verbose": False
+        }
         clients = [
-            (run_client, (f"client_{idx}", *client_args))
+            (run_client, (f"client_{idx}",), client_kwargs)
             for idx in range(nb_clients)
         ]
         # Run routines in isolated processes. Raise if any failed.
         success, outp = run_as_processes(server, *clients)
         if not success:
             raise RuntimeError(
                 "Something went wrong during the demo. Exceptions caught:\n"
```

### Comparing `declearn-2.3.2/examples/mnist/run_server.py` & `declearn-2.4.0/examples/mnist/run_server.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/examples/mnist_quickrun/config.toml` & `declearn-2.4.0/examples/mnist_quickrun/config.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # This is a minimal TOML file for the MNIST example
 # It contains the bare minimum to make the experiment run.
-# See quickstart for more details. 
+# See quickstart for more details.
 
 # The TOML is parsed by python as dictionnary with each `[header]`
 # as a key. Note the "=" sign and the absence of quotes around keys.
 # For more details, see the full doc : https://toml.io/en/
 
 [network] # Network configuration used by both client and server
     protocol = "websockets" # Protocol used, to keep things simple use websocket
     host = "127.0.0.1" # Address used, works as-is on most set ups
     port = 8765 # Port used, works as-is on most set ups
 
 [data] # Where to find your data
-    data_folder = "examples/mnist_quickrun/data_iid" 
+    data_folder = "examples/mnist_quickrun/data_iid"
 
 [optim] # Optimization options for both client and server
     aggregator = "averaging" # Server aggregation strategy
 
     [optim.client_opt] # Client optimization strategy
     lrate = 0.001 # Client learning rate
     modules = ["adam"] # List of optimizer modules used
@@ -33,9 +33,11 @@
     [run.training] # Client training options
     batch_size = 48 # Training batch size
 
     [run.evaluate] # Client evaluation options
     batch_size = 128 # Evaluation batch size
 
 [experiment] # What to report during the experiment and where to report it
-    metrics=[["multi-classif",{labels = [0,1,2,3,4,5,6,7,8,9]}]] # Accuracy metric
-
+    metrics = [
+        # Multi-label Accuracy, Precision, Recall and F-Score.
+        ["multi-classif", {labels = [0,1,2,3,4,5,6,7,8,9]}]
+    ]
```

### Comparing `declearn-2.3.2/examples/mnist_quickrun/mnist.ipynb` & `declearn-2.4.0/examples/mnist_quickrun/mnist.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998253706419029%*

 * *Differences: {"'cells'": "{2: {'source': ['We first clone the repo, to have both the package itself and the "*

 * *            '`examples` folder we will use in this tutorial, then naviguate to the package '*

 * *            "directory, and finally install the required dependencies.\\n', '\\n', '**If you have "*

 * *            'already cloned the repository and/or installed declearn, you may skip the following '*

 * *            'commands.** Simply make sure to set your current working directory to the folder '*

 * *            'under which th […]*

```diff
@@ -19,15 +19,17 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "Clzf4NTja121"
             },
             "source": [
-                "We first clone the repo, to have both the package itself and the `examples` folder we will use in this tutorial, then naviguate to the package directory, and finally install the required dependencies"
+                "We first clone the repo, to have both the package itself and the `examples` folder we will use in this tutorial, then naviguate to the package directory, and finally install the required dependencies.\n",
+                "\n",
+                "**If you have already cloned the repository and/or installed declearn, you may skip the following commands.** Simply make sure to set your current working directory to the folder under which the `examples/mnist_quickrun` subfolder may be found (as cloned or downloaded from the repo)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -96,15 +98,17 @@
             "cell_type": "markdown",
             "metadata": {
                 "id": "KlY_vVtFHv2P"
             },
             "source": [
                 "## The model\n",
                 "\n",
-                "To do this, we will use a simple CNN, defined in `examples/mnist_quickrun/model.py`"
+                "To do this, we will use a simple CNN, defined in `examples/mnist_quickrun/model.py`.\n",
+                "\n",
+                "Here, the model is implemented in TensorFlow, which is merely an implementation detail. If you update the `config.toml` file to use the `examples/mnist_quickrun/model_torch.py`, you will train a model with the same architecture, but implemented with Torch."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -143,15 +147,16 @@
                         "Non-trainable params: 0\n",
                         "_________________________________________________________________\n"
                     ]
                 }
             ],
             "source": [
                 "from examples.mnist_quickrun.model import network\n",
-                "network.summary()"
+                "\n",
+                "network.summary()  # network is a `tensorflow.keras.Model` instance"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "HoBcOs9hH2QA"
             },
@@ -320,28 +325,28 @@
                 "We can now run our experiment. As explained in the section 2.1 of the [quickstart documentation](https://magnet.gitlabpages.inria.fr/declearn/docs/latest/quickstart), using the `declearn-quickrun` entry-point requires a configuration file, some data, and a model:\n",
                 "\n",
                 "* A TOML file, to store your experiment configurations. Here: \n",
                 "`examples/mnist_quickrun/config.toml`.\n",
                 "* A folder with your data, split by client. Here: `examples/mnist_quickrun/data_iid`\n",
                 "* A model python file, to declare your model wrapped in a `declearn` object. Here: `examples/mnist_quickrun/model.py`.\n",
                 "\n",
-                "We then only have to run the `quickrun` util with the path to the TOML file:"
+                "We then only have to run the `quickrun` coroutine with the path to the TOML file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "1n_mvTIIWpRf"
             },
             "outputs": [],
             "source": [
                 "from declearn.quickrun import quickrun\n",
                 "\n",
-                "quickrun(config=\"examples/mnist_quickrun/config.toml\")"
+                "await quickrun(config=\"examples/mnist_quickrun/config.toml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The python code above is equivalent to running `declearn-quickrun examples/mnist_quickrun/config.toml` in a shell command-line."
```

### Comparing `declearn-2.3.2/examples/mnist_quickrun/readme.md` & `declearn-2.4.0/examples/mnist_quickrun/readme.md`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/mkdocs.yml` & `declearn-2.4.0/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 repo_url: https://gitlab.inria.fr/magnet/declearn/declearn2
 repo_name: magnet/declearn
 
 markdown_extensions:
   - pymdownx.arithmatex:  # mathjax
       generic: true
+  - pymdownx.superfences  # code coloring
 
 extra:
   version:
     provider: mike
     canonical_version: latest
 
 extra_javascript:
```

### Comparing `declearn-2.3.2/pyproject.toml` & `declearn-2.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "pip >= 19",
     "setuptools >= 62.0",
     "setuptools-scm[toml] >= 6.2",
 ]
 
 [project]
 name = "declearn"
-version = "2.3.2"
+version = "2.4.0"
 description = "Declearn - a python package for private decentralized learning."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "Paul Andrey", email = "paul.andrey@inria.fr"},
     {name = "Nathan Bigaud", email = "nathan.bigaud@inria.fr"},
@@ -32,76 +32,78 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Typing :: Typed",
 ]
 dependencies = [
     "cryptography >= 35.0",
-    "fire >= 0.4",
-    "pandas >= 1.2",
+    "fire ~= 0.4",
+    "pandas >= 1.2, < 3.0",
     "requests ~= 2.18",
-    "scikit-learn >= 1.0",
-    "tomli >= 2.0 ; python_version < '3.11'",
-    "typing_extensions >= 4.0",
+    "scikit-learn ~= 1.0",
+    "tomli ~= 2.0 ; python_version < '3.11'",
+    "tqdm ~= 4.62",
+    "typing_extensions ~= 4.0",
 ]
 
 [project.optional-dependencies]
 all = [  # all non-tests extra dependencies
-    "dm-haiku ~= 0.0.9",
-    "functorch >= 1.10, < 3.0",
+    "dm-haiku >= 0.0.9, <= 0.0.11 ; python_version > '3.8'",
+    "dm-haiku >= 0.0.9, <= 0.0.10 ; python_version == '3.8'",
     "grpcio >= 1.45",
     "jax[cpu] ~= 0.4.1",
-    "opacus ~= 1.1",
+    "opacus ~= 1.4",
     "protobuf >= 3.19",
-    "tensorflow ~= 2.5",
-    "torch >= 1.10, < 3.0",
-    "websockets ~= 10.1",
+    "tensorflow ~= 2.11",
+    "torch >= 1.13, < 3.0",
+    "websockets >= 10.1, < 13.0",
 ]
 # thematically grouped dependencies (part of "all")
 dp = [
-    "opacus ~= 1.1",
+    "opacus ~= 1.4",
 ]
 grpc = [
     "grpcio >= 1.45",
     "protobuf >= 3.19",
 ]
 haiku = [
-    "dm-haiku ~= 0.0.9",
+    "dm-haiku >= 0.0.9, <= 0.0.11 ; python_version > '3.8'",
+    "dm-haiku >= 0.0.9, <= 0.0.10 ; python_version == '3.8'",
     "jax[cpu] ~= 0.4.1",  # NOTE: GPU support must be manually installed
 ]
 tensorflow = [
-    "tensorflow ~= 2.5",
+    "tensorflow ~= 2.11",
 ]
 torch = [  # generic requirements for Torch
     "torch >= 1.13, < 3.0",
 ]
 torch1 = [  # Torch 1.13 (latest pre-2.0 version)
     "torch ~= 1.13.0",
 ]
 torch2 = [  # Torch 2.X version
     "torch ~= 2.0",
 ]
 websockets = [
-    "websockets ~= 10.1",
+    "websockets >= 10.1, < 13.0",
 ]
 # docs-building dependencies
 docs = [
-    "mkdocstrings[python] >= 0.8",
-    "mkdocs-autorefs",
-    "mkdocs-literate-nav",
-    "mkdocs-material >= 9.1",
+    "mkdocstrings[python] ~= 0.8",
+    "mkdocs-autorefs ~= 0.4",
+    "mkdocs-literate-nav ~= 0.4",
+    "mkdocs-material ~= 9.1",
 ]
 # test-specific dependencies
 tests = [
-    "black ~= 23.0",
+    "black ~= 24.0",
     "mypy ~= 1.0",
-    "pylint >= 2.14",
-    "pytest >= 6.1",
-    "pytest-asyncio",
-    "pytest-cov >= 4.0",
+    "pylint ~= 3.0",
+    "pytest ~= 7.4",
+    "pytest-asyncio ~= 0.20",
+    "pytest-cov ~= 4.0",
 ]
 
 [project.urls]
 homepage = "https://magnet.gitlabpages.inria.fr/docs"
 repository = "https://gitlab.inria.fr/magnet/declearn/declearn2.git"
 
 [tool.black]
```

### Comparing `declearn-2.3.2/scripts/gen_docs.py` & `declearn-2.4.0/scripts/gen_docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,17 @@
     module: griffe.dataclasses.Module,
     docdir: str,
 ) -> Dict[str, str]:
     """Create files for public submodules of a base module."""
     pub_mod = {}
     for key, mod in module.modules.items():
         if not key.startswith("_"):
+            if isinstance(mod, griffe.dataclasses.Alias):
+                key = f"{key} (alias re-export)"
+                mod = mod.target
             pub_mod[key] = generate_module_docs(mod, docdir)
     return pub_mod
 
 
 def _generate_private_submodules_content_doc(
     module: griffe.dataclasses.Module,
     docdir: str,
```

### Comparing `declearn-2.3.2/scripts/run_tests.sh` & `declearn-2.4.0/scripts/run_tests.sh`

 * *Files 5% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     Verbosely run linters on the declearn test suite source code.
 
     Return:
         The number of sub-commands that failed (0 if successful).
     '
     commands=(
         "pylint --recursive=y test"
-        "mypy --install-types --non-interactive --exclude=conftest.py declearn"
+        "mypy --install-types --non-interactive --exclude=conftest.py test"
         "black --check test"
     )
     run_commands "declearn test code static analysis" "${commands[@]}"
 }
 
 
 run_declearn_tests() {
@@ -164,58 +164,65 @@
 
 run_unit_tests() {
     : '
     Verbosely run the declearn unit tests (excluding integration ones).
     '
     echo "Running DecLearn unit tests."
     command="pytest $@
-        --cov --cov-append --cov-report=
+        --cov=declearn --cov-append --cov-report=
         --ignore=test/functional/
         test
     "
-    run_command $command
+    echo -e "\e[34m$command\e[0m"
+    if $command; then return 0; else return 1; fi
 }
 
 
 run_integration_tests() {
     : '
     Verbosely run the declearn integration tests (skipping unit ones).
     '
     echo "Running DecLearn integration tests."
     command="pytest $@
-        --cov --cov-append --cov-report=
+        --cov=declearn --cov-append --cov-report=
         test/functional/
     "
-    run_command $command
+    echo -e "\e[34m$command\e[0m"
+    if $command; then return 0; else return 1; fi
 }
 
 
 run_torch13_tests() {
     : '
     Verbosely run Torch 1.13-specific unit tests.
 
-    Install Torch 1.13 at the start of this function, and re-install
-    torch >=2.0 at the end of it, together with its co-dependencies.
+    Install Torch 1.13 at the start of this function, and attempt
+    to re-install torch >=2.0 at the end of it, together with its
+    co- dependencies. (This last step fails with a warning when
+    the initial torch was installed from an extra index, e.g. to
+    have support for a specific CUDA version.)
     '
-    echo "Re-installing torch 1.13 and its co-dependencies."
-    pip install .[torch1]
+    echo "Installing torch 1.13 and its co-dependencies."
+    TORCH_DEPS=$(pip freeze | grep -e torch -e opacus)
+    pip install "opacus == 1.4.0" "torch ~=1.13.0"
     if [[ $? -eq 0 ]]; then
         echo "Running unit tests for torch 1.13."
         command="pytest $@
-            --cov --cov-append --cov-report=
+            --cov=declearn --cov-append --cov-report=
             test/model/test_torch_model.py
         "
-        run_command $command
+        echo -e "\e[34m$command\e[0m"
+        $command
         status=$?
     else
         echo "\e[31mSkipping tests as installation failed.\e[0m"
         status=1
     fi
     echo "Re-installing torch 2.X and its co-dependencies."
-    pip install .[torch2]
+    pip install $TORCH_DEPS
     return $status
 }
 
 
 main() {
     if [[ $# -eq 0 ]]; then
         echo "Missing required positional argument."
```

### Comparing `declearn-2.3.2/test/communication/conftest.py` & `declearn-2.4.0/test/communication/conftest.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/communication/test_exchanges.py` & `declearn-2.4.0/test/communication/test_exchanges.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,19 +39,19 @@
 import asyncio
 import secrets
 from typing import AsyncIterator, Dict, List, Optional, Tuple
 
 import pytest
 import pytest_asyncio
 
+from declearn import messaging
 from declearn.communication import (
     build_client,
     build_server,
     list_available_protocols,
-    messaging,
 )
 from declearn.communication.api import NetworkClient, NetworkServer
 
 
 ### 1. Test that connections can be properly set up.
 
 
@@ -64,18 +64,18 @@
     """Fixture to provide with an instantiated and started NetworkServer."""
     server = build_server(
         protocol=protocol,
         host="127.0.0.1",  # truly "localhost", but fails on the CI otherwise
         port=8765,
         certificate=ssl_cert["server_cert"] if ssl else None,
         private_key=ssl_cert["server_pkey"] if ssl else None,
+        heartbeat=0.1,  # fasten tests by setting a low heartbeat
     )
-    await server.start()
-    yield server
-    await server.stop()
+    async with server:
+        yield server
 
 
 def client_from_server(
     server: NetworkServer,
     c_name: str = "client",
     ca_ssl: Optional[str] = None,
 ) -> NetworkClient:
@@ -114,56 +114,55 @@
 ) -> AsyncIterator[NetworkClient]:
     """Fixture to provide with an instantiated and started NetworkClient."""
     client = client_from_server(
         server,
         c_name="client",
         ca_ssl=ssl_cert["client_cert"] if ssl else None,
     )
-    await client.start()
-    yield client
-    await client.stop()
+    async with client:
+        yield client
 
 
 @pytest.mark.parametrize("ssl", [True, False], ids=["ssl", "no_ssl"])
 @pytest.mark.parametrize("protocol", list_available_protocols())
 class TestNetworkRegister:
     """Unit tests for client-registration operations."""
 
     @pytest.mark.asyncio
     async def test_early_request(
         self, server: NetworkServer, client: NetworkClient
     ) -> None:
         """Test that early registration requests are rejected."""
-        accepted = await client.register(data_info={"test": 42})
+        accepted = await client.register()
         assert not accepted
         assert not server.client_names
 
     @pytest.mark.asyncio
     async def test_register(
         self, server: NetworkServer, client: NetworkClient
     ) -> None:
         """Test that client registration works properly."""
-        data_info, accepted = await asyncio.gather(
+        output, accepted = await asyncio.gather(
             server.wait_for_clients(1),
-            client.register(data_info={"test": 42}),
+            client.register(),
         )
-        assert data_info == {"client": {"test": 42}}
+        assert output is None
         assert accepted
         assert server.client_names == {"client"}
 
     @pytest.mark.asyncio
     async def test_register_late(
         self, server: NetworkServer, client: NetworkClient
     ) -> None:
         """Test that late client registration fails properly."""
         # Wait for clients, with a timeout.
         with pytest.raises(RuntimeError):
-            await server.wait_for_clients(timeout=1)
+            await server.wait_for_clients(timeout=0.1)
         # Try registering after that timeout.
-        accepted = await client.register(data_info={"test": 42})
+        accepted = await client.register()
         assert not accepted
 
 
 ### 3. Test that a server and its registered clients can exchange messages.
 
 
 @pytest_asyncio.fixture(name="agents")
@@ -179,16 +178,16 @@
     clients = [
         client_from_server(server, c_name=f"client-{idx}", ca_ssl=ca_ssl)
         for idx in range(n_clients)
     ]
     # Start the clients and have the server register them.
     await asyncio.gather(*[client.start() for client in clients])
     await asyncio.gather(
-        server.wait_for_clients(n_clients, timeout=2),
-        *[client.register({}) for client in clients],
+        server.wait_for_clients(n_clients, timeout=1),
+        *[client.register() for client in clients],
     )
     # Yield the server and clients. On exit, stop the clients.
     yield server, clients
     await asyncio.gather(*[client.stop() for client in clients])
 
 
 @pytest.mark.parametrize("n_clients", [1, 3], ids=["1_client", "3_clients"])
@@ -219,47 +218,58 @@
     ) -> None:
         """Test that clients can send messages to the server."""
         server, clients = agents
         coros = []
         for idx, client in enumerate(clients):
             msg = messaging.GenericMessage(action="test", params={"idx": idx})
             coros.append(client.send_message(msg))
-        messages, *_ = await asyncio.gather(server.wait_for_messages(), *coros)
+        protos, *_ = await asyncio.gather(server.wait_for_messages(), *coros)
+        assert all(
+            isinstance(proto, messaging.SerializedMessage)
+            for proto in protos.values()
+        )
+        messages = {key: proto.deserialize() for key, proto in protos.items()}
         assert messages == {
             c.name: messaging.GenericMessage(action="test", params={"idx": i})
             for i, c in enumerate(clients)
         }
 
     async def server_to_clients_broadcast(
         self,
         agents: Tuple[NetworkServer, List[NetworkClient]],
     ) -> None:
         """Test that the server can send a shared message to all clients."""
         server, clients = agents
         msg = messaging.GenericMessage(action="test", params={"value": 42})
         send = server.broadcast_message(msg)
-        recv = [client.check_message(timeout=1) for client in clients]
+        recv = [client.recv_message(timeout=1) for client in clients]
         _, *replies = await asyncio.gather(send, *recv)
-        assert all(reply == msg for reply in replies)
+        assert all(
+            isinstance(reply, messaging.SerializedMessage) for reply in replies
+        )
+        assert all(reply.deserialize() == msg for reply in replies)
 
     async def server_to_clients_individual(
         self,
         agents: Tuple[NetworkServer, List[NetworkClient]],
     ) -> None:
         """Test that the server can send individual messages to clients."""
         server, clients = agents
         messages = {
             name: messaging.GenericMessage(action="test", params={"idx": idx})
             for idx, name in enumerate(server.client_names)
         }  # type: Dict[str, messaging.Message]
         send = server.send_messages(messages)
-        recv = [client.check_message(timeout=1) for client in clients]
+        recv = [client.recv_message(timeout=1) for client in clients]
         _, *replies = await asyncio.gather(send, *recv)
         assert all(
-            reply == messages[client.name]
+            isinstance(reply, messaging.SerializedMessage) for reply in replies
+        )
+        assert all(
+            reply.deserialize() == messages[client.name]
             for client, reply in zip(clients, replies)
         )
 
     async def clients_to_server_large(
         self,
         agents: Tuple[NetworkServer, List[NetworkClient]],
     ) -> None:
@@ -268,14 +278,19 @@
         coros = []
         large = secrets.token_bytes(2**22).hex()
         for idx, client in enumerate(clients):
             msg = messaging.GenericMessage(
                 action="test", params={"idx": idx, "content": large}
             )
             coros.append(client.send_message(msg))
-        messages, *_ = await asyncio.gather(server.wait_for_messages(), *coros)
+        protos, *_ = await asyncio.gather(server.wait_for_messages(), *coros)
+        assert all(
+            isinstance(proto, messaging.SerializedMessage)
+            for proto in protos.values()
+        )
+        messages = {key: proto.deserialize() for key, proto in protos.items()}
         assert messages == {
             c.name: messaging.GenericMessage(
                 action="test", params={"idx": i, "content": large}
             )
             for i, c in enumerate(clients)
         }
```

### Comparing `declearn-2.3.2/test/communication/test_grpc.py` & `declearn-2.4.0/test/communication/test_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,38 +24,46 @@
 
 Tests dealing with more complex methods, Client/Server API enforcement and
 proper behaviour in the context of Federated Learning are left to separate
 test scripts.
 """
 
 import asyncio
+import uuid
 from typing import AsyncIterator, Dict, Iterator
 
 import grpc  # type: ignore
 import pytest
 import pytest_asyncio
 
-from declearn.communication.messaging import Empty
+from declearn.communication.api.backend.actions import Ping
 from declearn.communication.grpc._server import load_pem_file
 from declearn.communication.grpc import GrpcClient, GrpcServer
 from declearn.communication.grpc.protobufs import message_pb2
 from declearn.communication.grpc.protobufs.message_pb2_grpc import (
     MessageBoardServicer,
     MessageBoardStub,
     add_MessageBoardServicer_to_server,
 )
+from declearn.messaging import Message
 
 #################################################################
 # 0. Set up pytest fixtures to avoid redundant code in tests
 
 HOST = "localhost"
 PORT = 50051
 SERVER_URI = f"{HOST}:{PORT}"
 
 
+class StubMessage(Message):
+    """Minimal stub Message subclass."""
+
+    typekey = f"stub-{uuid.uuid4()}"
+
+
 class FakeMessageBoard(MessageBoardServicer):
     """Minimal MessageBoard implementation to test the connection."""
 
     def ping(
         self,
         request: message_pb2.Empty,
         context: grpc.ServicerContext,
@@ -63,15 +71,15 @@
         return message_pb2.Empty()
 
     def send(
         self,
         request: message_pb2.Message,
         context: grpc.ServicerContext,
     ) -> Iterator[message_pb2.Message]:
-        yield message_pb2.Message(message=Empty().to_string())
+        yield message_pb2.Message(message=Ping().to_string())
 
 
 @pytest_asyncio.fixture(name="insecure_grpc_server")
 async def insecure_grpc_server_fixture() -> AsyncIterator[grpc.Server]:
     """Create, start and return a grpc Server with unsecured communications."""
     server = grpc.aio.server()
     mboard = FakeMessageBoard()
@@ -118,34 +126,33 @@
     yield MessageBoardStub(channel)  # type: ignore
     await channel.close()
 
 
 @pytest_asyncio.fixture(name="insecure_declearn_server")
 async def insecure_declearn_server_fixture() -> AsyncIterator[GrpcServer]:
     """Create and return a GrpcServer with unsecured communications."""
-    server = GrpcServer(host=HOST, port=PORT)
-    await server.start()
-    yield server
-    await server.stop()
+    server = GrpcServer(host=HOST, port=PORT, heartbeat=0.1)
+    async with server:
+        yield server
 
 
 @pytest_asyncio.fixture(name="secure_declearn_server")
 async def secure_declearn_server_fixture(
     ssl_cert: Dict[str, str],
 ) -> AsyncIterator[GrpcServer]:
     """Create and return a GrpcServer with secured communications."""
     server = GrpcServer(
         host=HOST,
         port=PORT,
         certificate=ssl_cert["server_cert"],
         private_key=ssl_cert["server_pkey"],
+        heartbeat=0.1,
     )
-    await server.start()
-    yield server
-    await server.stop()
+    async with server:
+        yield server
 
 
 @pytest_asyncio.fixture(name="insecure_declearn_client")
 async def insecure_declearn_client_fixture() -> AsyncIterator[GrpcClient]:
     """Create and return a GrpcClient with unsecured communications."""
     client = GrpcClient(server_uri=SERVER_URI, name="client")
     await client.start()
@@ -256,38 +263,38 @@
 async def test_client_with_insecure_grpc_server(
     insecure_grpc_server: grpc.Server,
     insecure_declearn_client: GrpcClient,
 ) -> None:
     """Unit test for minimal unsecured GrpcClient use."""
     # fixture; pylint: disable=unused-argument
     client = insecure_declearn_client
-    await client.send_message(Empty())
+    await client.send_message(StubMessage())
 
 
 @pytest.mark.asyncio
 async def test_secure_client_with_secure_grpc_server(
     secure_grpc_server: grpc.Server,
     secure_declearn_client: GrpcClient,
 ) -> None:
     """Unit test for minimal secured GrpcClient use."""
     # fixture; pylint: disable=unused-argument
     client = secure_declearn_client
-    await client.send_message(Empty())
+    await client.send_message(StubMessage())
 
 
 @pytest.mark.asyncio
 async def test_insecure_client_with_secure_grpc_server_fails(
     secure_grpc_server: grpc.Server,
     insecure_declearn_client: GrpcClient,
 ) -> None:
     """Unit test for GrpcClient failure due to unproper security settings."""
     # fixture; pylint: disable=unused-argument
     client = insecure_declearn_client
     with pytest.raises(grpc.aio.AioRpcError):
-        await client.send_message(Empty())
+        await client.send_message(StubMessage())
 
 
 #################################################################
 # 4. Test the declearn Server and Client classes together
 
 
 @pytest.mark.asyncio
@@ -298,47 +305,47 @@
     """Unit test for minimal unsecured GrpcServer/GrpcClient use."""
     # fixture; pylint: disable=unused-argument
     client = insecure_declearn_client
     server = insecure_declearn_server
     await asyncio.gather(
         server.wait_for_clients(1, timeout=5), client.register({})
     )
-    await client.send_message(Empty())
+    await client.send_message(StubMessage())
 
 
 @pytest.mark.asyncio
 async def test_secure_client_with_secure_server(
     secure_declearn_server: GrpcServer,
     secure_declearn_client: GrpcClient,
 ) -> None:
     """Unit test for minimal secured GrpcServer/GrpcClient use."""
     # fixture; pylint: disable=unused-argument
     client = secure_declearn_client
     server = secure_declearn_server
     await asyncio.gather(
         server.wait_for_clients(1, timeout=5), client.register({})
     )
-    await client.send_message(Empty())
+    await client.send_message(StubMessage())
 
 
 @pytest.mark.asyncio
 async def test_insecure_client_with_secure_server_fails(
     secure_declearn_server: GrpcServer,
     insecure_declearn_client: GrpcClient,
 ) -> None:
     """Unit test for declearn-gRPC failure due to security asymmetry (1/2)."""
     # fixture; pylint: disable=unused-argument
     client = insecure_declearn_client
     with pytest.raises(grpc.aio.AioRpcError):
-        await client.send_message(Empty())
+        await client.send_message(StubMessage())
 
 
 @pytest.mark.asyncio
 async def test_secure_client_with_insecure_server_fails(
     insecure_declearn_server: GrpcServer,
     secure_declearn_client: GrpcClient,
 ) -> None:
     """Unit test for declearn-gRPC failure due to security asymmetry (2/2)."""
     # fixture; pylint: disable=unused-argument
     client = secure_declearn_client
     with pytest.raises(grpc.aio.AioRpcError):
-        await client.send_message(Empty())
+        await client.send_message(StubMessage())
```

### Comparing `declearn-2.3.2/test/communication/test_server.py` & `declearn-2.4.0/test/communication/test_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit tests for `declearn.communication.api.NetworkServer` classes."""
 
 import asyncio
-from typing import AsyncIterator, Dict
+from typing import AsyncIterator, Dict, Tuple
 from unittest import mock
 
 import pytest
 import pytest_asyncio
 
+from declearn import messaging
 from declearn.communication import (
     build_server,
     list_available_protocols,
-    messaging,
 )
 from declearn.communication.api import NetworkServer
+from declearn.communication.api.backend import MessagesHandler, actions, flags
 from declearn.utils import access_types_mapping, get_logger
+from declearn.version import VERSION
 
 
 SERVER_CLASSES = access_types_mapping("NetworkServer")
 
 
 @pytest.mark.parametrize("protocol", list_available_protocols())
 class TestNetworkServerInit:
@@ -53,15 +55,15 @@
     def test_init_minimal(self, protocol: str) -> None:
         """Test that instantiation with minimal parameters work."""
         cls = SERVER_CLASSES[protocol]
         server = cls(host="127.0.0.1", port=8765)
         assert isinstance(server, cls)
         assert server.host == "127.0.0.1"
         assert server.port == 8765
-        assert server.handler.__class__.__name__ == "MessagesHandler"
+        assert isinstance(server.handler, MessagesHandler)
 
     def test_init_ssl(self, protocol: str, ssl_cert: Dict[str, str]) -> None:
         """Test that instantiation with optional SSL parameters works."""
         cls = SERVER_CLASSES[protocol]
         server = cls(
             host="127.0.0.1",
             port=8765,
@@ -115,90 +117,87 @@
     protocol: str,
 ) -> AsyncIterator[NetworkServer]:
     """Fixture to provide with an instantiated and started NetworkServer."""
     server = build_server(
         protocol=protocol,
         host="127.0.0.1",
         port=8765,
+        heartbeat=0.1,  # fasten tests by setting a low heartbeat
     )
     async with server:
         yield server
 
 
 @pytest.mark.parametrize("protocol", list_available_protocols())
 class TestNetworkServerRegister:
     """Unit tests for `NetworkServer` client-registration methods."""
 
     @pytest.mark.asyncio
     async def test_server_early_request(self, server: NetworkServer) -> None:
         """Test that early 'JoinRequest' are adequately rejected."""
         ctx = mock.MagicMock()
-        req = messaging.JoinRequest("mock", {}).to_string()
+        req = actions.Join(name="mock", version=VERSION).to_string()
         rep = await server.handler.handle_message(req, context=ctx)
-        assert isinstance(rep, messaging.JoinReply)
-        assert not rep.accept
-        assert rep.flag == messaging.flags.REGISTRATION_UNSTARTED
+        assert isinstance(rep, actions.Reject)
+        assert rep.flag == flags.REGISTRATION_UNSTARTED
 
     @pytest.mark.asyncio
     async def test_server_await_client(self, server: NetworkServer) -> None:
         """Test 'wait_for_clients' with a single client."""
-        clients_info = asyncio.create_task(
+        wait_for_clients = asyncio.create_task(
             server.wait_for_clients(min_clients=1)
         )
-        join_request = messaging.JoinRequest("mock", {})
+        join_request = actions.Join(name="mock", version=VERSION)
         server_reply = asyncio.create_task(
             server.handler.handle_message(join_request.to_string(), context=0)
         )
-        info = await clients_info
-        assert info == {"mock": {}}
+        await wait_for_clients
         reply = await server_reply
-        assert isinstance(reply, messaging.JoinReply)
-        assert reply.accept
-        assert reply.flag == messaging.flags.REGISTERED_WELCOME
+        assert isinstance(reply, actions.Accept)
+        assert reply.flag == flags.REGISTERED_WELCOME
 
     @pytest.mark.asyncio
     async def test_server_await_timeout(self, server: NetworkServer) -> None:
         """Test 'wait_for_clients' with an expected timeout error."""
         with pytest.raises(RuntimeError):
-            await server.wait_for_clients(timeout=1)
+            await server.wait_for_clients(timeout=0.1)
 
     @pytest.mark.asyncio
     async def test_server_await_clients(self, server: NetworkServer) -> None:
         """Test 'wait_for_clients' with a race between many clients.
 
         Test that the following cases yield expected behaviors:
         - valid join request with a new name
         - valid join request with a duplicated name
         - duplicated valid join request (same context)
         - late join request (third client with only two places)
         """
         # Set up a server waiting routine and join requests' posting.
-        clients_info = server.wait_for_clients(
+        wait_clients = server.wait_for_clients(
             min_clients=1, max_clients=2, timeout=2
         )
         join_replies = []
         for idx in range(3):
-            req = messaging.JoinRequest("mock", {}).to_string()
+            req = actions.Join(name="mock", version=VERSION).to_string()
             ctx = min(idx, 1)  # first and second contexts will be the same
             join_replies.append(server.handler.handle_message(req, ctx))
         # Run the former routines concurrently. Verify server-side results.
-        results = await asyncio.gather(clients_info, *join_replies)
-        assert results[0] == {"mock": {}, "mock.1": {}}
+        results = await asyncio.gather(wait_clients, *join_replies)
+        assert results[0] is None
         # Verify request-wise replies.
         for idx, rep in enumerate(results[1:]):
-            assert isinstance(rep, messaging.JoinReply)
             if idx < 2:  # first and third requests will be accepted
-                assert rep.accept, idx
-                assert rep.flag == messaging.flags.REGISTERED_WELCOME
+                assert isinstance(rep, actions.Accept)
+                assert rep.flag == flags.REGISTERED_WELCOME
             elif idx == 2:  # second request is reundant with the first
-                assert rep.accept
-                assert rep.flag == messaging.flags.REGISTERED_ALREADY
+                assert isinstance(rep, actions.Accept)
+                assert rep.flag == flags.REGISTERED_ALREADY
             else:  # fourth request is a third client when only two are exp.
-                assert not rep.accept
-                assert rep.flag == messaging.flags.REGISTRATION_CLOSED
+                assert isinstance(rep, actions.Reject)
+                assert rep.flag == flags.REGISTRATION_CLOSED
 
 
 @pytest.mark.parametrize("protocol", list_available_protocols())
 class TestNetworkServerSend:
     """Unit tests for `NetworkServer` message-sending methods."""
 
     @pytest.mark.asyncio
@@ -208,16 +207,17 @@
         Mock the message-sending backend, that has dedicated tests.
         """
         handler = server.handler = mock.create_autospec(server.handler)
         setattr(server.handler, "client_names", {"a", "b", "c"})
         msg = messaging.GenericMessage(action="test", params={})
         await server.broadcast_message(msg)
         assert handler.send_message.await_count == 3
+        dump = msg.to_string()
         handler.send_message.assert_has_awaits(
-            [mock.call(msg, client, 1, None) for client in ("a", "b", "c")],
+            [mock.call(dump, client, None) for client in ("a", "b", "c")],
             any_order=True,
         )
 
     @pytest.mark.asyncio
     async def test_broadcast_message_subset(
         self, server: NetworkServer
     ) -> None:
@@ -225,16 +225,17 @@
 
         Mock the message-sending backend, that has dedicated tests.
         """
         handler = server.handler = mock.create_autospec(server.handler)
         msg = messaging.GenericMessage(action="test", params={})
         await server.broadcast_message(msg, clients={"a", "b"})
         assert handler.send_message.await_count == 2
+        dump = msg.to_string()
         handler.send_message.assert_has_awaits(
-            [mock.call(msg, client, 1, None) for client in ("a", "b")],
+            [mock.call(dump, client, None) for client in ("a", "b")],
             any_order=True,
         )
 
     @pytest.mark.asyncio
     async def test_send_messages(self, server: NetworkServer) -> None:
         """Test 'send_messages', mocking the message-sending backend.
 
@@ -244,15 +245,18 @@
         messages = {
             str(i): messaging.GenericMessage(action="test", params={"idx": i})
             for i in range(3)
         }  # type: Dict[str, messaging.Message]
         await server.send_messages(messages)
         assert handler.send_message.await_count == 3
         handler.send_message.assert_has_awaits(
-            [mock.call(msg, clt, 1, None) for clt, msg in messages.items()],
+            [
+                mock.call(msg.to_string(), clt, None)
+                for clt, msg in messages.items()
+            ],
             any_order=True,
         )
 
     @pytest.mark.asyncio
     async def test_send_messages_error(self, server: NetworkServer) -> None:
         """Test 'send_messages' error-raising, mocking the backend."""
         handler = server.handler = mock.create_autospec(server.handler)
@@ -266,21 +270,22 @@
 
     @pytest.mark.asyncio
     async def test_send_message(self, server: NetworkServer) -> None:
         """Test 'send_message' - enabling to mock it elsewhere."""
         server.handler.registered_clients = {0: "mock.0", 1: "mock.1"}
         msg = messaging.GenericMessage(action="test", params={})
         # Create tasks to send a message and let the client collect it.
-        req = messaging.GetMessageRequest().to_string()
+        req = actions.Recv().to_string()
         send = server.send_message(msg, client="mock.0")
         recv = server.handler.handle_message(req, 0)
         # Check that the send routine works, as does the collection one.
         outpt, reply = await asyncio.gather(send, recv)
         assert outpt is None
-        assert reply == msg
+        assert isinstance(reply, actions.Send)
+        assert reply.content == msg.to_string()
 
     @pytest.mark.asyncio
     async def test_send_message_errors(self, server: NetworkServer) -> None:
         """Test that 'send_message' raises expected exceptions."""
         server.handler.registered_clients = {0: "mock.0", 1: "mock.1"}
         msg = messaging.GenericMessage(action="test", params={})
         # Test case when sending to an unknown client.
@@ -291,84 +296,106 @@
             await server.send_message(msg, client="mock.0", timeout=1)
 
     @pytest.mark.asyncio
     async def test_reject_msg_request(self, server: NetworkServer) -> None:
         """Test that 'send_message' properly handles clients' identity."""
         server.handler.registered_clients = {0: "mock.0", 1: "mock.1"}
         msg = messaging.GenericMessage(action="test", params={})
+        req = actions.Recv(timeout=1).to_string()
         # Create tasks to send a message and have another client request one.
-        req = messaging.GetMessageRequest(timeout=1).to_string()
         send = server.send_message(msg, client="mock.0", timeout=1)
         recv = server.handler.handle_message(req, 1)
         # Check that both routines time out.
-        excpt, reply = await asyncio.gather(send, recv, return_exceptions=True)
+        excpt, reply = await asyncio.gather(
+            send, recv, return_exceptions=True
+        )  # type: Tuple[asyncio.TimeoutError, messaging.Error]
         assert isinstance(excpt, asyncio.TimeoutError)
-        assert isinstance(reply, messaging.Error)
-        assert reply.message == messaging.flags.CHECK_MESSAGE_TIMEOUT
+        assert isinstance(reply, actions.Reject)
+        assert reply.flag == flags.CHECK_MESSAGE_TIMEOUT
 
 
 @pytest.mark.parametrize("protocol", list_available_protocols())
 class TestNetworkServerRecv:
     """Unit tests for `NetworkServer` message-receiving methods."""
 
     @pytest.mark.asyncio
     async def test_wait_for_messages(self, server: NetworkServer) -> None:
         """Test that 'wait_for_messages' works correctly."""
         server.handler.registered_clients = {0: "mock.0", 1: "mock.1"}
         msg = messaging.GenericMessage(action="test", params={})
+        act = actions.Send(msg.to_string())
         # Create tasks to wait for messages, and receive them.
-        wait = server.wait_for_messages()
-        recv_0 = server.handler.handle_message(msg.to_string(), context=0)
-        recv_1 = server.handler.handle_message(msg.to_string(), context=1)
+        wait = server.wait_for_messages_with_timeout(2)
+        recv_0 = server.handler.handle_message(act.to_string(), context=0)
+        recv_1 = server.handler.handle_message(act.to_string(), context=1)
         # Await all tasks and assert that results match expectations.
         outp, reply_0, reply_1 = await asyncio.gather(wait, recv_0, recv_1)
-        assert outp == {"mock.0": msg, "mock.1": msg}
-        assert isinstance(reply_0, messaging.Empty)
-        assert isinstance(reply_1, messaging.Empty)
+        assert isinstance(outp[1], list) and not outp[1]
+        assert all(
+            isinstance(out, messaging.SerializedMessage)
+            for out in outp[0].values()
+        )
+        recv = {key: out.deserialize() for key, out in outp[0].items()}
+        assert recv == {"mock.0": msg, "mock.1": msg}
+        assert isinstance(reply_0, actions.Ping)
+        assert isinstance(reply_1, actions.Ping)
 
     @pytest.mark.asyncio
     async def test_wait_for_messages_subset(
         self, server: NetworkServer
     ) -> None:
         """Test 'wait_for_messages' for a subset of all clients."""
         server.handler.registered_clients = {0: "mock.0", 1: "mock.1"}
         msg = messaging.GenericMessage(action="test", params={})
         # Create tasks to wait for messages of the 1st client and receive it.
-        wait = server.wait_for_messages(clients={"mock.1"})
-        recv = server.handler.handle_message(msg.to_string(), context=1)
+        wait = server.wait_for_messages_with_timeout(
+            timeout=2, clients={"mock.1"}
+        )
+        recv = server.handler.handle_message(
+            actions.Send(msg.to_string()).to_string(), context=1
+        )
         # Await all tasks and assert that results match expectations.
         outp, reply = await asyncio.gather(wait, recv)
-        assert outp == {"mock.1": msg}
-        assert isinstance(reply, messaging.Empty)
+        assert isinstance(outp[1], list) and not outp[1]
+        recv = {key: out.deserialize() for key, out in outp[0].items()}
+        assert recv == {"mock.1": msg}
+        assert isinstance(reply, actions.Ping)
 
     @pytest.mark.asyncio
     async def test_wait_for_messages_errors(
         self, server: NetworkServer
     ) -> None:
         """Test that 'wait_for_messages' raises expected errors."""
         server.handler.registered_clients = {0: "mock.0", 1: "mock.1"}
         # Specify to wait for messages from an unknown client.
         with pytest.raises(KeyError):
             await server.wait_for_messages(clients={"unknown"})
         # Wait for a message that never comes, with a timeout.
-        with pytest.raises(asyncio.TimeoutError):
-            await server.wait_for_messages(timeout=1)
+        recv, miss = await server.wait_for_messages_with_timeout(timeout=1)
+        assert isinstance(recv, dict) and not recv
+        assert sorted(miss) == ["mock.0", "mock.1"]
 
     @pytest.mark.asyncio
     async def test_reject_send_request(self, server: NetworkServer) -> None:
         """Test that 'wait_for_messages' properly handles clients' identity."""
         server.handler.registered_clients = {0: "mock.0", 1: "mock.1"}
         msg_0 = messaging.GenericMessage(action="test-0", params={})
         msg_1 = messaging.GenericMessage(action="test-1", params={})
         # Create tasks to wait for messages of the 1st client and receive it.
         wait_0 = server.wait_for_messages(clients={"mock.0"})
         wait_1 = server.wait_for_messages(clients={"mock.1"})
-        recv_1 = server.handler.handle_message(msg_1.to_string(), context=1)
-        recv_0 = server.handler.handle_message(msg_0.to_string(), context=0)
+        recv_1 = server.handler.handle_message(
+            actions.Send(msg_1.to_string()).to_string(), context=1
+        )
+        recv_0 = server.handler.handle_message(
+            actions.Send(msg_0.to_string()).to_string(), context=0
+        )
         # Await all tasks and assert that results match expectations.
         outp_0, outp_1, reply_1, reply_0 = await asyncio.gather(
             wait_0, wait_1, recv_1, recv_0
         )
-        assert outp_0 == {"mock.0": msg_0}
-        assert outp_1 == {"mock.1": msg_1}
-        assert isinstance(reply_0, messaging.Empty)
-        assert isinstance(reply_1, messaging.Empty)
+        recv_0 = {key: out.deserialize() for key, out in outp_0.items()}
+        recv_1 = {key: out.deserialize() for key, out in outp_1.items()}
+        assert recv_0 == {"mock.0": msg_0}
+        assert recv_1 == {"mock.1": msg_1}
+        assert isinstance(reply_0, actions.Ping)
+        assert isinstance(reply_1, actions.Ping)
```

### Comparing `declearn-2.3.2/test/conftest.py` & `declearn-2.4.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/data_info/test_classes_field.py` & `declearn-2.4.0/test/data_info/test_classes_field.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/data_info/test_data_info_utils.py` & `declearn-2.4.0/test/data_info/test_data_info_utils.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/data_info/test_datatype_field.py` & `declearn-2.4.0/test/data_info/test_datatype_field.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/data_info/test_nbsamples_field.py` & `declearn-2.4.0/test/data_info/test_nbsamples_field.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/data_info/test_shape_field.py` & `declearn-2.4.0/test/data_info/test_shape_field.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/dataset/dataset_testbase.py` & `declearn-2.4.0/test/dataset/dataset_testbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import numpy as np
 
 from declearn.dataset import Dataset
 from declearn.test_utils import assert_batch_equal, to_numpy
 
 
 class DatasetTestToolbox:
-
     """TestCase fixture-provider protocol."""
 
     # pylint: disable=too-few-public-methods
 
     framework: str
 
     data, label, weights = (
@@ -42,16 +41,15 @@
 
     @abstractmethod
     def get_dataset(self) -> Dataset:
         """Convert the test data into a framework-specific dataset"""
 
 
 class DatasetTestSuite:
-
-    """Base tests for declearn Dataset abstract methods"""
+    """Base tests for declearn Dataset abstract methods."""
 
     def test_generate_batches_batchsize(self, toolbox: DatasetTestToolbox):
         """Test batch_size argument to test_generate_batches method"""
         expected = [
             (np.ones((2, 2)), np.array([1, 2]), np.array([1.0, 1.0])),
             (np.zeros((2, 2)), np.array([3, 4]), np.array([1.0, 1.0])),
         ]
```

### Comparing `declearn-2.3.2/test/dataset/test_dataset_utils.py` & `declearn-2.4.0/test/dataset/test_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/dataset/test_examples.py` & `declearn-2.4.0/test/dataset/test_examples.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/dataset/test_inmemory.py` & `declearn-2.4.0/test/dataset/test_inmemory.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/dataset/test_tensorflow_dataset.py` & `declearn-2.4.0/test/dataset/test_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/dataset/test_torch_dataset.py` & `declearn-2.4.0/test/dataset/test_torch_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     from dataset_testbase import DatasetTestSuite, DatasetTestToolbox
 
 
 SEED = 0
 
 
 class CustomDataset(torch.utils.data.Dataset):
-
-    """Basic torch.utils.data.Dataset for testing purposes"""
+    """Basic torch.utils.data.Dataset for testing purposes."""
 
     def __init__(self, inputs, labels, weights) -> None:
         self.inputs = inputs
         self.labels = labels
         self.weights = weights
 
     def __len__(self):
@@ -62,16 +61,15 @@
 
     def get_data_specs(self):
         """Basic get_data_spec method"""
         return {"classes": tuple(range(1, 5))}
 
 
 class TorchDatasetTestToolbox(DatasetTestToolbox):
-
-    """Toolbox for Torch Dataset"""
+    """Toolbox for Torch Dataset."""
 
     # pylint: disable=too-few-public-methods
 
     framework = "torch"
 
     def get_dataset(self) -> TorchDataset:
         return TorchDataset(
```

### Comparing `declearn-2.3.2/test/functional/conftest.py` & `declearn-2.4.0/test/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/functional/test_main.py` & `declearn-2.4.0/test/functional/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,18 +38,20 @@
 from declearn.utils import set_device_policy
 
 # Select the subset of tests to run, based on framework availability.
 # Note: TensorFlow and Torch (-related) imports are delayed due to this.
 # pylint: disable=ungrouped-imports
 FRAMEWORKS = ["Sksgd", "Tflow", "Torch"]
 try:
-    import tensorflow as tf  # type: ignore
+    import tensorflow  # type: ignore  # pylint: disable=unused-import
 except ModuleNotFoundError:
     FRAMEWORKS.remove("Tflow")
 else:
+    # pylint: disable=import-error,no-name-in-module
+    import tensorflow.keras as tf_keras  # type: ignore
     from declearn.model.tensorflow import TensorflowModel
 try:
     import torch
 except ModuleNotFoundError:
     FRAMEWORKS.remove("Torch")
 else:
     from declearn.model.torch import TorchModel
@@ -99,31 +101,31 @@
         raise ValueError("Invalid 'framework' attribute.")
 
     def _build_tflow_model(
         self,
     ) -> Model:
         """Return a TensorflowModel suitable for the learning task."""
         if self.kind == "Reg":
-            output_layer = tf.keras.layers.Dense(1)
+            output_layer = tf_keras.layers.Dense(1)
             loss = "mse"
         elif self.kind == "Bin":
-            output_layer = tf.keras.layers.Dense(1, activation="sigmoid")
+            output_layer = tf_keras.layers.Dense(1, activation="sigmoid")
             loss = "binary_crossentropy"
         elif self.kind == "Clf":
-            output_layer = tf.keras.layers.Dense(4, activation="softmax")
+            output_layer = tf_keras.layers.Dense(4, activation="softmax")
             loss = "sparse_categorical_crossentropy"
         else:
             raise ValueError("Invalid 'kind' attribute.")
         stack = [
-            tf.keras.layers.InputLayer((32,)),
-            tf.keras.layers.Dense(32, activation="relu"),
-            tf.keras.layers.Dense(8, activation="relu"),
+            tf_keras.layers.InputLayer((32,)),
+            tf_keras.layers.Dense(32, activation="relu"),
+            tf_keras.layers.Dense(8, activation="relu"),
             output_layer,
         ]
-        model = tf.keras.Sequential(stack)
+        model = tf_keras.Sequential(stack)
         return TensorflowModel(model, loss, metrics=None)
 
     def _build_torch_model(
         self,
     ) -> Model:
         """Return a TorchModel suitable for the learning task."""
         # Build the model and return it.
@@ -176,14 +178,15 @@
         """Return a NetworkServer instance."""
         return build_server(
             self.protocol,
             host="127.0.0.1",
             port=8765,
             certificate=self.ssl_cert["server_cert"] if self.use_ssl else None,
             private_key=self.ssl_cert["server_pkey"] if self.use_ssl else None,
+            heartbeat=0.1,  # fasten the tests by setting up a low heartbeat
         )
 
     def build_netwk_client(
         self,
         name: str = "client",
     ) -> NetworkClient:
         """Return a NetworkClient instance."""
```

### Comparing `declearn-2.3.2/test/functional/test_quickrun.py` & `declearn-2.4.0/test/functional/test_quickrun.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 """Functional test of the declearn quickrun example."""
 
 import os
 import pathlib
 
 import numpy as np
+import pytest
 
 from declearn.dataset import split_data
 from declearn.quickrun import quickrun
 
 
 MODEL_CODE = """
 from declearn.model.sklearn import SklearnSGDModel
@@ -33,14 +34,15 @@
 """
 
 CONFIG_TOML = """
 [network]
 protocol = "websockets"
 host = "127.0.0.1"
 port = 8080
+heartbeat = 0.1
 
 [data]
 
 [optim]
 [optim.client_opt]
 lrate = 0.01
 modules = ["adam"]
@@ -59,15 +61,16 @@
 [experiment]
 metrics = [
     ["multi-classif", {labels = [0, 1, 2, 3, 4, 5, 6, 6, 7, 8, 9]}]
 ]
 """
 
 
-def test_quickrun_mnist(tmp_path: str) -> None:
+@pytest.mark.asyncio
+async def test_quickrun_mnist(tmp_path: str) -> None:
     """Run a very basic MNIST example using 'declearn-quickrun'."""
     # Download, prepare and split the MNIST dataset into iid shards.
     split_data(tmp_path, n_shards=2, seed=0)
     # Flatten out the input images to enable their processing with sklearn.
     for path in pathlib.Path(tmp_path).glob("data_iid/client_*/*_data.npy"):
         images = np.load(path)
         np.save(path, images.reshape((-1, 28 * 28)))
@@ -75,8 +78,8 @@
     model = os.path.join(tmp_path, "model.py")
     with open(model, "w", encoding="utf-8") as file:
         file.write(MODEL_CODE)
     config = os.path.join(tmp_path, "config.toml")
     with open(config, "w", encoding="utf-8") as file:
         file.write(CONFIG_TOML)
     # Run the quickrun experiment.
-    quickrun(config)
+    await quickrun(config)
```

### Comparing `declearn-2.3.2/test/functional/test_toy_reg.py` & `declearn-2.4.0/test/functional/test_toy_reg.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,14 @@
 
 # pylint: disable=duplicate-code
 
 SEED = 0
 R2_THRESHOLD = 0.9999
 
 
-set_device_policy(gpu=False)  # disable GPU use to avoid concurrence
-
-
 def get_model(framework: FrameworkType) -> Model:
     """Set up a simple toy regression model, with zero-valued weights."""
     set_device_policy(gpu=False)  # disable GPU use to avoid concurrence
     if framework == "numpy":
         return _get_model_numpy()
     if framework == "tensorflow":
         return _get_model_tflow()
@@ -138,18 +135,19 @@
 
 def _get_model_tflow() -> TensorflowModel:
     """Return a linear model with MSE loss in TensorFlow, with zero weights."""
     tf.random.set_seed(SEED)  # set seed
     tfmod = tf.keras.Sequential(tf.keras.layers.Dense(units=1))
     tfmod.build([None, 100])
     model = TensorflowModel(tfmod, loss="mean_squared_error")
-    zeros = {
-        key: tf.zeros_like(val)
-        for key, val in model.get_weights().coefs.items()
-    }
+    with tf.device("CPU"):
+        zeros = {
+            key: tf.zeros_like(val)
+            for key, val in model.get_weights().coefs.items()
+        }
     model.set_weights(TensorflowVector(zeros))
     return model
 
 
 def _get_model_torch() -> TorchModel:
     """Return a linear model with MSE loss in Torch, with zero weights."""
     torch.manual_seed(SEED)  # set seed
@@ -166,34 +164,38 @@
     return model
 
 
 def _get_model_haiku() -> HaikuModel:
     """Return a linear model with MSE loss in Haiku, with zero weights."""
     model = HaikuModel(haiku_model_fn, loss=haiku_loss_fn)
     model.initialize({"data_type": "float32", "features_shape": (100,)})
+    zeros_like = jax.jit(jax.numpy.zeros_like, backend="cpu")
     zeros = {
-        key: jax.numpy.zeros_like(val)
-        for key, val in model.get_weights().coefs.items()
+        key: zeros_like(val) for key, val in model.get_weights().coefs.items()
     }
     model.set_weights(JaxNumpyVector(zeros))
     return model
 
 
-def get_dataset(framework: FrameworkType, inputs, labels):
+def get_dataset(
+    framework: FrameworkType,
+    inputs: np.ndarray,
+    labels: np.ndarray,
+) -> Dataset:
     """Return a framework-appropriate dataset"""
     if framework == "torch":
-        inputs = torch.from_numpy(inputs)
-        labels = torch.from_numpy(labels)
-        return TorchDataset(torch.utils.data.TensorDataset(inputs, labels))
+        pt_inp = torch.from_numpy(inputs)
+        pt_lab = torch.from_numpy(labels)
+        return TorchDataset(torch.utils.data.TensorDataset(pt_inp, pt_lab))
     if framework == "tensorflow":
-        inputs = tf.convert_to_tensor(inputs)
-        labels = tf.convert_to_tensor(labels)
-        return TensorflowDataset(
-            tf.data.Dataset.from_tensor_slices((inputs, labels))
-        )
+        with tf.device("CPU"):
+            tf_inp = tf.convert_to_tensor(inputs)
+            tf_lab = tf.convert_to_tensor(labels)
+            tf_dst = tf.data.Dataset.from_tensor_slices((tf_inp, tf_lab))
+        return TensorflowDataset(tf_dst)
     return InMemoryDataset(inputs, labels, expose_data_type=True)
 
 
 def prep_full_dataset(
     n_train: int = 300,
     n_valid: int = 150,
 ) -> Tuple[Tuple[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]]:
@@ -378,15 +380,15 @@
     clients: int = 3,
 ) -> None:
     """Routine to run a FL server, called by `run_declearn_experiment`."""
     # pylint: disable=too-many-arguments
     # Set up the FederatedServer.
     model = get_model(framework)
     netwk = NetworkServerConfig.from_params(
-        protocol="websockets", host="127.0.0.1", port=8765
+        protocol="websockets", host="127.0.0.1", port=8765, heartbeat=0.1
     )
     optim = FLOptimConfig.from_params(
         aggregator="averaging",
         client_opt={
             "lrate": lrate if framework != "numpy" else (lrate * 2),
             "regularizers": [("lasso", {"alpha": 0.1})],
         },
```

### Comparing `declearn-2.3.2/test/main/test_checkpoint.py` & `declearn-2.4.0/test/main/test_checkpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,16 +85,15 @@
     return f"{type_obj}_config.json"
 
 
 # Actual tests
 
 
 class TestCheckpointer:
-
-    """Unit tests for Checkpointer class"""
+    """Unit tests for Checkpointer class."""
 
     def test_init_default(self, tmp_path: str) -> None:
         """Test `Checkpointer.__init__` with `max_history=None`."""
         checkpointer = Checkpointer(folder=tmp_path, max_history=None)
         assert checkpointer.folder == tmp_path
         assert Path(checkpointer.folder).is_dir()
         assert checkpointer.max_history is None
```

### Comparing `declearn-2.3.2/test/main/test_data_info.py` & `declearn-2.4.0/test/main/test_data_info.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/main/test_early_stopping.py` & `declearn-2.4.0/test/main/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/main/test_train_manager.py` & `declearn-2.4.0/test/main/test_train_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 """Unit tests for `declearn.main.utils.TrainingManager`."""
 
 from unittest import mock
 from typing import Any, Iterator, Optional
 
 import numpy
 
+from declearn.aggregator import Aggregator
 from declearn.communication import messaging
 from declearn.dataset import Dataset
 from declearn.main.utils import TrainingManager
 from declearn.metrics import Metric, MetricSet
 from declearn.model.api import Model, Vector
 from declearn.optimizer import Optimizer
 
@@ -36,19 +37,22 @@
 
 
 def build_manager(n_batch: int) -> Any:  # TrainingManager with Mock attributes
     """Return a TrainingManager instance with Mock attributes."""
     model = mock.create_autospec(Model, instance=True)
     model.compute_batch_predictions.return_value = (MockArray, MockArray, None)
     optim = mock.create_autospec(Optimizer, instance=True)
+    aggrg = mock.create_autospec(Aggregator, instance=True)
     train_data = build_mock_dataset(n_batch)
     valid_data = build_mock_dataset(n_batch)
     metrics = mock.create_autospec(MetricSet, instance=True)
     metrics.metrics = []
-    return TrainingManager(model, optim, train_data, valid_data, metrics)
+    return TrainingManager(
+        model, optim, aggrg, train_data, valid_data, metrics
+    )
 
 
 def build_mock_dataset(n_batch: int) -> Dataset:
     """Build a Mock Dataset that yields a fixed number of batches."""
 
     def get_mock_batches(**_) -> Iterator[Any]:
         """Yield mock data batches."""
@@ -91,77 +95,98 @@
         manager = build_manager(n_batch=100)
         reply = manager.training_round(build_train_request(n_epoch=1))
         assert isinstance(reply, messaging.TrainReply)
         assert reply.n_epoch == 1
         assert reply.n_steps == 100
         assert manager.optim.run_train_step.call_count == 100
         manager.train_data.generate_batches.assert_called_once_with(**BATCHES)
+        manager.aggrg.prepare_for_sharing.assert_called_once_with(
+            updates=mock.ANY, n_steps=100
+        )
 
     def test_training_round_with_steps_constraint_1(self) -> None:
         """Test running a 20-steps (< 1 epoch) training round."""
         manager = build_manager(n_batch=100)
         reply = manager.training_round(build_train_request(n_steps=20))
         assert isinstance(reply, messaging.TrainReply)
         assert reply.n_epoch == 1
         assert reply.n_steps == 20
         assert manager.optim.run_train_step.call_count == 20
         manager.train_data.generate_batches.assert_called_once_with(**BATCHES)
+        manager.aggrg.prepare_for_sharing.assert_called_once_with(
+            updates=mock.ANY, n_steps=20
+        )
 
     def test_training_round_with_steps_constraint_2(self) -> None:
         """Test running a 150-steps (1.5 epochs) training round."""
         manager = build_manager(n_batch=100)
         reply = manager.training_round(build_train_request(n_steps=150))
         assert isinstance(reply, messaging.TrainReply)
         assert reply.n_epoch == 2
         assert reply.n_steps == 150
         assert manager.optim.run_train_step.call_count == 150
         assert manager.train_data.generate_batches.call_count == 2
+        manager.aggrg.prepare_for_sharing.assert_called_once_with(
+            updates=mock.ANY, n_steps=150
+        )
 
     def test_training_round_with_timeout_constraint(self) -> None:
         """Test running a time-constrained training round."""
         manager = build_manager(n_batch=100)
         reply = manager.training_round(build_train_request(timeout=0.1))
         assert isinstance(reply, messaging.TrainReply)
         assert 0.1 <= reply.t_spent
         assert manager.optim.run_train_step.call_count == reply.n_steps
         assert manager.train_data.generate_batches.call_count == reply.n_epoch
+        manager.aggrg.prepare_for_sharing.assert_called_once_with(
+            updates=mock.ANY, n_steps=reply.n_steps
+        )
 
     def test_training_round_with_multiple_constraints_1(self) -> None:
         """Test running a min(3 epoch, 150 steps) training round."""
         manager = build_manager(n_batch=100)
         request = build_train_request(n_epoch=3, n_steps=150)
         reply = manager.training_round(request)
         assert isinstance(reply, messaging.TrainReply)
         assert reply.n_epoch == 2
         assert reply.n_steps == 150
         assert manager.optim.run_train_step.call_count == 150
         assert manager.train_data.generate_batches.call_count == 2
+        manager.aggrg.prepare_for_sharing.assert_called_once_with(
+            updates=mock.ANY, n_steps=150
+        )
 
     def test_training_round_with_multiple_constraints_2(self) -> None:
         """Test running a min(3 epoch, 500 steps) training round."""
         manager = build_manager(n_batch=100)
         request = build_train_request(n_epoch=3, n_steps=500)
         reply = manager.training_round(request)
         assert isinstance(reply, messaging.TrainReply)
         assert reply.n_epoch == 3
         assert reply.n_steps == 300
         assert manager.optim.run_train_step.call_count == 300
         assert manager.train_data.generate_batches.call_count == 3
+        manager.aggrg.prepare_for_sharing.assert_called_once_with(
+            updates=mock.ANY, n_steps=300
+        )
 
     def test_training_round_with_multiple_constraints_3(self) -> None:
         """Test running a min(10 epochs, 0.1 second) training round."""
         manager = build_manager(n_batch=100)
         request = build_train_request(n_epoch=10, n_steps=1000, timeout=0.1)
         reply = manager.training_round(request)
         assert isinstance(reply, messaging.TrainReply)
         assert reply.n_epoch < 10
         assert reply.n_steps < 1000
         assert 0.1 <= reply.t_spent
         assert manager.optim.run_train_step.call_count == reply.n_steps
         assert manager.train_data.generate_batches.call_count == reply.n_epoch
+        manager.aggrg.prepare_for_sharing.assert_called_once_with(
+            updates=mock.ANY, n_steps=reply.n_steps
+        )
 
 
 def build_evaluation_request(
     n_steps: Optional[int] = None,
     timeout: Optional[float] = None,
 ) -> messaging.EvaluationRequest:
     """Return an EvaluationRequest with specified constraint parameters."""
```

### Comparing `declearn-2.3.2/test/main/test_train_manager_dp.py` & `declearn-2.4.0/test/main/test_train_manager_dp.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,35 +13,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit tests for `declearn.main.privacy.DPTrainingManager`."""
 
-import sys
+import os
 from typing import Any, Optional
 
 import pytest
 from opacus.accountants import RDPAccountant  # type: ignore
 from opacus.accountants.utils import get_noise_multiplier  # type: ignore
 
 from declearn.communication import messaging
 from declearn.dataset import DataSpecs
 from declearn.main.privacy import DPTrainingManager
 from declearn.optimizer.modules import GaussianNoiseModule
+from declearn.test_utils import make_importable
 
-
-# Relative imports from the unit tests code of the parent class.
-# pylint: disable=wrong-import-order, wrong-import-position
-# fmt: off
-sys.path.append(".")
-from test_train_manager import BATCHES, build_manager, build_train_request
-sys.path.pop()
-# pylint: enable=wrong-import-order, wrong-import-position
-# fmt: on
+with make_importable(os.path.dirname(__file__)):
+    from test_train_manager import BATCHES, build_manager, build_train_request
 
 
 BATCHES["poisson"] = True  # mock the use of Poisson sampling out of coherence
 
 
 def build_dp_manager(n_batch: int) -> Any:  # DPTrainingManager with Mock attrs
     """Return a DPTrainingManager instance with Mock attributes."""
@@ -51,15 +45,19 @@
         n_samples=n_batch * BATCHES["batch_size"],
         features_shape=(8,),  # unused
     )
     # Enable accessing the `modules` attribute of the mock Optimizer.
     base.optim.modules = []
     # Replace the base TrainingManager with a DPTrainingManager.
     return DPTrainingManager(
-        base.model, base.optim, base.train_data, base.valid_data
+        model=base.model,
+        optim=base.optim,
+        aggrg=base.aggrg,
+        train_data=base.train_data,
+        valid_data=base.valid_data,
     )
 
 
 def build_privacy_request(
     rounds: int = 1,
     n_epoch: Optional[int] = None,
     n_steps: Optional[int] = None,
```

### Comparing `declearn-2.3.2/test/metrics/test_binary_apr.py` & `declearn-2.4.0/test/metrics/test_binary_apr.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/metrics/test_binary_roc.py` & `declearn-2.4.0/test/metrics/test_binary_roc.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,30 +64,29 @@
             key: val[::2] if isinstance(val, np.ndarray) else val
             for key, val in scores.items()
         }
     elif scale != 0.1:
         raise ValueError("Unsupported 'scale' testing parameter.")
     # Compute expected aggregated states and scores.
     agg_states = {key: 2 * val for key, val in states.items()}
-    agg_states["thr"] = states["thr"]
+    agg_states["thresh"] = states["thresh"]
     agg_scores = scores.copy()
     # Instantiate a BinaryRocAUC and return a MetricTestCase.
     metric = BinaryRocAUC(scale=scale, bound=((0.2, 0.8) if bound else None))
+    supports_secagg = bound
     return MetricTestCase(
-        metric, inputs, states, scores, agg_states, agg_scores
+        metric, inputs, states, scores, agg_states, agg_scores, supports_secagg
     )
 
 
-def _test_case_1d() -> (
-    Tuple[
-        Dict[str, np.ndarray],
-        Dict[str, Union[float, np.ndarray]],
-        Dict[str, Union[float, np.ndarray]],
-    ]
-):
+def _test_case_1d() -> Tuple[
+    Dict[str, np.ndarray],
+    Dict[str, Union[float, np.ndarray]],
+    Dict[str, Union[float, np.ndarray]],
+]:
     """Return a test case with 1-D samples (standard binary classif)."""
     # similar inputs as for Binary APR; pylint: disable=duplicate-code
     inputs = {
         "y_true": np.array([0, 0, 1, 1]),
         "y_pred": np.array([4, 8, 6, 8]) / 10,
     }
     # pylint: enable=duplicate-code
@@ -100,40 +99,38 @@
         ),
         "fpos": np.array(
             [2.0, 2.0, 2.0, 2.0, 2.0, 1.0, 1.0, 1.0, 1.0, 0.0, 0.0]
         ),
         "fneg": np.array(
             [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 2.0, 2.0]
         ),
-        "thr": np.array(
+        "thresh": np.array(
             [0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
         ),
     }  # type: Dict[str, Union[float, np.ndarray]]
     scores = {
         "tpr": np.array(
             [0.0, 0.0, 0.5, 0.5, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0]
         ),
         "fpr": np.array(
             [0.0, 0.0, 0.5, 0.5, 0.5, 0.5, 1.0, 1.0, 1.0, 1.0, 1.0]
         ),
-        "thr": np.array(
+        "thresh": np.array(
             [1.0, 0.9, 0.8, 0.7, 0.6, 0.5, 0.4, 0.3, 0.2, 0.1, 0.0]
         ),
         "roc_auc": 0.625,
     }  # type: Dict[str, Union[float, np.ndarray]]
     return inputs, states, scores
 
 
-def _test_case_2d() -> (
-    Tuple[
-        Dict[str, np.ndarray],
-        Dict[str, Union[float, np.ndarray]],
-        Dict[str, Union[float, np.ndarray]],
-    ]
-):
+def _test_case_2d() -> Tuple[
+    Dict[str, np.ndarray],
+    Dict[str, Union[float, np.ndarray]],
+    Dict[str, Union[float, np.ndarray]],
+]:
     """Return a test case with 2-D samples (multilabel binary classif)."""
     # similar inputs as for Binary APR; pylint: disable=duplicate-code
     inputs = {
         "y_true": np.array(
             [
                 [0, 0, 1, 1],
                 [1, 1, 0, 0],
@@ -159,26 +156,26 @@
         ),
         "fpos": np.array(
             [6.0, 6.0, 4.0, 1.0, 1.0, 1.0, 1.0, 0.0, 0.0, 0.0, 0.0]
         ),
         "fneg": np.array(
             [0.0, 0.0, 0.0, 0.0, 0.0, 2.0, 2.0, 3.0, 3.0, 4.0, 6.0]
         ),
-        "thr": np.array(
+        "thresh": np.array(
             [0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
         ),
     }  # type: Dict[str, Union[float, np.ndarray]]
     scores = {
         "tpr": np.array(
             [0.0, 1 / 3, 0.5, 0.5, 2 / 3, 2 / 3, 1.0, 1.0, 1.0, 1.0, 1.0]
         ),
         "fpr": np.array(
             [0.0, 0.0, 0.0, 0.0, 1 / 6, 1 / 6, 1 / 6, 1 / 6, 2 / 3, 1.0, 1.0]
         ),
-        "thr": np.array(
+        "thresh": np.array(
             [1.0, 0.9, 0.8, 0.7, 0.6, 0.5, 0.4, 0.3, 0.2, 0.1, 0.0]
         ),
         "roc_auc": 0.9305555555555556,
     }  # type: Dict[str, Union[float, np.ndarray]]
     return inputs, states, scores
 
 
@@ -192,18 +189,32 @@
         """Test the aggregation of states aligned to distinct thresholds."""
         metric = test_case.metric
         metbis = BinaryRocAUC(scale=0.05, bound=(0.4, 1.2))
         metric.update(**test_case.inputs)
         metbis.update(**test_case.inputs)
         # Test that bound into bound fails as boundaries differ.
         if metric.bound:
-            with pytest.raises(ValueError):
-                metric.agg_states(metbis.get_states())
-            with pytest.raises(ValueError):
-                metbis.agg_states(metric.get_states())
-        # Test that aggregation works otherwise, with thresholds being updated.
+            with pytest.raises(TypeError):
+                metric.set_states(metbis.get_states())
+            with pytest.raises(TypeError):
+                metbis.set_states(metric.get_states())
         else:
-            metric.agg_states(metbis.get_states())
+            # Gather states from both metrics.
+            unbound = metric.get_states()
+            bounded = metbis.get_states()
+            assert type(bounded)
+            # Test that bound + unbound fails, as it would change type.
+            with pytest.raises(ValueError):
+                bounded + unbound  # pylint: disable=pointless-statement
+            # Test that assignment of unbound states into bounded metric fails.
+            with pytest.raises(TypeError):
+                metbis.set_states(unbound)
+            # Test that unbound + bound works, with thresholds being updated.
+            aggregated = unbound + bounded
+            metric.set_states(aggregated)
             assert metric.bound is None
-            thresh = metric.get_states()["thr"]
-            thrbis = metbis.get_states()["thr"]
+            thresh = metric.get_states().thresh
+            thrbis = unbound.thresh
             assert all(val in thresh for val in thrbis)
+            # Test that assignment of bounded into unbound metric works.
+            metric.set_states(bounded)
+            assert isinstance(metric.get_states(), type(unbound))
```

### Comparing `declearn-2.3.2/test/metrics/test_mae_mse.py` & `declearn-2.4.0/test/metrics/test_mae_mse.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 from typing import Dict, Literal, Union
 
 import numpy as np
 import pytest
 
 from declearn.metrics import MeanAbsoluteError, MeanSquaredError, Metric
-from declearn.test_utils import assert_dict_equal, make_importable
+from declearn.test_utils import make_importable
 
 # relative imports from `metric_testing.py`
 with make_importable(os.path.dirname(__file__)):
     from metric_testing import MetricTestCase, MetricTestSuite
 
 
 @pytest.fixture(name="test_case")
@@ -47,19 +47,19 @@
     else:
         metric = MeanSquaredError()
         errors = np.square(y_pred)
     # Compute expected results, optionally using sample weights.
     if weighted:
         s_wght = inputs["s_wght"] = np.abs(np.random.normal(size=(32,)))
         errors = errors * s_wght
-        states = {"current": errors.sum(), "divisor": s_wght.sum()}
+        states = {"num_sum": errors.sum(), "divisor": s_wght.sum()}
     else:
-        states = {"current": errors.sum(), "divisor": 32}
+        states = {"num_sum": errors.sum(), "divisor": 32}
     scores = {
-        case: states["current"] / states["divisor"]
+        case: states["num_sum"] / states["divisor"]
     }  # type: Dict[str, Union[float, np.ndarray]]
     # Compute derived aggregation results. Wrap as a test case and return.
     agg_states = {key: 2 * val for key, val in states.items()}
     agg_scores = scores.copy()
     return MetricTestCase(
         metric, inputs, states, scores, agg_states, agg_scores
     )
@@ -87,31 +87,14 @@
             metric.update(y_true, y_pred, s_wght)
 
     def test_zero_result(self, test_case: MetricTestCase) -> None:
         """Test that `get_results` works with zero-valued divisor."""
         metric = test_case.metric
         assert metric.get_result() == {metric.name: 0.0}
 
-    def test_update_expanded_shape(self, test_case: MetricTestCase) -> None:
-        """Test that the metric supports expanded-dim input predictions."""
-        # Gather states with basic inputs.
-        metric, inputs = test_case.metric, test_case.inputs
-        metric.update(**inputs)
-        states = metric.get_states()
-        metric.reset()
-        # Do the same with expanded-dim predictions.
-        metric.update(
-            inputs["y_true"],
-            np.expand_dims(inputs["y_pred"], -1),
-            inputs.get("s_wght"),
-        )
-        st_bis = metric.get_states()
-        # Verify that results are the same.
-        assert_dict_equal(states, st_bis)
-
 
 @pytest.mark.parametrize("weighted", [False, True], ids=["base", "weighted"])
 @pytest.mark.parametrize("case", ["mae"])
 class TestMeanAbsoluteError(MeanMetricTestSuite):
     """Unit tests for `MeanAbsoluteError`."""
```

### Comparing `declearn-2.3.2/test/metrics/test_metricset.py` & `declearn-2.4.0/test/metrics/test_metricset.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit tests for `declearn.metrics.MetricSet`."""
 
 from unittest import mock
-from typing import Tuple
+from typing import Dict, Tuple
 
 import numpy as np
 import pytest
 
-from declearn.metrics import MeanAbsoluteError, MeanSquaredError, MetricSet
+from declearn.metrics import (
+    MeanAbsoluteError,
+    MeanSquaredError,
+    MetricSet,
+    MetricState,
+)
 
 
 def get_mock_metricset() -> (
     Tuple[MeanAbsoluteError, MeanSquaredError, MetricSet]
 ):
     """Provide with a MetricSet wrapping mock metrics."""
     mae = mock.create_autospec(MeanAbsoluteError, instance=True)
@@ -86,15 +91,15 @@
         """Test that `MetricSet.update` works as expected."""
         mae, mse, metrics = get_mock_metricset()
         inputs = {
             "y_true": np.random.normal((8, 32)),
             "y_pred": np.random.normal((8, 32)),
             "s_wght": None,
         }
-        metrics.update(**inputs)
+        metrics.update(**inputs)  # type: ignore
         mae.update.assert_called_once_with(**inputs)  # type: ignore  # mock
         mse.update.assert_called_once_with(**inputs)  # type: ignore  # mock
 
     def test_reset(self) -> None:
         """Test that `MetricSet.reset` works as expected."""
         mae, mse, metrics = get_mock_metricset()
         metrics.reset()
@@ -105,22 +110,38 @@
         """Test that `MetricSet.get_states` works as expected."""
         mae, mse, metrics = get_mock_metricset()
         states = metrics.get_states()
         assert isinstance(states, dict)
         mae.get_states.assert_called_once()  # type: ignore  # mock
         mse.get_states.assert_called_once()  # type: ignore  # mock
 
+    def test_set_states(self) -> None:
+        """Test that `MetricSet.set_states` works as expected."""
+        mae, mse, metrics = get_mock_metricset()
+        states = {
+            "mae": mock.create_autospec(MetricState, instance=True),
+            "mse": mock.create_autospec(MetricState, instance=True),
+        }
+        metrics.set_states(states)
+        mae.set_states.assert_called_once_with(  # type: ignore  # mock
+            states["mae"]
+        )
+        mse.set_states.assert_called_once_with(  # type: ignore  # mock
+            states["mse"]
+        )
+
     def test_agg_states(self) -> None:
-        """Test that `MetricSet.agg_states` works as expected."""
+        """Test that deprecated `MetricSet.agg_states` works as expected."""
         mae, mse, metrics = get_mock_metricset()
         states = {
             "mae": mae.get_states(),
             "mse": mse.get_states(),
-        }
-        metrics.agg_states(states)
+        }  # type: Dict[str, MetricState]
+        with pytest.warns(DeprecationWarning):
+            metrics.agg_states(states)
         mae.agg_states.assert_called_once_with(states["mae"])  # type: ignore
         mse.agg_states.assert_called_once_with(states["mse"])  # type: ignore
 
     def test_get_config(self) -> None:
         """Test that `MetricSet.get_config` works as expected."""
         mae = MeanAbsoluteError()
         mse = MeanSquaredError()
```

### Comparing `declearn-2.3.2/test/metrics/test_multi_apr.py` & `declearn-2.4.0/test/metrics/test_multi_apr.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,36 +54,38 @@
         inputs["y_pred"] = inputs["y_pred"].argmax(axis=1)
     if use_lnames:
         inputs["y_true"] = np.array(["a", "b", "c"])[inputs["y_true"]]
         if not use_scores:
             inputs["y_pred"] = np.array(["a", "b", "c"])[inputs["y_pred"]]
     # Declare the asociated expected metric states and results.
     confmt = np.array([[2.0, 1.0, 0.0], [0.0, 1.0, 0.0], [1.0, 0.0, 1.0]])
-    states = {"confm": confmt}
+    states = {"confmat": confmt}
     scores = {
         "accuracy": 2 / 3,
         "precision": np.array([2 / 3, 1 / 2, 1.0]),
         "recall": np.array([2 / 3, 1.0, 1 / 2]),
         "f-score": np.array([2 / 3, 2 / 3, 2 / 3]),
         "confusion": confmt,
     }
     # Compute expected values of aggregated states and scores.
-    agg_states = {"confm": 2 * confmt}
+    agg_states = {"confmat": 2 * confmt}
     agg_scores = scores.copy()
-    agg_scores["confusion"] = agg_states["confm"]
+    agg_scores["confusion"] = agg_states["confmat"]
     # Wrap it all up into a MetricTestCase container.
     metric = MulticlassAccuracyPrecisionRecall(
         labels=["a", "b", "c"] if use_lnames else [0, 1, 2]  # type: ignore
     )
     return MetricTestCase(
         metric, inputs, states, scores, agg_states, agg_scores  # type: ignore
     )
 
 
 @pytest.mark.parametrize("use_lnames", [False, True], ids=["012", "abc"])
 @pytest.mark.parametrize("use_scores", [False, True], ids=["labels", "scores"])
 class TestMulticlassAccuracyPrecisionRecall(MetricTestSuite):
     """Unit tests for `MulticlassAccuracyPrecisionRecall`."""
 
-    def test_squeeze(self, test_case: MetricTestCase) -> None:
+    def test_update_with_squeezable_inputs(
+        self, test_case: MetricTestCase
+    ) -> None:
         with pytest.raises((AssertionError, TypeError)):
-            super().test_squeeze(test_case)
+            super().test_update_with_squeezable_inputs(test_case)
```

### Comparing `declearn-2.3.2/test/metrics/test_rsquared.py` & `declearn-2.4.0/test/metrics/test_rsquared.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,16 @@
 
     def test_zero_result(self, test_case: MetricTestCase) -> None:
         """Test that `get_results` works with zero-valued divisor."""
         metric = test_case.metric
         # Case when no samples have been seen: return 0.
         assert metric.get_result() == {metric.name: 0.0}
         # Case when SSt is null but SSr is not: return 0.
-        states = getattr(metric, "_states")
-        states["sum_of_weights"] = 1.0
-        states["sum_of_squared_errors"] = 0.1
+        states = metric.get_states()
+        states.sum_of_weights = 1.0
+        states.sum_of_squared_errors = 0.1
+        metric.set_states(states)
         assert metric.get_result() == {metric.name: 0.0}
         # Case when SSt and SSr are null but samples have been seen: return 1.
-        states["sum_of_squared_errors"] = 0.0
+        states.sum_of_squared_errors = 0.0
+        metric.set_states(states)
         assert metric.get_result() == {metric.name: 1.0}
```

### Comparing `declearn-2.3.2/test/model/model_testing.py` & `declearn-2.4.0/test/model/model_testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Shared testing code for TensorFlow and Torch models' unit tests."""
 
+import copy
 import json
 from typing import Any, Generic, List, Protocol, Tuple, Type, TypeVar, Union
 
 import numpy as np
 
 from declearn.model.api import Model, Vector
-from declearn.test_utils import to_numpy
+from declearn.test_utils import assert_json_serializable_dict, to_numpy
 from declearn.typing import Batch
 from declearn.utils import json_pack, json_unpack
 
 VectorT = TypeVar("VectorT", bound=Vector)
 
 
 class ModelTestCase(Protocol, Generic[VectorT]):
@@ -55,22 +56,31 @@
     ) -> None:
         """Raise if a vector is backed on the wrong type of device."""
 
 
 class ModelTestSuite:
     """Unit tests for a declearn Model."""
 
-    def test_serialization(
+    def test_get_config(
         self,
         test_case: ModelTestCase,
     ) -> None:
-        """Check that the model can be JSON-(de)serialized properly."""
+        """Check that the model's config is JSON-serializable."""
         model = test_case.model
-        config = json.dumps(model.get_config())
-        other = model.from_config(json.loads(config))
+        config = model.get_config()
+        assert_json_serializable_dict(config)
+
+    def test_from_config(
+        self,
+        test_case: ModelTestCase,
+    ) -> None:
+        """Check that the model can be instantiated from its config."""
+        model = test_case.model
+        config = model.get_config()
+        other = model.from_config(copy.deepcopy(config))
         assert model.get_config() == other.get_config()
         assert model.device_policy == other.device_policy
 
     def test_get_set_weights(
         self,
         test_case: ModelTestCase,
     ) -> None:
```

### Comparing `declearn-2.3.2/test/model/test_haiku_model.py` & `declearn-2.4.0/test/model/test_haiku_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,29 +24,28 @@
 import numpy as np
 import pytest
 
 try:
     import haiku as hk
     import jax
     import jax.numpy as jnp
-    from jax.config import config as jaxconfig
 except ModuleNotFoundError:
     pytest.skip("jax and/or haiku are unavailable", allow_module_level=True)
 
 from declearn.model.haiku import HaikuModel, JaxNumpyVector
 from declearn.test_utils import make_importable
 from declearn.typing import Batch
 from declearn.utils import set_device_policy
 
 # relative imports from `model_testing.py`
 with make_importable(os.path.dirname(__file__)):
     from model_testing import ModelTestCase, ModelTestSuite
 
-# Overriding float32 default in jax
-jaxconfig.update("jax_enable_x64", True)
+# Enable float64 support.
+jax.config.update("jax_enable_x64", True)
 
 
 def cnn_fn(inputs: jax.Array) -> jax.Array:
     """Simple CNN in a purely functional form"""
     stack = [
         hk.Conv2D(output_channels=32, kernel_shape=(7, 7), padding="SAME"),
         jax.nn.relu,
@@ -231,19 +230,26 @@
 
 @pytest.mark.parametrize("device", DEVICES)
 @pytest.mark.parametrize("kind", ["MLP", "MLP-tune", "RNN", "CNN"])
 class TestHaikuModel(ModelTestSuite):
     """Unit tests for declearn.model.tensorflow.TensorflowModel."""
 
     @pytest.mark.filterwarnings("ignore: Our custom Haiku serialization")
-    def test_serialization(
+    def test_get_config(
         self,
         test_case: ModelTestCase,
     ) -> None:
-        super().test_serialization(test_case)
+        super().test_get_config(test_case)
+
+    @pytest.mark.filterwarnings("ignore: Our custom Haiku serialization")
+    def test_from_config(
+        self,
+        test_case: ModelTestCase,
+    ) -> None:
+        super().test_from_config(test_case)
 
     @pytest.mark.parametrize(
         "criterion_type", ["names", "pytree", "predicate"]
     )
     def test_get_frozen_weights(
         self,
         test_case: HaikuTestCase,
```

### Comparing `declearn-2.3.2/test/model/test_sksgd_model.py` & `declearn-2.4.0/test/model/test_sksgd_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -116,23 +116,14 @@
 
 @pytest.mark.parametrize("as_sparse", [False, True], ids=["", "Sparse"])
 @pytest.mark.parametrize("s_weights", [False, True], ids=["", "SmpWgt"])
 @pytest.mark.parametrize("n_classes", [None, 2, 5], ids=["Reg", "Bin", "Clf"])
 class TestSklearnSGDModel(ModelTestSuite):
     """Unit tests for declearn.model.sklearn.SklearnSGDModel."""
 
-    def test_serialization(  # type: ignore  # Liskov does not matter here
-        self,
-        test_case: SklearnSGDTestCase,
-    ) -> None:
-        # Avoid re-running tests that are unaltered by data parameters.
-        if test_case.s_weights or test_case.as_sparse:
-            return None
-        return super().test_serialization(test_case)
-
     def test_initialization(
         self,
         test_case: SklearnSGDTestCase,
     ) -> None:
         """Check that weights are properly initialized to zero."""
         # Avoid re-running tests that are unaltered by data parameters.
         if test_case.s_weights or test_case.as_sparse:
```

### Comparing `declearn-2.3.2/test/model/test_tflow_model.py` & `declearn-2.4.0/test/model/test_tflow_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 try:
     with warnings.catch_warnings():  # silence tensorflow import-time warnings
         warnings.simplefilter("ignore")
         import tensorflow as tf  # type: ignore
 except ModuleNotFoundError:
     pytest.skip("TensorFlow is unavailable", allow_module_level=True)
+else:
+    import tensorflow.keras as tf_keras  # type: ignore
 
 from declearn.model.tensorflow import TensorflowModel, TensorflowVector
 from declearn.model.tensorflow.utils import build_keras_loss
 from declearn.test_utils import make_importable
 from declearn.typing import Batch
 from declearn.utils import set_device_policy
 
@@ -102,40 +104,40 @@
     @property
     def model(
         self,
     ) -> TensorflowModel:
         """Suited toy binary-classification keras model."""
         if self.kind.startswith("MLP"):
             stack = [
-                tf.keras.layers.Dense(32, activation="relu"),
-                tf.keras.layers.Dense(16, activation="relu"),
-                tf.keras.layers.Dense(1, activation="sigmoid"),
+                tf_keras.layers.Dense(32, activation="relu"),
+                tf_keras.layers.Dense(16, activation="relu"),
+                tf_keras.layers.Dense(1, activation="sigmoid"),
             ]
             shape = [None, 64]
             if self.kind == "MLP-tune":
                 stack[0].trainable = False
         elif self.kind == "RNN":
             stack = [
-                tf.keras.layers.Embedding(100, 32),
-                tf.keras.layers.LSTM(16, activation="tanh"),
-                tf.keras.layers.Dense(1, activation="sigmoid"),
+                tf_keras.layers.Embedding(100, 32),
+                tf_keras.layers.LSTM(16, activation="tanh"),
+                tf_keras.layers.Dense(1, activation="sigmoid"),
             ]
             shape = [None, 128]
         elif self.kind == "CNN":
             cnn_kwargs = {"padding": "same", "activation": "relu"}
             stack = [
-                tf.keras.layers.Conv2D(32, 7, **cnn_kwargs),
-                tf.keras.layers.MaxPool2D((8, 8)),
-                tf.keras.layers.Conv2D(16, 5, **cnn_kwargs),
-                tf.keras.layers.AveragePooling2D((8, 8)),
-                tf.keras.layers.Reshape((16,)),
-                tf.keras.layers.Dense(1, activation="sigmoid"),
+                tf_keras.layers.Conv2D(32, 7, **cnn_kwargs),
+                tf_keras.layers.MaxPool2D((8, 8)),
+                tf_keras.layers.Conv2D(16, 5, **cnn_kwargs),
+                tf_keras.layers.AveragePooling2D((8, 8)),
+                tf_keras.layers.Reshape((16,)),
+                tf_keras.layers.Dense(1, activation="sigmoid"),
             ]
             shape = [None, 64, 64, 3]
-        tfmod = tf.keras.Sequential(stack)
+        tfmod = tf_keras.Sequential(stack)
         tfmod.build(shape)  # as model is built, no data_info is required
         return TensorflowModel(tfmod, loss="binary_crossentropy", metrics=None)
 
     def assert_correct_device(
         self,
         vector: TensorflowVector,
     ) -> None:
@@ -169,32 +171,41 @@
     """Unit tests for declearn.model.tensorflow.TensorflowModel."""
 
     def test_get_frozen_weights(
         self,
         test_case: ModelTestCase,
     ) -> None:
         """Check that `get_weights` behaves properly with frozen weights."""
+        # Set up a model with a frozen layer.
         model = test_case.model
         tfmod = model.get_wrapped_model()
         tfmod.layers[0].trainable = False  # freeze the first layer's weights
-        w_all = model.get_weights()
-        w_trn = model.get_weights(trainable=True)
-        assert set(w_trn.coefs).issubset(w_all.coefs)  # check on keys
-        assert w_trn.coefs.keys() == {v.name for v in tfmod.trainable_weights}
-        assert w_all.coefs.keys() == {v.name for v in tfmod.weights}
+        # Access names of the model's variables (via TensorFlow/Keras API).
+        if hasattr(tf_keras, "version") and tf_keras.version().startswith("3"):
+            names_all_wghts = {v.value.name for v in tfmod.weights}
+            names_trainable = {v.value.name for v in tfmod.trainable_weights}
+        else:
+            names_all_wghts = {v.name for v in tfmod.weights}
+            names_trainable = {v.name for v in tfmod.trainable_weights}
+        # Verify that DecLearn-accessed weights' names match.
+        weights_all = model.get_weights()
+        weights_trn = model.get_weights(trainable=True)
+        assert set(weights_trn.coefs).issubset(weights_all.coefs)
+        assert weights_all.coefs.keys() == names_all_wghts
+        assert weights_trn.coefs.keys() == names_trainable
 
     def test_set_frozen_weights(
         self,
         test_case: ModelTestCase,
     ) -> None:
         """Check that `set_weights` behaves properly with frozen weights."""
         # Setup a model with some frozen weights, and gather trainable ones.
         model = test_case.model
         tfmod = model.get_wrapped_model()
-        tfmod.layers[0].trainable = False  # freeze the first layer's weights
+        tfmod.layers[-1].trainable = False  # freeze the last layer's weights
         w_trn = model.get_weights(trainable=True)
         # Test that `set_weights` works if and only if properly parametrized.
         with pytest.raises(KeyError):
             model.set_weights(w_trn)
         model.set_weights(w_trn, trainable=True)
         with pytest.raises(KeyError):
             model.set_weights(model.get_weights(), trainable=True)
@@ -206,72 +217,78 @@
         """Check that at instantiation, model weights are properly placed."""
         model = test_case.model
         policy = model.device_policy
         assert policy.gpu == (test_case.device == "GPU")
         assert policy.idx == 0
         tfmod = model.get_wrapped_model()
         device = f"{test_case.device}:0"
-        for var in tfmod.weights:
+        if hasattr(tf_keras, "version") and tf_keras.version().startswith("3"):
+            variables = [var.value for var in tfmod.weights]
+        else:
+            variables = tfmod.weights
+        for var in variables:
             assert var.device.endswith(device)
 
 
 class TestBuildKerasLoss:
     """Unit tests for `build_keras_loss` util function."""
 
     def test_build_keras_loss_from_string_class_name(self) -> None:
         """Test `build_keras_loss` with a valid class name string input."""
         loss = build_keras_loss(
-            "BinaryCrossentropy", tf.keras.losses.Reduction.SUM
+            "BinaryCrossentropy", tf_keras.losses.Reduction.SUM
         )
-        assert isinstance(loss, tf.keras.losses.BinaryCrossentropy)
-        assert loss.reduction == tf.keras.losses.Reduction.SUM
+        assert isinstance(loss, tf_keras.losses.BinaryCrossentropy)
+        assert loss.reduction == tf_keras.losses.Reduction.SUM
 
     def test_build_keras_loss_from_string_function_name(self) -> None:
         """Test `build_keras_loss` with a valid function name string input."""
         loss = build_keras_loss(
-            "binary_crossentropy", tf.keras.losses.Reduction.SUM
+            "binary_crossentropy", tf_keras.losses.Reduction.SUM
         )
-        assert isinstance(loss, tf.keras.losses.BinaryCrossentropy)
-        assert loss.reduction == tf.keras.losses.Reduction.SUM
+        assert isinstance(loss, tf_keras.losses.BinaryCrossentropy)
+        assert loss.reduction == tf_keras.losses.Reduction.SUM
 
     def test_build_keras_loss_from_string_noclass_function_name(self) -> None:
         """Test `build_keras_loss` with a valid function name string input."""
-        loss = build_keras_loss("mse", tf.keras.losses.Reduction.SUM)
-        assert isinstance(loss, tf.keras.losses.Loss)
+        if hasattr(tf_keras, "version") and tf_keras.version().startswith("3"):
+            pytest.skip("Skipping test that no longer works with Keras 3.")
+        loss = build_keras_loss("mse", tf_keras.losses.Reduction.SUM)
+        assert isinstance(loss, tf_keras.losses.Loss)
         assert hasattr(loss, "loss_fn")
-        assert loss.loss_fn is tf.keras.losses.mse
-        assert loss.reduction == tf.keras.losses.Reduction.SUM
+        assert loss.loss_fn is tf_keras.losses.mse
+        assert loss.reduction == tf_keras.losses.Reduction.SUM
 
     def test_build_keras_loss_from_loss_instance(self) -> None:
         """Test `build_keras_loss` with a valid keras Loss input."""
         # Set up a BinaryCrossentropy loss instance.
-        loss = tf.keras.losses.BinaryCrossentropy(
-            reduction=tf.keras.losses.Reduction.SUM
+        loss = tf_keras.losses.BinaryCrossentropy(
+            reduction=tf_keras.losses.Reduction.SUM
         )
-        assert loss.reduction == tf.keras.losses.Reduction.SUM
+        assert loss.reduction == tf_keras.losses.Reduction.SUM
         # Pass it through the util and verify that reduction changes.
-        loss = build_keras_loss(loss, tf.keras.losses.Reduction.NONE)
-        assert isinstance(loss, tf.keras.losses.BinaryCrossentropy)
-        assert loss.reduction == tf.keras.losses.Reduction.NONE
+        loss = build_keras_loss(loss, tf_keras.losses.Reduction.NONE)
+        assert isinstance(loss, tf_keras.losses.BinaryCrossentropy)
+        assert loss.reduction == tf_keras.losses.Reduction.NONE
 
     def test_build_keras_loss_from_loss_function(self) -> None:
         """Test `build_keras_loss` with a valid keras loss function input."""
         loss = build_keras_loss(
-            tf.keras.losses.binary_crossentropy, tf.keras.losses.Reduction.SUM
+            tf_keras.losses.binary_crossentropy, tf_keras.losses.Reduction.SUM
         )
-        assert isinstance(loss, tf.keras.losses.Loss)
+        assert isinstance(loss, tf_keras.losses.Loss)
         assert hasattr(loss, "loss_fn")
-        assert loss.loss_fn is tf.keras.losses.binary_crossentropy
-        assert loss.reduction == tf.keras.losses.Reduction.SUM
+        assert loss.loss_fn is tf_keras.losses.binary_crossentropy
+        assert loss.reduction == tf_keras.losses.Reduction.SUM
 
     def test_build_keras_loss_from_custom_function(self) -> None:
         """Test `build_keras_loss` with a valid custom loss function input."""
 
         def loss_fn(y_true: tf.Tensor, y_pred: tf.Tensor) -> tf.Tensor:
             """Custom loss function."""
             return tf.reduce_sum(tf.cast(tf.equal(y_true, y_pred), tf.float32))
 
-        loss = build_keras_loss(loss_fn, tf.keras.losses.Reduction.SUM)
-        assert isinstance(loss, tf.keras.losses.Loss)
+        loss = build_keras_loss(loss_fn, tf_keras.losses.Reduction.SUM)
+        assert isinstance(loss, tf_keras.losses.Loss)
         assert hasattr(loss, "loss_fn")
         assert loss.loss_fn is loss_fn
-        assert loss.reduction == tf.keras.losses.Reduction.SUM
+        assert loss.reduction == tf_keras.losses.Reduction.SUM
```

### Comparing `declearn-2.3.2/test/model/test_torch_model.py` & `declearn-2.4.0/test/model/test_torch_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit tests for TorchModel."""
 
-import json
+import copy
 import os
 import typing
 from typing import List, Literal, Tuple
 
 import pytest
 
 try:
@@ -215,43 +215,61 @@
 
 @pytest.mark.parametrize("device", DEVICES)
 @pytest.mark.parametrize("kind", typing.get_args(Kind))
 class TestTorchModel(ModelTestSuite):
     """Unit tests for declearn.model.torch.TorchModel."""
 
     @pytest.mark.filterwarnings("ignore: PyTorch JSON serialization")
-    def test_serialization(
+    def test_get_config(
         self,
         test_case: ModelTestCase,
     ) -> None:
         if getattr(test_case, "kind", "") == "RNN":
             # NOTE: this test fails on python 3.8 but succeeds in 3.10
             #       due to the (de)serialization of a custom nn.Module
             #       the expected model behaviour is, however, correct
             try:
-                self._test_serialization(test_case)
+                super().test_get_config(test_case)
             except AssertionError:
                 pytest.skip(
                     "skipping failed test due to custom nn.Module pickling"
                 )
-        self._test_serialization(test_case)
+        super().test_get_config(test_case)
 
-    def _test_serialization(
+    @pytest.mark.filterwarnings("ignore: PyTorch JSON serialization")
+    def test_from_config(
+        self,
+        test_case: ModelTestCase,
+    ) -> None:
+        if getattr(test_case, "kind", "") == "RNN":
+            # NOTE: this test fails on python 3.8 but succeeds in 3.10
+            #       due to the (de)serialization of a custom nn.Module
+            #       the expected model behaviour is, however, correct
+            try:
+                self._test_from_config(test_case)
+            except AssertionError:
+                pytest.skip(
+                    "skipping failed test due to custom nn.Module pickling"
+                )
+        self._test_from_config(test_case)
+
+    def _test_from_config(
         self,
         test_case: ModelTestCase,
     ) -> None:
-        """Check that the model can be JSON-(de)serialized properly.
+        """Check that the model can be instantiated from its config.
 
-        This method replaces the parent `test_serialization` one.
+        This method replaces the parent `test_from_config` one.
         """
         # Same setup as in parent test: a model and a config-based other.
         model = test_case.model
-        config = json.dumps(model.get_config())
-        other = model.from_config(json.loads(config))
-        # Verify that both models have the same device policy.
+        config = model.get_config()
+        other = model.from_config(copy.deepcopy(config))
+        # Verify that both models have the same config and device policy.
+        assert other.get_config() == config
         assert model.device_policy == other.device_policy
         # Verify that both models have a similar structure of modules.
         mod_a = list(model.get_wrapped_model().modules())
         mod_b = list(other.get_wrapped_model().modules())
         assert len(mod_a) == len(mod_b)
         assert all(isinstance(a, type(b)) for a, b in zip(mod_a, mod_b))
         assert all(repr(a) == repr(b) for a, b in zip(mod_a, mod_b))
```

### Comparing `declearn-2.3.2/test/optimizer/conftest.py` & `declearn-2.4.0/test/optimizer/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,13 +17,20 @@
 
 """Shared pytest fixtures for testing optmizer and plugins."""
 
 
 import pytest
 
 from declearn.test_utils import list_available_frameworks
+from declearn.utils import set_device_policy
 
 
 @pytest.fixture(name="framework", params=list_available_frameworks())
 def framework_fixture(request):
     """Fixture to provide with the name of a model framework."""
     return request.param
+
+
+@pytest.fixture(autouse=True)
+def disable_gpu():
+    """Ensure 'declearn.optimizer' submodule unit tests run on CPU only."""
+    set_device_policy(gpu=False)
```

### Comparing `declearn-2.3.2/test/optimizer/optim_testing.py` & `declearn-2.4.0/test/optimizer/optim_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,21 +53,21 @@
 
     @staticmethod
     def assert_equivalent(reg_a: Plugin, reg_b: Plugin) -> None:
         """Assert that two plug-ins are of same type and configuration."""
         assert type(reg_a) is type(reg_b)
         assert reg_a.get_config() == reg_b.get_config()
 
-    def test_config(self, cls: Type[Plugin]) -> None:
+    def test_rebuild_from_config(self, cls: Type[Plugin]) -> None:
         """Test a plug-in class's (get|from)_config methods."""
         plugin = cls()
         cfg = plugin.get_config()
         self.assert_equivalent(plugin, cls.from_config(cfg))
 
-    def test_specs(self, cls: Type[Plugin]) -> None:
+    def test_rebuild_from_specs(self, cls: Type[Plugin]) -> None:
         """Test that a plug-in can be rebuilt using `from_specs`."""
         plugin = cls()
         base = (
             OptiModule if isinstance(plugin, OptiModule) else Regularizer
         )  # type: Type[Union[OptiModule, Regularizer]]
         name = plugin.name
         config = plugin.get_config()
```

### Comparing `declearn-2.3.2/test/optimizer/test_modules.py` & `declearn-2.4.0/test/optimizer/test_modules.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,51 +35,48 @@
 
 import functools
 import os
 from typing import Type
 
 import pytest
 from declearn.optimizer import list_optim_modules
-from declearn.optimizer.modules import NoiseModule, OptiModule
+from declearn.optimizer.modules import AuxVar, NoiseModule, OptiModule
 from declearn.test_utils import (
     FrameworkType,
     GradientsTestCase,
     assert_dict_equal,
     assert_json_serializable_dict,
     make_importable,
 )
-from declearn.utils import set_device_policy
 
 # relative imports from `optim_testing.py`
 with make_importable(os.path.dirname(__file__)):
     from optim_testing import PluginTestBase
 
 
 # Access the list of modules to test; remove some that have dedicated tests.
 OPTIMODULE_SUBCLASSES = list_optim_modules()
 OPTIMODULE_SUBCLASSES.pop("tensorflow-optim", None)
 OPTIMODULE_SUBCLASSES.pop("torch-optim", None)
 
-set_device_policy(gpu=False)  # run all OptiModule tests on CPU
-
 
 class OptiModuleTestSuite(PluginTestBase):
     """Unit test suite for declearn.optimizer.modules.OptiModule classes."""
 
     def test_collect_aux_var(
         self, cls: Type[OptiModule], framework: FrameworkType
     ) -> None:
         """Test an OptiModule's collect_aux_var method."""
         test_case = GradientsTestCase(framework)
         module = cls()
         module.run(test_case.mock_gradient)
         aux_var = module.collect_aux_var()
-        assert (aux_var is None) or isinstance(aux_var, dict)
-        if isinstance(aux_var, dict):
-            assert_json_serializable_dict(aux_var)
+        assert (aux_var is None) or isinstance(aux_var, AuxVar)
+        if isinstance(aux_var, AuxVar):
+            assert_json_serializable_dict(aux_var.to_dict())
 
     def test_get_state_initial(self, cls: Type[OptiModule]) -> None:
         """Test an OptiModule's get_state method at instanciation."""
         module = cls()
         states = module.get_state()
         assert_json_serializable_dict(states)
```

### Comparing `declearn-2.3.2/test/optimizer/test_noise.py` & `declearn-2.4.0/test/optimizer/test_noise.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/optimizer/test_optimizer.py` & `declearn-2.4.0/test/optimizer/test_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from unittest import mock
 from uuid import uuid4
 
 import pytest
 
 from declearn.model.api import Model, Vector
 from declearn.optimizer import Optimizer
-from declearn.optimizer.modules import OptiModule
+from declearn.optimizer.modules import AuxVar, OptiModule
 from declearn.optimizer.regularizers import Regularizer
 from declearn.test_utils import assert_json_serializable_dict
 
 
 class MockOptiModule(OptiModule):
     """Type-registered mock OptiModule subclass."""
 
@@ -209,24 +209,25 @@
         mod_a.name = "mock-a"
         mod_a.aux_name = "mock"
         mod_b = mock.create_autospec(OptiModule, instance=True)
         mod_b.name = "mock-b"
         mod_b.aux_name = None
         optim = Optimizer(lrate=0.001, modules=[mod_a, mod_b])
         # Process "valid" auxiliary variables and verify their proper passing.
-        aux_var = {"mock": {"mock": "aux_vars"}}
+        aux_var = {"mock": mock.create_autospec(AuxVar, instance=True)}
         assert optim.process_aux_var(aux_var) is None
         mod_a.process_aux_var.assert_called_once_with(aux_var["mock"])
         mod_b.process_aux_var.assert_not_called()
 
     def test_process_aux_var_invalid(self) -> None:
         """Test that `Optimizer.process_aux_var` raises expected errors."""
         optim = Optimizer(lrate=0.001)
+        aux_var = {"mock": mock.create_autospec(AuxVar, instance=True)}
         with pytest.raises(KeyError):
-            optim.process_aux_var({"mock": {"mock": "aux_vars"}})
+            optim.process_aux_var(aux_var)
 
     def test_start_round(self) -> None:
         """Test, using mocks, that `Optimizer.start_round` works."""
         optim = Optimizer(
             lrate=0.001,
             regularizers=[mock.create_autospec(Regularizer)],
         )
```

### Comparing `declearn-2.3.2/test/optimizer/test_regularizers.py` & `declearn-2.4.0/test/optimizer/test_regularizers.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/optimizer/test_tflow_optim.py` & `declearn-2.4.0/test/optimizer/test_tflow_optim.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,29 +27,28 @@
 # pylint: disable=duplicate-code
 try:
     with warnings.catch_warnings():  # silence tensorflow import-time warnings
         warnings.simplefilter("ignore")
         import tensorflow as tf  # type: ignore
 except ModuleNotFoundError:
     pytest.skip("TensorFlow is unavailable", allow_module_level=True)
+else:
+    import tensorflow.keras as tf_keras  # type: ignore
 # pylint: enable=duplicate-code
 
 from declearn.model.tensorflow import TensorflowOptiModule, TensorflowVector
 from declearn.optimizer.modules import OptiModule
 from declearn.test_utils import GradientsTestCase, make_importable, to_numpy
 from declearn.utils import set_device_policy
 
 # relative imports from `test_modules.py`
 with make_importable(os.path.dirname(__file__)):
     from test_modules import OptiModuleTestSuite
 
 
-set_device_policy(gpu=False)  # force most tests to run on CPU
-
-
 DEVICES = ["CPU"]
 if tf.config.list_logical_devices("GPU"):
     DEVICES.append("GPU")
 
 
 @pytest.fixture(name="cls")
 def cls_fixture(optim: str) -> Iterator[Type[TensorflowOptiModule]]:
@@ -60,19 +59,25 @@
     TensorflowOptiModule.__init__.__defaults__ = defaults
 
 
 def get_optim_dec(optim: str) -> OptiModule:
     """Instanciate an OptiModule parameterized to match a torch one."""
     if optim == "adam":
         name = "adam"
-        kwargs = {"beta_1": 0.9, "beta_2": 0.999, "eps": 1e-07}
+        kwargs = {"beta_1": 0.9, "beta_2": 0.999, "eps": 0.0}
+        # We are disabling the use of epsilon, because keras treats it as
+        # epsilon hat (i.e. eps * (1 - beta_2^t)), which is a dishonest
+        # way of saying they are implementing the formula wrong.
+        # We implemented a hacky fix that therefore adjusts the epsilon
+        # value at each step, but for some reason we are faced with some
+        # numerical stability issue that has the test fail.
     elif optim == "rmsprop":
         name = "rmsprop"
         kwargs = {"beta": 0.9, "eps": 0.0}
-        # We are disabling the use of epsilon, because keras rmsprop divices
+        # We are disabling the use of epsilon, because keras rmsprop divides
         # outputs by sqrt(state + epsilon) instead of (sqrt(state) + epsilon)
         # which can only be corrected by pre-computing state variables, which
         # is tedious and greatly diminishes the interest for the test.
     elif optim == "adagrad":
         name = "adagrad"
         # Adjust the initial state and epsilon for a couple of reasons:
         # 1. `initial_accumulator_value=0.1` in tensorflow, but 0. in declearn
@@ -102,15 +107,15 @@
     This function therefore updates the epsilon parameter of the keras adam
     optimizer wrapped into a TensorflowOptiModule. It assumes that epsilon
     was already adjusted at all prior steps.
     """
     idx = module.optim.iterations.numpy()
     prev = np.sqrt(1 - module.optim.beta_2**idx) if idx else 1.0
     curr = np.sqrt(1 - module.optim.beta_2 ** (idx + 1))
-    module.optim.epsilon = module.optim.epsilon * curr / prev
+    module.optim.epsilon = module.optim.epsilon / prev * curr
     return module
 
 
 @pytest.fixture(name="framework")
 def framework_fixture():
     """Fixture to ensure 'TensorflowOptiModule' only receives tf gradients."""
     return "tensorflow"
@@ -136,21 +141,19 @@
         Ensure that on 10 successive passes on the same random-valued
         input gradients, outputs have the same values, up to numerical
         precision (relative tolerance of 10^-5, absolute of 10^-8).
         """
         optim_tfk = TensorflowOptiModule(optim)
         optim_dec = get_optim_dec(optim)
         gradients = GradientsTestCase("tensorflow").mock_gradient
-        if optim == "rmsprop":  # disable epsilon due to keras formula error
+        if optim in ("adam", "rmsprop"):
+            # Disable epsilon due to keras formula errors.
             optim_tfk.optim.epsilon = 0.0
         # Compare the declearn and keras implementations over 10 steps.
         for _ in range(10):
-            # Run Adam-specific fix.
-            if optim == "adam":
-                optim_tfk = fix_adam_epsilon(optim_tfk)
             # Compute gradients with both implementations.
             grads_tfk = optim_tfk.run(gradients).coefs
             grads_dec = optim_dec.run(gradients).coefs
             # Assert that the output gradients are (nearly) identical.
             assert all(
                 np.allclose(
                     to_numpy(grads_tfk[key], "tensorflow"),
@@ -196,11 +199,15 @@
         # Set the device policy, setup a module and run computations.
         set_device_policy(gpu=(device == "GPU"), idx=None)
         module = TensorflowOptiModule(optim)
         with tf.device(device):
             grads = GradientsTestCase("tensorflow").mock_gradient
         updts = module.run(grads)
         # Assert that the outputs and internal states are properly placed.
+        if hasattr(tf_keras, "version") and tf_keras.version().startswith("3"):
+            optimizer_variables = [var.value for var in module.optim.variables]
+        else:
+            optimizer_variables = module.optim.variables()
         assert all(device in t.device for t in updts.coefs.values())
-        assert all(device in t.device for t in module.optim.variables())
+        assert all(device in t.device for t in optimizer_variables)
         # Reset device policy to run other tests on CPU as expected.
         set_device_policy(gpu=False)
```

### Comparing `declearn-2.3.2/test/optimizer/test_torch_optim.py` & `declearn-2.4.0/test/optimizer/test_torch_optim.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,14 @@
 from declearn.utils import set_device_policy
 
 # relative imports from `test_modules.py`
 with make_importable(os.path.dirname(__file__)):
     from test_modules import OptiModuleTestSuite
 
 
-set_device_policy(gpu=False)  # force most tests to run on CPU
-
-
 DEVICES = ["CPU"]
 if torch.cuda.device_count():
     DEVICES.append("GPU")
 
 
 @pytest.fixture(name="optim_cls")
 def optim_cls_fixture(optim: str) -> str:
```

### Comparing `declearn-2.3.2/test/quickrun/test_quickrun_utils.py` & `declearn-2.4.0/test/quickrun/test_quickrun_utils.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/utils/test_json.py` & `declearn-2.4.0/test/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/utils/test_register.py` & `declearn-2.4.0/test/utils/test_register.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/utils/test_serialize.py` & `declearn-2.4.0/test/utils/test_serialize.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/utils/test_toml.py` & `declearn-2.4.0/test/utils/test_toml.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/vector/test_jaxnp_vector.py` & `declearn-2.4.0/test/vector/test_jaxnp_vector.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,33 +17,35 @@
 
 """Unit tests for 'declearn.model.haiku.JaxNumpyVector'."""
 
 import os
 
 import pytest
 
+# pylint: disable=duplicate-code
+
 try:
     import jax
 except ModuleNotFoundError:
     pytest.skip("jax and/or haiku are unavailable", allow_module_level=True)
 
+# pylint: enable=duplicate-code
+
 from declearn.model.haiku import JaxNumpyVector
 from declearn.model.haiku.utils import select_device
 from declearn.model.sklearn import NumpyVector
-from declearn.utils import set_device_policy
 from declearn.test_utils import make_importable
 
 with make_importable(os.path.dirname(__file__)):
     from vector_testing import VectorFactory, VectorTestSuite
 
 
+# Enable float64 support.
 jax.config.update("jax_enable_x64", True)
 
-set_device_policy(gpu=False)
-
 
 class JaxNumpyVectorFactory(VectorFactory):
     """Factory for RNG-seeded fixed-spec JaxNumpyVector instances."""
 
     framework = "jax"
     vector_cls = JaxNumpyVector
```

### Comparing `declearn-2.3.2/test/vector/test_numpy_vector.py` & `declearn-2.4.0/test/vector/test_numpy_vector.py`

 * *Files identical despite different names*

### Comparing `declearn-2.3.2/test/vector/test_tflow_vector.py` & `declearn-2.4.0/test/vector/test_tflow_vector.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,24 +24,20 @@
 try:
     import tensorflow as tf  # type: ignore
 except ModuleNotFoundError:
     pytest.skip(reason="TensorFlow is unavailable", allow_module_level=True)
 
 from declearn.model.sklearn import NumpyVector
 from declearn.model.tensorflow import TensorflowVector
-from declearn.utils import set_device_policy
 from declearn.test_utils import make_importable
 
 with make_importable(os.path.dirname(__file__)):
     from vector_testing import VectorFactory, VectorTestSuite
 
 
-set_device_policy(gpu=False)
-
-
 class TensorflowVectorFactory(VectorFactory):
     """Factory for RNG-seeded fixed-spec TensorflowVector instances."""
 
     framework = "tensorflow"
     vector_cls = TensorflowVector
 
     def make_vector(
```

### Comparing `declearn-2.3.2/test/vector/test_torch_vector.py` & `declearn-2.4.0/test/vector/test_torch_vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,20 @@
 try:
     import torch
 except ModuleNotFoundError:
     pytest.skip(reason="PyTorch is unavailable", allow_module_level=True)
 
 from declearn.model.sklearn import NumpyVector
 from declearn.model.torch import TorchVector
-from declearn.utils import set_device_policy
 from declearn.test_utils import make_importable
 
 with make_importable(os.path.dirname(__file__)):
     from vector_testing import VectorFactory, VectorTestSuite
 
 
-set_device_policy(gpu=False)
-
-
 class TorchVectorFactory(VectorFactory):
     """Factory for RNG-seeded fixed-spec TorchVector instances."""
 
     framework = "torch"
     vector_cls = TorchVector
 
     def make_vector(
```

### Comparing `declearn-2.3.2/test/vector/vector_testing.py` & `declearn-2.4.0/test/vector/vector_testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import operator
 from abc import ABCMeta, abstractmethod
 from typing import Any, Callable, Dict, ClassVar, Generic, Type, TypeVar
 
 import numpy as np
 
-from declearn.model.api import Vector
+from declearn.model.api import Vector, VectorSpec
 from declearn.test_utils import assert_json_serializable_dict, to_numpy
 
 
 __all__ = [
     "VectorFactory",
     "VectorTestSuite",
 ]
@@ -142,14 +142,55 @@
         tested Vector subclass and of its associate data types.
         """
         vector = factory.make_vector(seed=0)
         vecbis = Vector.build(vector.coefs)
         assert isinstance(vecbis, type(vector))
         assert vector == vecbis
 
+    def test_flatten(
+        self,
+        factory: VectorFactory,
+    ) -> None:
+        """Test that a Vector's `flatten` method outputs proper-type data."""
+        vector = factory.make_vector(seed=0)
+        values, v_spec = vector.flatten()
+        assert isinstance(values, list)
+        assert all(isinstance(x, float) for x in values)
+        assert isinstance(v_spec, VectorSpec)
+        assert v_spec.names == factory.names
+        assert v_spec.shapes == dict(zip(factory.names, factory.shapes))
+        assert v_spec.dtypes == dict(zip(factory.names, factory.dtypes))
+        assert isinstance(v_spec.v_type, tuple)
+        assert len(v_spec.v_type) == 2
+        assert all(isinstance(s, str) for s in v_spec.v_type)
+
+    def test_flatten_unflatten(
+        self,
+        factory: VectorFactory,
+    ) -> None:
+        """Test that a Vector can be flattened and then unflattened."""
+        vector = factory.make_vector(seed=0)
+        values, v_spec = vector.flatten()
+        vecbis = type(vector).unflatten(values, v_spec)
+        assert vector == vecbis
+
+    def test_build_from_specs(
+        self,
+        factory: VectorFactory,
+    ) -> None:
+        """Test that the `Vector.build_from_specs` generic works.
+
+        It is designed to enable unflattening a Vector from its specs.
+        """
+        vector = factory.make_vector(seed=0)
+        values, v_spec = vector.flatten()
+        vecbis = Vector.build_from_specs(values, v_spec)
+        assert isinstance(vecbis, type(vector))
+        assert vector == vecbis
+
     def test_sign(
         self,
         factory: VectorFactory,
     ) -> None:
         """Test that the sign operator of a Vector works properly."""
         vector = factory.make_vector(seed=0)
         expect = {
@@ -164,15 +205,15 @@
         factory: VectorFactory,
     ) -> None:
         """Test that the sum-reduce operator of a Vector works properly."""
         vector = factory.make_vector(seed=0)
         expect = {
             key: np.sum(to_numpy(val, factory.framework))
             for key, val in vector.coefs.items()
-        }
+        }  # type: Dict[str, np.ndarray]
         result = vector.sum()
         factory.assert_equal(expect, result)
 
 
 class VectorVectorOpTests:
     """Unit tests for operating on two same-class, same-specs Vector."""
```

