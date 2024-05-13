# Comparing `tmp/InternEvo-0.5.0.dev20240510.tar.gz` & `tmp/InternEvo-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternEvo-0.5.0.dev20240510.tar", last modified: Fri May 10 09:38:11 2024, max compression
+gzip compressed data, was "InternEvo-0.5.1.tar", last modified: Mon May 13 03:15:44 2024, max compression
```

## Comparing `InternEvo-0.5.0.dev20240510.tar` & `InternEvo-0.5.1.tar`

### file list

```diff
@@ -1,178 +1,179 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.983318 InternEvo-0.5.0.dev20240510/
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:11.966544 InternEvo-0.5.0.dev20240510/InternEvo.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5332 2024-05-10 09:38:09.000000 InternEvo-0.5.0.dev20240510/InternEvo.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4832 2024-05-10 09:38:10.000000 InternEvo-0.5.0.dev20240510/InternEvo.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-10 09:38:09.000000 InternEvo-0.5.0.dev20240510/InternEvo.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-05-10 09:38:09.000000 InternEvo-0.5.0.dev20240510/InternEvo.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-17 04:37:11.000000 InternEvo-0.5.0.dev20240510/LICENSE
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5332 2024-05-10 09:38:11.776085 InternEvo-0.5.0.dev20240510/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-22 07:03:00.000000 InternEvo-0.5.0.dev20240510/README.md
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:11.972697 InternEvo-0.5.0.dev20240510/internlm/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:33.000000 InternEvo-0.5.0.dev20240510/internlm/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.010555 InternEvo-0.5.0.dev20240510/internlm/accelerator/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/accelerator/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/accelerator/abstract_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/accelerator/cuda_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/accelerator/dipu_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/accelerator/npu_accelerator.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.025747 InternEvo-0.5.0.dev20240510/internlm/apis/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.0.dev20240510/internlm/apis/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-18 05:06:05.000000 InternEvo-0.5.0.dev20240510/internlm/apis/inference.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.067975 InternEvo-0.5.0.dev20240510/internlm/checkpoint/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 03:23:14.000000 InternEvo-0.5.0.dev20240510/internlm/checkpoint/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-04-17 07:54:15.000000 InternEvo-0.5.0.dev20240510/internlm/checkpoint/checkpoint_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-04-12 05:43:58.000000 InternEvo-0.5.0.dev20240510/internlm/checkpoint/components.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14172 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/checkpoint/load_funcs.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2474 2024-04-10 07:31:31.000000 InternEvo-0.5.0.dev20240510/internlm/checkpoint/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.105108 InternEvo-0.5.0.dev20240510/internlm/core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-17 04:37:12.000000 InternEvo-0.5.0.dev20240510/internlm/core/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.137568 InternEvo-0.5.0.dev20240510/internlm/core/context/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:13.000000 InternEvo-0.5.0.dev20240510/internlm/core/context/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/core/context/parallel_context.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:13.000000 InternEvo-0.5.0.dev20240510/internlm/core/context/process_group_initializer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/core/context/random.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 03:23:14.000000 InternEvo-0.5.0.dev20240510/internlm/core/engine.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/core/gradient_handler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8456 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/core/naive_amp.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.151538 InternEvo-0.5.0.dev20240510/internlm/core/parallel/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:36.000000 InternEvo-0.5.0.dev20240510/internlm/core/parallel/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3810 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/core/parallel/shard.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.179803 InternEvo-0.5.0.dev20240510/internlm/core/scheduler/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-06 04:29:21.000000 InternEvo-0.5.0.dev20240510/internlm/core/scheduler/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-04-25 06:33:10.000000 InternEvo-0.5.0.dev20240510/internlm/core/scheduler/base_scheduler.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.206707 InternEvo-0.5.0.dev20240510/internlm/core/scheduler/comm/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/core/scheduler/comm/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/core/scheduler/comm/p2p.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4958 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/core/scheduler/comm/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8882 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/core/scheduler/no_pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    63810 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/core/scheduler/pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-04-19 04:15:43.000000 InternEvo-0.5.0.dev20240510/internlm/core/trainer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.234290 InternEvo-0.5.0.dev20240510/internlm/data/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 03:23:14.000000 InternEvo-0.5.0.dev20240510/internlm/data/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6991 2024-04-11 07:24:57.000000 InternEvo-0.5.0.dev20240510/internlm/data/build_dataloader.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.293586 InternEvo-0.5.0.dev20240510/internlm/data/tokenized/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:25.000000 InternEvo-0.5.0.dev20240510/internlm/data/tokenized/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 03:23:14.000000 InternEvo-0.5.0.dev20240510/internlm/data/tokenized/batch_sampler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4401 2024-04-10 08:49:50.000000 InternEvo-0.5.0.dev20240510/internlm/data/tokenized/collaters.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 03:23:14.000000 InternEvo-0.5.0.dev20240510/internlm/data/tokenized/dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/data/tokenized/dummy_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1894 2024-04-10 08:49:50.000000 InternEvo-0.5.0.dev20240510/internlm/data/tokenized/dummy_dataset_multimodal.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22498 2024-04-10 12:29:02.000000 InternEvo-0.5.0.dev20240510/internlm/data/tokenized/packed_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 03:23:14.000000 InternEvo-0.5.0.dev20240510/internlm/data/tokenized/single_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 03:23:14.000000 InternEvo-0.5.0.dev20240510/internlm/data/train_state.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2546 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/data/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.311912 InternEvo-0.5.0.dev20240510/internlm/eval/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 03:23:14.000000 InternEvo-0.5.0.dev20240510/internlm/eval/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4999 2024-04-11 02:33:26.000000 InternEvo-0.5.0.dev20240510/internlm/eval/evaluation.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.343539 InternEvo-0.5.0.dev20240510/internlm/initialize/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-18 05:06:05.000000 InternEvo-0.5.0.dev20240510/internlm/initialize/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-17 04:37:12.000000 InternEvo-0.5.0.dev20240510/internlm/initialize/initialize_tensor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5934 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/initialize/initialize_trainer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27583 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/initialize/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.357684 InternEvo-0.5.0.dev20240510/internlm/initialize/legacy/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.0.dev20240510/internlm/initialize/legacy/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/initialize/legacy/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.427904 InternEvo-0.5.0.dev20240510/internlm/model/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:37.000000 InternEvo-0.5.0.dev20240510/internlm/model/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1354 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/builder.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.457385 InternEvo-0.5.0.dev20240510/internlm/model/llava/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:37.000000 InternEvo-0.5.0.dev20240510/internlm/model/llava/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      499 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/llava/clip_builder.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2674 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/llava/clip_encoder.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1407 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/llava/projector_builder.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.475024 InternEvo-0.5.0.dev20240510/internlm/model/losses/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 03:23:14.000000 InternEvo-0.5.0.dev20240510/internlm/model/losses/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1716 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/losses/ce_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16875 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/metrics.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15915 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/modeling_internlm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21691 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/modeling_internlm2.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20973 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/modeling_llama.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10481 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/modeling_llava.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    17537 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/modeling_moe.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.523733 InternEvo-0.5.0.dev20240510/internlm/model/modules/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 03:21:42.000000 InternEvo-0.5.0.dev20240510/internlm/model/modules/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13791 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/modules/embedding.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21583 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/modules/linear.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27792 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/modules/mha.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4613 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/modules/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      424 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/modules/norm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3277 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/modules/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.561423 InternEvo-0.5.0.dev20240510/internlm/model/moe/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:37.000000 InternEvo-0.5.0.dev20240510/internlm/model/moe/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/model/moe/base_layer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:13.000000 InternEvo-0.5.0.dev20240510/internlm/model/moe/experts.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20335 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/moe/gshard_layer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.596556 InternEvo-0.5.0.dev20240510/internlm/model/moe/megablock/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-17 08:44:21.000000 InternEvo-0.5.0.dev20240510/internlm/model/moe/megablock/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8669 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/moe/megablock/megablock_dmoe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13597 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/moe/megablock/megablock_moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2563 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/moe/megablock/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11288 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/moe/megablock/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4848 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/moe/moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:13.000000 InternEvo-0.5.0.dev20240510/internlm/model/moe/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.647193 InternEvo-0.5.0.dev20240510/internlm/model/ops/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 03:21:42.000000 InternEvo-0.5.0.dev20240510/internlm/model/ops/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    33645 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/ops/attention.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2084 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/ops/cross_entropy.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2400 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/ops/linear.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2489 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/ops/norm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5346 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/ops/rotary_emb.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1670 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/ops/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2952 2024-05-10 09:05:35.000000 InternEvo-0.5.0.dev20240510/internlm/model/registry.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      883 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/internlm/model/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.676275 InternEvo-0.5.0.dev20240510/internlm/monitor/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/monitor/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/monitor/alert.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/monitor/monitor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/monitor/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.690146 InternEvo-0.5.0.dev20240510/internlm/solver/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 03:23:15.000000 InternEvo-0.5.0.dev20240510/internlm/solver/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/solver/activation_checkpoint.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.740918 InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:26.000000 InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-18 05:06:05.000000 InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/base_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1946 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/compatible_adamw.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 09:32:05.000000 InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/fsdp_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42554 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/hybrid_zero_optim.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 09:32:05.000000 InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/store.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-08 13:12:12.000000 InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.761812 InternEvo-0.5.0.dev20240510/internlm/solver/schedulers/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 03:23:15.000000 InternEvo-0.5.0.dev20240510/internlm/solver/schedulers/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:42:40.000000 InternEvo-0.5.0.dev20240510/internlm/solver/schedulers/beta2_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 03:23:15.000000 InternEvo-0.5.0.dev20240510/internlm/solver/schedulers/lr_scheduler.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.784937 InternEvo-0.5.0.dev20240510/internlm/train/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      645 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/internlm/train/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27621 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/internlm/train/pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3575 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/internlm/train/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.864379 InternEvo-0.5.0.dev20240510/internlm/utils/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.0.dev20240510/internlm/utils/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7964 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/internlm/utils/common.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/utils/gputest.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2112 2024-04-10 11:15:50.000000 InternEvo-0.5.0.dev20240510/internlm/utils/logger.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/utils/megatron_timers.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3953 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/internlm/utils/parallel.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:42:40.000000 InternEvo-0.5.0.dev20240510/internlm/utils/simple_memory_profiler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/utils/storage_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 03:23:15.000000 InternEvo-0.5.0.dev20240510/internlm/utils/timeout.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4032 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/internlm/utils/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/internlm/utils/writer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-10 09:38:11.779603 InternEvo-0.5.0.dev20240510/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1103 2024-05-10 08:28:23.000000 InternEvo-0.5.0.dev20240510/setup.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.876414 InternEvo-0.5.0.dev20240510/tests/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.0.dev20240510/tests/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4526 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/tests/common_fixture.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.898596 InternEvo-0.5.0.dev20240510/tests/test_core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-18 05:04:59.000000 InternEvo-0.5.0.dev20240510/tests/test_core/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5841 2024-04-23 01:33:18.000000 InternEvo-0.5.0.dev20240510/tests/test_core/test_pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6968 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/tests/test_core/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:36:12.973241 InternEvo-0.5.0.dev20240510/tests/test_training/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-12 05:43:58.000000 InternEvo-0.5.0.dev20240510/tests/test_training/7B_check_acc.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-07 04:30:38.000000 InternEvo-0.5.0.dev20240510/tests/test_training/7B_check_init.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-18 05:04:59.000000 InternEvo-0.5.0.dev20240510/tests/test_training/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8054 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/tests/test_training/test_forward_output_no_fa.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11809 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/tests/test_training/test_load_ckpt_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14426 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/tests/test_training/test_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3855 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/tests/test_training/test_no_fa_train_temp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6773 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/tests/test_training/test_norm_weight.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12656 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/tests/test_training/test_swap_nb_loss_and_gradnorm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14290 2024-05-10 09:05:36.000000 InternEvo-0.5.0.dev20240510/tests/test_training/train_CI.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.655348 InternEvo-0.5.1/
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.428905 InternEvo-0.5.1/InternEvo.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5169 2024-05-13 03:15:42.000000 InternEvo-0.5.1/InternEvo.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4864 2024-05-13 03:15:42.000000 InternEvo-0.5.1/InternEvo.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-13 03:15:42.000000 InternEvo-0.5.1/InternEvo.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      178 2024-05-13 03:15:42.000000 InternEvo-0.5.1/InternEvo.egg-info/requires.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-05-13 03:15:42.000000 InternEvo-0.5.1/InternEvo.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-25 08:28:54.000000 InternEvo-0.5.1/LICENSE
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5169 2024-05-13 03:15:44.781929 InternEvo-0.5.1/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-25 08:28:54.000000 InternEvo-0.5.1/README.md
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.435649 InternEvo-0.5.1/internlm/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:31.000000 InternEvo-0.5.1/internlm/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.473776 InternEvo-0.5.1/internlm/accelerator/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/accelerator/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/accelerator/abstract_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/accelerator/cuda_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/accelerator/dipu_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/accelerator/npu_accelerator.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.488552 InternEvo-0.5.1/internlm/apis/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.1/internlm/apis/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-25 08:28:55.000000 InternEvo-0.5.1/internlm/apis/inference.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.534683 InternEvo-0.5.1/internlm/checkpoint/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 18:58:58.000000 InternEvo-0.5.1/internlm/checkpoint/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-04-17 07:54:31.000000 InternEvo-0.5.1/internlm/checkpoint/checkpoint_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-04-12 05:43:59.000000 InternEvo-0.5.1/internlm/checkpoint/components.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14172 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/checkpoint/load_funcs.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2474 2024-04-10 07:31:30.000000 InternEvo-0.5.1/internlm/checkpoint/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.571682 InternEvo-0.5.1/internlm/core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-25 08:28:55.000000 InternEvo-0.5.1/internlm/core/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.604386 InternEvo-0.5.1/internlm/core/context/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:10.000000 InternEvo-0.5.1/internlm/core/context/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/core/context/parallel_context.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:10.000000 InternEvo-0.5.1/internlm/core/context/process_group_initializer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/core/context/random.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 18:58:58.000000 InternEvo-0.5.1/internlm/core/engine.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/core/gradient_handler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8456 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/core/naive_amp.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.621091 InternEvo-0.5.1/internlm/core/parallel/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 08:58:45.000000 InternEvo-0.5.1/internlm/core/parallel/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3810 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/core/parallel/shard.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.651834 InternEvo-0.5.1/internlm/core/scheduler/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-08 03:13:39.000000 InternEvo-0.5.1/internlm/core/scheduler/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-03-22 07:04:00.000000 InternEvo-0.5.1/internlm/core/scheduler/base_scheduler.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.679162 InternEvo-0.5.1/internlm/core/scheduler/comm/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/core/scheduler/comm/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/core/scheduler/comm/p2p.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4958 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/core/scheduler/comm/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8882 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/core/scheduler/no_pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    63810 2024-05-11 06:37:46.000000 InternEvo-0.5.1/internlm/core/scheduler/pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-04-19 04:15:42.000000 InternEvo-0.5.1/internlm/core/trainer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.717878 InternEvo-0.5.1/internlm/data/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 18:58:58.000000 InternEvo-0.5.1/internlm/data/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6991 2024-04-11 07:14:24.000000 InternEvo-0.5.1/internlm/data/build_dataloader.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.776826 InternEvo-0.5.1/internlm/data/tokenized/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:00.000000 InternEvo-0.5.1/internlm/data/tokenized/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 18:58:58.000000 InternEvo-0.5.1/internlm/data/tokenized/batch_sampler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4401 2024-04-10 08:53:30.000000 InternEvo-0.5.1/internlm/data/tokenized/collaters.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 18:58:58.000000 InternEvo-0.5.1/internlm/data/tokenized/dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/data/tokenized/dummy_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1894 2024-04-10 08:53:30.000000 InternEvo-0.5.1/internlm/data/tokenized/dummy_dataset_multimodal.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22498 2024-04-10 13:25:54.000000 InternEvo-0.5.1/internlm/data/tokenized/packed_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 18:58:58.000000 InternEvo-0.5.1/internlm/data/tokenized/single_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 18:58:58.000000 InternEvo-0.5.1/internlm/data/train_state.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2546 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/data/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.794481 InternEvo-0.5.1/internlm/eval/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 18:58:58.000000 InternEvo-0.5.1/internlm/eval/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4999 2024-04-11 02:31:26.000000 InternEvo-0.5.1/internlm/eval/evaluation.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.844810 InternEvo-0.5.1/internlm/initialize/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-25 08:28:55.000000 InternEvo-0.5.1/internlm/initialize/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-25 08:28:55.000000 InternEvo-0.5.1/internlm/initialize/initialize_tensor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5934 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/initialize/initialize_trainer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27583 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/initialize/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.861304 InternEvo-0.5.1/internlm/initialize/legacy/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.1/internlm/initialize/legacy/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/initialize/legacy/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:43.976069 InternEvo-0.5.1/internlm/model/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 08:58:45.000000 InternEvo-0.5.1/internlm/model/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1354 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/builder.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.012759 InternEvo-0.5.1/internlm/model/llava/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 08:58:45.000000 InternEvo-0.5.1/internlm/model/llava/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      499 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/llava/clip_builder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2674 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/llava/clip_encoder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1407 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/llava/projector_builder.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.028251 InternEvo-0.5.1/internlm/model/losses/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 18:58:58.000000 InternEvo-0.5.1/internlm/model/losses/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1716 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/losses/ce_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16875 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/metrics.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15915 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/modeling_internlm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21691 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/modeling_internlm2.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20973 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/modeling_llama.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10481 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/modeling_llava.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    17537 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/modeling_moe.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.087042 InternEvo-0.5.1/internlm/model/modules/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.5.1/internlm/model/modules/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13791 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/modules/embedding.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21583 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/modules/linear.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27792 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/modules/mha.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4613 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/modules/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      424 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/modules/norm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3277 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/modules/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.133136 InternEvo-0.5.1/internlm/model/moe/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 08:58:45.000000 InternEvo-0.5.1/internlm/model/moe/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/model/moe/base_layer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:10.000000 InternEvo-0.5.1/internlm/model/moe/experts.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20335 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/moe/gshard_layer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.164403 InternEvo-0.5.1/internlm/model/moe/megablock/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-17 08:44:20.000000 InternEvo-0.5.1/internlm/model/moe/megablock/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8669 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/moe/megablock/megablock_dmoe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13597 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/moe/megablock/megablock_moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2563 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/moe/megablock/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11288 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/moe/megablock/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4848 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/moe/moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:10.000000 InternEvo-0.5.1/internlm/model/moe/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.212652 InternEvo-0.5.1/internlm/model/ops/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.5.1/internlm/model/ops/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    33645 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/ops/attention.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2084 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/ops/cross_entropy.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2400 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/ops/linear.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2489 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/ops/norm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5346 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/ops/rotary_emb.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1670 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/ops/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2952 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/registry.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      883 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/model/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.248188 InternEvo-0.5.1/internlm/monitor/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/monitor/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/monitor/alert.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/monitor/monitor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/monitor/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.262385 InternEvo-0.5.1/internlm/solver/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 18:58:59.000000 InternEvo-0.5.1/internlm/solver/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/solver/activation_checkpoint.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.322400 InternEvo-0.5.1/internlm/solver/optimizer/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:01.000000 InternEvo-0.5.1/internlm/solver/optimizer/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-25 08:28:55.000000 InternEvo-0.5.1/internlm/solver/optimizer/base_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1946 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/solver/optimizer/compatible_adamw.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 08:39:35.000000 InternEvo-0.5.1/internlm/solver/optimizer/fsdp_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42554 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/solver/optimizer/hybrid_zero_optim.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 08:39:35.000000 InternEvo-0.5.1/internlm/solver/optimizer/store.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-08 13:12:08.000000 InternEvo-0.5.1/internlm/solver/optimizer/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.344641 InternEvo-0.5.1/internlm/solver/schedulers/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 18:58:59.000000 InternEvo-0.5.1/internlm/solver/schedulers/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:26:29.000000 InternEvo-0.5.1/internlm/solver/schedulers/beta2_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 18:58:59.000000 InternEvo-0.5.1/internlm/solver/schedulers/lr_scheduler.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.370737 InternEvo-0.5.1/internlm/train/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      601 2024-05-11 06:37:46.000000 InternEvo-0.5.1/internlm/train/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    26101 2024-05-11 07:01:18.000000 InternEvo-0.5.1/internlm/train/pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3575 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/train/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.464726 InternEvo-0.5.1/internlm/utils/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.1/internlm/utils/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7964 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/utils/common.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/utils/gputest.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2112 2024-04-10 11:16:15.000000 InternEvo-0.5.1/internlm/utils/logger.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/utils/megatron_timers.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3953 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/utils/parallel.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:26:29.000000 InternEvo-0.5.1/internlm/utils/simple_memory_profiler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/utils/storage_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 18:58:59.000000 InternEvo-0.5.1/internlm/utils/timeout.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4032 2024-05-10 09:00:44.000000 InternEvo-0.5.1/internlm/utils/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-04-07 02:41:24.000000 InternEvo-0.5.1/internlm/utils/writer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-13 03:15:44.785618 InternEvo-0.5.1/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1235 2024-05-13 03:06:04.000000 InternEvo-0.5.1/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.478018 InternEvo-0.5.1/tests/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.1/tests/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4526 2024-05-10 09:00:44.000000 InternEvo-0.5.1/tests/common_fixture.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.517490 InternEvo-0.5.1/tests/test_core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.1/tests/test_core/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5841 2024-04-24 06:39:45.000000 InternEvo-0.5.1/tests/test_core/test_pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6968 2024-05-10 09:00:44.000000 InternEvo-0.5.1/tests/test_core/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:13:44.643430 InternEvo-0.5.1/tests/test_training/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-12 05:43:59.000000 InternEvo-0.5.1/tests/test_training/7B_check_acc.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-07 02:41:25.000000 InternEvo-0.5.1/tests/test_training/7B_check_init.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:46.000000 InternEvo-0.5.1/tests/test_training/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8054 2024-05-10 09:00:44.000000 InternEvo-0.5.1/tests/test_training/test_forward_output_no_fa.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11809 2024-05-10 09:00:44.000000 InternEvo-0.5.1/tests/test_training/test_load_ckpt_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14426 2024-05-10 09:00:44.000000 InternEvo-0.5.1/tests/test_training/test_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3855 2024-05-10 09:00:44.000000 InternEvo-0.5.1/tests/test_training/test_no_fa_train_temp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6773 2024-05-10 09:00:44.000000 InternEvo-0.5.1/tests/test_training/test_norm_weight.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12656 2024-05-10 09:00:44.000000 InternEvo-0.5.1/tests/test_training/test_swap_nb_loss_and_gradnorm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14290 2024-05-10 09:00:44.000000 InternEvo-0.5.1/tests/test_training/train_CI.py
```

### Comparing `InternEvo-0.5.0.dev20240510/InternEvo.egg-info/PKG-INFO` & `InternEvo-0.5.1/InternEvo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.5.0.dev20240510
+Version: 0.5.1
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # InternEvo
```

#### html2text {}

```diff
@@ -1,15 +1,13 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.5.0.dev20240510 Summary: an
-open-sourced lightweight training framework aims to support model pre-training
-without the need for extensive dependencies Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown License-File: LICENSE # InternEvo
+Metadata-Version: 2.1 Name: InternEvo Version: 0.5.1 Summary: an open-sourced
+lightweight training framework aims to support model pre-training without the
+need for extensive dependencies Classifier: Programming Language :: Python ::
+3.10 Classifier: Intended Audience :: Developers Classifier: Intended Audience
+:: Education Classifier: Intended Audience :: Science/Research Description-
+Content-Type: text/markdown License-File: LICENSE # InternEvo
                              [./doc/imgs/logo.svg]
                                       Â 
                                  IInntteerrnnEEvvoo _H_O_T
                                       Â 
   [![Documentation Status](https://readthedocs.org/projects/internevo/badge/
 ?version=latest)](https://internevo.readthedocs.io/zh_CN/latest/?badge=latest)
 [![license](./doc/imgs/license.svg)](./LICENSE) [ðUsage](./doc/en/usage.md)
```

### Comparing `InternEvo-0.5.0.dev20240510/InternEvo.egg-info/SOURCES.txt` & `InternEvo-0.5.1/InternEvo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 InternEvo.egg-info/PKG-INFO
 InternEvo.egg-info/SOURCES.txt
 InternEvo.egg-info/dependency_links.txt
+InternEvo.egg-info/requires.txt
 InternEvo.egg-info/top_level.txt
 internlm/__init__.py
 internlm/accelerator/__init__.py
 internlm/accelerator/abstract_accelerator.py
 internlm/accelerator/cuda_accelerator.py
 internlm/accelerator/dipu_accelerator.py
 internlm/accelerator/npu_accelerator.py
```

### Comparing `InternEvo-0.5.0.dev20240510/LICENSE` & `InternEvo-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/PKG-INFO` & `InternEvo-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.5.0.dev20240510
+Version: 0.5.1
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # InternEvo
```

#### html2text {}

```diff
@@ -1,15 +1,13 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.5.0.dev20240510 Summary: an
-open-sourced lightweight training framework aims to support model pre-training
-without the need for extensive dependencies Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown License-File: LICENSE # InternEvo
+Metadata-Version: 2.1 Name: InternEvo Version: 0.5.1 Summary: an open-sourced
+lightweight training framework aims to support model pre-training without the
+need for extensive dependencies Classifier: Programming Language :: Python ::
+3.10 Classifier: Intended Audience :: Developers Classifier: Intended Audience
+:: Education Classifier: Intended Audience :: Science/Research Description-
+Content-Type: text/markdown License-File: LICENSE # InternEvo
                              [./doc/imgs/logo.svg]
                                       Â 
                                  IInntteerrnnEEvvoo _H_O_T
                                       Â 
   [![Documentation Status](https://readthedocs.org/projects/internevo/badge/
 ?version=latest)](https://internevo.readthedocs.io/zh_CN/latest/?badge=latest)
 [![license](./doc/imgs/license.svg)](./LICENSE) [ðUsage](./doc/en/usage.md)
```

### Comparing `InternEvo-0.5.0.dev20240510/README.md` & `InternEvo-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/accelerator/abstract_accelerator.py` & `InternEvo-0.5.1/internlm/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/accelerator/cuda_accelerator.py` & `InternEvo-0.5.1/internlm/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/accelerator/dipu_accelerator.py` & `InternEvo-0.5.1/internlm/accelerator/dipu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/accelerator/npu_accelerator.py` & `InternEvo-0.5.1/internlm/accelerator/npu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/apis/inference.py` & `InternEvo-0.5.1/internlm/apis/inference.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/checkpoint/checkpoint_manager.py` & `InternEvo-0.5.1/internlm/checkpoint/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/checkpoint/components.py` & `InternEvo-0.5.1/internlm/checkpoint/components.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/checkpoint/load_funcs.py` & `InternEvo-0.5.1/internlm/checkpoint/load_funcs.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/checkpoint/utils.py` & `InternEvo-0.5.1/internlm/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/context/__init__.py` & `InternEvo-0.5.1/internlm/core/context/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/context/parallel_context.py` & `InternEvo-0.5.1/internlm/core/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/context/process_group_initializer.py` & `InternEvo-0.5.1/internlm/core/context/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/context/random.py` & `InternEvo-0.5.1/internlm/core/context/random.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/engine.py` & `InternEvo-0.5.1/internlm/core/engine.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/gradient_handler.py` & `InternEvo-0.5.1/internlm/core/gradient_handler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/naive_amp.py` & `InternEvo-0.5.1/internlm/core/naive_amp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/parallel/shard.py` & `InternEvo-0.5.1/internlm/core/parallel/shard.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/scheduler/base_scheduler.py` & `InternEvo-0.5.1/internlm/core/scheduler/base_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/scheduler/comm/__init__.py` & `InternEvo-0.5.1/internlm/core/scheduler/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/scheduler/comm/p2p.py` & `InternEvo-0.5.1/internlm/core/scheduler/comm/p2p.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/scheduler/comm/utils.py` & `InternEvo-0.5.1/internlm/core/scheduler/comm/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/scheduler/no_pipeline_scheduler.py` & `InternEvo-0.5.1/internlm/core/scheduler/no_pipeline_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/scheduler/pipeline_scheduler.py` & `InternEvo-0.5.1/internlm/core/scheduler/pipeline_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/core/trainer.py` & `InternEvo-0.5.1/internlm/core/trainer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/data/build_dataloader.py` & `InternEvo-0.5.1/internlm/data/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/data/tokenized/batch_sampler.py` & `InternEvo-0.5.1/internlm/data/tokenized/batch_sampler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/data/tokenized/collaters.py` & `InternEvo-0.5.1/internlm/data/tokenized/collaters.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/data/tokenized/dataset.py` & `InternEvo-0.5.1/internlm/data/tokenized/dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/data/tokenized/dummy_dataset.py` & `InternEvo-0.5.1/internlm/data/tokenized/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/data/tokenized/dummy_dataset_multimodal.py` & `InternEvo-0.5.1/internlm/data/tokenized/dummy_dataset_multimodal.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/data/tokenized/packed_dataset.py` & `InternEvo-0.5.1/internlm/data/tokenized/packed_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/data/tokenized/single_dataset.py` & `InternEvo-0.5.1/internlm/data/tokenized/single_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/data/utils.py` & `InternEvo-0.5.1/internlm/data/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/eval/evaluation.py` & `InternEvo-0.5.1/internlm/eval/evaluation.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/initialize/initialize_tensor.py` & `InternEvo-0.5.1/internlm/initialize/initialize_tensor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/initialize/initialize_trainer.py` & `InternEvo-0.5.1/internlm/initialize/initialize_trainer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/initialize/launch.py` & `InternEvo-0.5.1/internlm/initialize/launch.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/initialize/legacy/launch.py` & `InternEvo-0.5.1/internlm/initialize/legacy/launch.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/builder.py` & `InternEvo-0.5.1/internlm/model/builder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/llava/clip_encoder.py` & `InternEvo-0.5.1/internlm/model/llava/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/llava/projector_builder.py` & `InternEvo-0.5.1/internlm/model/llava/projector_builder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/losses/ce_loss.py` & `InternEvo-0.5.1/internlm/model/losses/ce_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/metrics.py` & `InternEvo-0.5.1/internlm/model/metrics.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/modeling_internlm.py` & `InternEvo-0.5.1/internlm/model/modeling_internlm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/modeling_internlm2.py` & `InternEvo-0.5.1/internlm/model/modeling_internlm2.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/modeling_llama.py` & `InternEvo-0.5.1/internlm/model/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/modeling_llava.py` & `InternEvo-0.5.1/internlm/model/modeling_llava.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/modeling_moe.py` & `InternEvo-0.5.1/internlm/model/modeling_moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/modules/embedding.py` & `InternEvo-0.5.1/internlm/model/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/modules/linear.py` & `InternEvo-0.5.1/internlm/model/modules/linear.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/modules/mha.py` & `InternEvo-0.5.1/internlm/model/modules/mha.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/modules/mlp.py` & `InternEvo-0.5.1/internlm/model/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/modules/utils.py` & `InternEvo-0.5.1/internlm/model/modules/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/moe/base_layer.py` & `InternEvo-0.5.1/internlm/model/moe/base_layer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/moe/experts.py` & `InternEvo-0.5.1/internlm/model/moe/experts.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/moe/gshard_layer.py` & `InternEvo-0.5.1/internlm/model/moe/gshard_layer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/moe/megablock/megablock_dmoe.py` & `InternEvo-0.5.1/internlm/model/moe/megablock/megablock_dmoe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/moe/megablock/megablock_moe.py` & `InternEvo-0.5.1/internlm/model/moe/megablock/megablock_moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/moe/megablock/mlp.py` & `InternEvo-0.5.1/internlm/model/moe/megablock/mlp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/moe/megablock/utils.py` & `InternEvo-0.5.1/internlm/model/moe/megablock/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/moe/moe.py` & `InternEvo-0.5.1/internlm/model/moe/moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/moe/utils.py` & `InternEvo-0.5.1/internlm/model/moe/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/ops/attention.py` & `InternEvo-0.5.1/internlm/model/ops/attention.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/ops/cross_entropy.py` & `InternEvo-0.5.1/internlm/model/ops/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/ops/linear.py` & `InternEvo-0.5.1/internlm/model/ops/linear.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/ops/norm.py` & `InternEvo-0.5.1/internlm/model/ops/norm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/ops/rotary_emb.py` & `InternEvo-0.5.1/internlm/model/ops/rotary_emb.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/ops/utils.py` & `InternEvo-0.5.1/internlm/model/ops/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/registry.py` & `InternEvo-0.5.1/internlm/model/registry.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/model/utils.py` & `InternEvo-0.5.1/internlm/model/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/monitor/alert.py` & `InternEvo-0.5.1/internlm/monitor/alert.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/monitor/monitor.py` & `InternEvo-0.5.1/internlm/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/monitor/utils.py` & `InternEvo-0.5.1/internlm/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/solver/activation_checkpoint.py` & `InternEvo-0.5.1/internlm/solver/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/base_optimizer.py` & `InternEvo-0.5.1/internlm/solver/optimizer/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/compatible_adamw.py` & `InternEvo-0.5.1/internlm/solver/optimizer/compatible_adamw.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/fsdp_optimizer.py` & `InternEvo-0.5.1/internlm/solver/optimizer/fsdp_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/hybrid_zero_optim.py` & `InternEvo-0.5.1/internlm/solver/optimizer/hybrid_zero_optim.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/store.py` & `InternEvo-0.5.1/internlm/solver/optimizer/store.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/solver/optimizer/utils.py` & `InternEvo-0.5.1/internlm/solver/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/solver/schedulers/beta2_scheduler.py` & `InternEvo-0.5.1/internlm/solver/schedulers/beta2_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/solver/schedulers/lr_scheduler.py` & `InternEvo-0.5.1/internlm/solver/schedulers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/train/__init__.py` & `InternEvo-0.5.1/internlm/train/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,20 @@
     initialize_model,
     initialize_optimizer,
     initialize_parallel_communicator,
     load_new_batch,
     record_current_batch_training_metrics,
     set_fp32_attr_for_model,
     set_parallel_attr_for_param_groups,
-    wrap_FSDP_model,
 )
 
 __all__ = [
     "initialize_llm_profile",
     "initialize_model",
     "initialize_parallel_communicator",
     "initialize_optimizer",
     "load_new_batch",
     "record_current_batch_training_metrics",
-    "wrap_FSDP_model",
     "get_scheduler_hooks",
     "set_parallel_attr_for_param_groups",
     "set_fp32_attr_for_model",
 ]
```

### Comparing `InternEvo-0.5.0.dev20240510/internlm/train/pipeline.py` & `InternEvo-0.5.1/internlm/train/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
-import functools
 import math
 import time
 from typing import Callable, Iterable, List, Optional, Tuple, TypeVar, Union
 
 import torch
 from torch import nn
-from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
-from torch.distributed.fsdp.fully_sharded_data_parallel import (
-    BackwardPrefetch,
-    ShardingStrategy,
-)
-from torch.distributed.fsdp.wrap import transformer_auto_wrap_policy
 from torch.utils.data import DataLoader
 
 from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import (
     IS_REPLICA_ZERO_PARALLEL,
     IS_TENSOR_DATA_PARALLEL,
     IS_TENSOR_EXPERT_DATA_PARALLEL,
@@ -56,16 +49,14 @@
 from internlm.model.modules.linear import (
     ColumnParallelLinear,
     ParallelLinearWithCommExt,
     RewardModelLinear,
     RowParallelLinear,
     ScaleColumnParallelLinear,
 )
-from internlm.model.modules.mha import GQA, MHA
-from internlm.model.modules.mlp import FeedForward
 from internlm.model.modules.utils import is_moe_param
 from internlm.model.moe.megablock.mlp import (
     MegaBlockFeedForward,
     MegaBlockGroupedFeedForward,
 )
 from internlm.model.moe.moe import MoE
 from internlm.model.ops.norm import RMSNorm
@@ -219,52 +210,14 @@
     sync_model_replica_param_group(model)
 
     # Change random state mode to ParallelMode.DATA after model is built, guaranteeing the random
     # state in the same dp group are all the same.
     random_mode = ParallelMode.WEIGHT_DATA if is_using_isp() else ParallelMode.DATA
     set_mode(random_mode)
 
-    # if fsdp enabled, wrap the model
-    model = wrap_FSDP_model(model)
-
-    # TODO: add a checker to ensure model only use ours linear, expect fsdp.
-
-    return model
-
-
-def wrap_FSDP_model(model: Union[nn.Module, nn.ModuleList]):
-    if gpc.config.parallel.zero1.fsdp:
-
-        # set wrap_policy for fsdp wrap
-        transformer_wrap_policy = functools.partial(
-            transformer_auto_wrap_policy,
-            transformer_layer_cls={
-                Embedding1D,
-                MHA,
-                GQA,
-                RMSNorm,
-                FeedForward,
-                RewardModelLinear,
-                ScaleColumnParallelLinear,
-            },
-        )
-
-        # wrap the model
-        grp = gpc.get_group(ParallelMode.ZERO1)
-        model = FSDP(  # pylint: disable=unexpected-keyword-arg
-            module=model,
-            process_group=grp,
-            sharding_strategy=ShardingStrategy.FULL_SHARD,
-            auto_wrap_policy=transformer_wrap_policy,
-            forward_prefetch=True,
-            backward_prefetch=BackwardPrefetch.BACKWARD_PRE,
-            limit_all_gathers=True,
-            use_orig_params=True,
-        )
-
     return model
 
 
 _T = TypeVar("_T")
 
 
 def _submodule_filter(model: Union[nn.Module, nn.ModuleList], target_cls: Union[_T, Tuple[_T]]) -> Iterable[_T]:
```

### Comparing `InternEvo-0.5.0.dev20240510/internlm/train/utils.py` & `InternEvo-0.5.1/internlm/train/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/utils/common.py` & `InternEvo-0.5.1/internlm/utils/common.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/utils/gputest.py` & `InternEvo-0.5.1/internlm/utils/gputest.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/utils/logger.py` & `InternEvo-0.5.1/internlm/utils/logger.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/utils/megatron_timers.py` & `InternEvo-0.5.1/internlm/utils/megatron_timers.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/utils/parallel.py` & `InternEvo-0.5.1/internlm/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/utils/simple_memory_profiler.py` & `InternEvo-0.5.1/internlm/utils/simple_memory_profiler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/utils/storage_manager.py` & `InternEvo-0.5.1/internlm/utils/storage_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/utils/timeout.py` & `InternEvo-0.5.1/internlm/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/utils/utils.py` & `InternEvo-0.5.1/internlm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/internlm/utils/writer.py` & `InternEvo-0.5.1/internlm/utils/writer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/common_fixture.py` & `InternEvo-0.5.1/tests/common_fixture.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/test_core/test_pipeline.py` & `InternEvo-0.5.1/tests/test_core/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/test_core/utils.py` & `InternEvo-0.5.1/tests/test_core/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/test_training/7B_check_acc.py` & `InternEvo-0.5.1/tests/test_training/7B_check_acc.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/test_training/7B_check_init.py` & `InternEvo-0.5.1/tests/test_training/7B_check_init.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/test_training/test_forward_output_no_fa.py` & `InternEvo-0.5.1/tests/test_training/test_forward_output_no_fa.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/test_training/test_load_ckpt_loss.py` & `InternEvo-0.5.1/tests/test_training/test_load_ckpt_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/test_training/test_loss.py` & `InternEvo-0.5.1/tests/test_training/test_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/test_training/test_no_fa_train_temp.py` & `InternEvo-0.5.1/tests/test_training/test_no_fa_train_temp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/test_training/test_norm_weight.py` & `InternEvo-0.5.1/tests/test_training/test_norm_weight.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/test_training/test_swap_nb_loss_and_gradnorm.py` & `InternEvo-0.5.1/tests/test_training/test_swap_nb_loss_and_gradnorm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.0.dev20240510/tests/test_training/train_CI.py` & `InternEvo-0.5.1/tests/test_training/train_CI.py`

 * *Files identical despite different names*

