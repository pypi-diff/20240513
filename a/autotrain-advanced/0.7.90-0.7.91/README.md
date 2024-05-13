# Comparing `tmp/autotrain-advanced-0.7.90.tar.gz` & `tmp/autotrain-advanced-0.7.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.7.90.tar", last modified: Mon May 13 17:04:12 2024, max compression
+gzip compressed data, was "autotrain-advanced-0.7.91.tar", last modified: Mon May 13 17:19:16 2024, max compression
```

## Comparing `autotrain-advanced-0.7.90.tar` & `autotrain-advanced-0.7.91.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.187326 autotrain-advanced-0.7.90/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.90/LICENSE
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13287 2024-05-13 17:04:12.187326 autotrain-advanced-0.7.90/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2741 2024-05-04 09:15:32.000000 autotrain-advanced-0.7.90/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-13 17:04:12.187326 autotrain-advanced-0.7.90/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.90/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.163326 autotrain-advanced-0.7.90/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.167326 autotrain-advanced-0.7.90/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1450 2024-05-13 17:04:01.000000 autotrain-advanced-0.7.90/src/autotrain/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.167326 autotrain-advanced-0.7.90/src/autotrain/app/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.90/src/autotrain/app/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.90/src/autotrain/app/api_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-13 16:31:05.000000 autotrain-advanced-0.7.90/src/autotrain/app/app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.90/src/autotrain/app/db.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.90/src/autotrain/app/models.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.90/src/autotrain/app/oauth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    18596 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/app/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.167326 autotrain-advanced-0.7.90/src/autotrain/app/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.90/src/autotrain/app/static/logo.png
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.167326 autotrain-advanced-0.7.90/src/autotrain/app/templates/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.90/src/autotrain/app/templates/duplicate.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.90/src/autotrain/app/templates/error.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.90/src/autotrain/app/templates/index.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.90/src/autotrain/app/templates/login.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1594 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.90/src/autotrain/app/training_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17416 2024-05-13 16:38:01.000000 autotrain-advanced-0.7.90/src/autotrain/app/ui_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3220 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.90/src/autotrain/app/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.167326 autotrain-advanced-0.7.90/src/autotrain/backends/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.90/src/autotrain/backends/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/backends/base.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.90/src/autotrain/backends/endpoints.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.90/src/autotrain/backends/local.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.90/src/autotrain/backends/ngc.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.90/src/autotrain/backends/nvcf.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.90/src/autotrain/backends/spaces.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.167326 autotrain-advanced-0.7.90/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.90/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3668 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7711 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_object_detection.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9902 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_seq2seq.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_spacerunner.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7989 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7933 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_text_regression.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7910 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_token_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.90/src/autotrain/cli/run_tools.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/cli/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/commands.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.90/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.90/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.90/src/autotrain/logging.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6051 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.90/src/autotrain/parser.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.167326 autotrain-advanced-0.7.90/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.90/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.90/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.90/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.90/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.167326 autotrain-advanced-0.7.90/src/autotrain/tools/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.90/src/autotrain/tools/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.90/src/autotrain/tools/convert_to_kohya.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.90/src/autotrain/tools/merge_adapter.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.171326 autotrain-advanced-0.7.90/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.171326 autotrain-advanced-0.7.90/src/autotrain/trainers/clm/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/clm/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/clm/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/clm/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/clm/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/clm/train_clm_default.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/clm/train_clm_dpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/clm/train_clm_orpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/clm/train_clm_reward.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/clm/train_clm_sft.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20504 2024-05-09 12:46:57.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/clm/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8195 2024-05-06 12:50:40.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/common.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.171326 autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/train.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/train_xl.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.171326 autotrain-advanced-0.7.90/src/autotrain/trainers/generic/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/generic/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/generic/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/generic/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/generic/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.171326 autotrain-advanced-0.7.90/src/autotrain/trainers/image_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/image_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7406 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/image_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/image_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1824 2024-05-13 09:34:02.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/image_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/image_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.171326 autotrain-advanced-0.7.90/src/autotrain/trainers/object_detection/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/object_detection/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7094 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/object_detection/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/object_detection/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1982 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/object_detection/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7854 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/object_detection/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.171326 autotrain-advanced-0.7.90/src/autotrain/trainers/seq2seq/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/seq2seq/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8817 2024-04-29 09:01:25.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/seq2seq/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/seq2seq/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2424 2024-04-25 05:53:33.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/seq2seq/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/seq2seq/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.171326 autotrain-advanced-0.7.90/src/autotrain/trainers/tabular/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/tabular/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/tabular/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/tabular/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/tabular/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.171326 autotrain-advanced-0.7.90/src/autotrain/trainers/text_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/text_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7647 2024-04-25 05:44:56.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/text_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/text_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1876 2024-04-25 05:53:42.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/text_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/text_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.175326 autotrain-advanced-0.7.90/src/autotrain/trainers/text_regression/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/text_regression/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6928 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/text_regression/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/text_regression/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1875 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/text_regression/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2117 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/text_regression/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.175326 autotrain-advanced-0.7.90/src/autotrain/trainers/token_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/token_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7428 2024-04-25 05:44:07.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/token_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/token_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1877 2024-04-25 05:53:47.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/token_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1675 2024-04-25 05:15:09.000000 autotrain-advanced-0.7.90/src/autotrain/trainers/token_classification/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.90/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.175326 autotrain-advanced-0.7.90/src/autotrain_advanced.egg-info/
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13287 2024-05-13 17:04:12.000000 autotrain-advanced-0.7.90/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4885 2024-05-13 17:04:12.000000 autotrain-advanced-0.7.90/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-13 17:04:12.000000 autotrain-advanced-0.7.90/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-13 17:04:12.000000 autotrain-advanced-0.7.90/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3635 2024-05-13 17:04:12.000000 autotrain-advanced-0.7.90/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-13 17:04:12.000000 autotrain-advanced-0.7.90/src/autotrain_advanced.egg-info/top_level.txt
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:04:12.175326 autotrain-advanced-0.7.90/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.90/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.672819 autotrain-advanced-0.7.91/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.91/LICENSE
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13452 2024-05-13 17:19:16.672819 autotrain-advanced-0.7.91/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2741 2024-05-04 09:15:32.000000 autotrain-advanced-0.7.91/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-13 17:19:16.672819 autotrain-advanced-0.7.91/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.91/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.648820 autotrain-advanced-0.7.91/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.648820 autotrain-advanced-0.7.91/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1450 2024-05-13 17:19:06.000000 autotrain-advanced-0.7.91/src/autotrain/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.652819 autotrain-advanced-0.7.91/src/autotrain/app/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.91/src/autotrain/app/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.91/src/autotrain/app/api_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-13 16:31:05.000000 autotrain-advanced-0.7.91/src/autotrain/app/app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.91/src/autotrain/app/db.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.91/src/autotrain/app/models.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.91/src/autotrain/app/oauth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    18596 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/app/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.652819 autotrain-advanced-0.7.91/src/autotrain/app/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.91/src/autotrain/app/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.652819 autotrain-advanced-0.7.91/src/autotrain/app/templates/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.91/src/autotrain/app/templates/duplicate.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.91/src/autotrain/app/templates/error.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.91/src/autotrain/app/templates/index.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.91/src/autotrain/app/templates/login.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1594 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.91/src/autotrain/app/training_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17416 2024-05-13 16:38:01.000000 autotrain-advanced-0.7.91/src/autotrain/app/ui_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3220 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.91/src/autotrain/app/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.652819 autotrain-advanced-0.7.91/src/autotrain/backends/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.91/src/autotrain/backends/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/backends/base.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.91/src/autotrain/backends/endpoints.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.91/src/autotrain/backends/local.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.91/src/autotrain/backends/ngc.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.91/src/autotrain/backends/nvcf.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.91/src/autotrain/backends/spaces.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.652819 autotrain-advanced-0.7.91/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.91/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3668 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7711 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_object_detection.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9902 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_seq2seq.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_spacerunner.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7989 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7933 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_text_regression.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7910 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_token_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.91/src/autotrain/cli/run_tools.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/cli/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/commands.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.91/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.91/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.91/src/autotrain/logging.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6051 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.91/src/autotrain/parser.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.652819 autotrain-advanced-0.7.91/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.91/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.91/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.91/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.91/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.652819 autotrain-advanced-0.7.91/src/autotrain/tools/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.91/src/autotrain/tools/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.91/src/autotrain/tools/convert_to_kohya.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.91/src/autotrain/tools/merge_adapter.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.652819 autotrain-advanced-0.7.91/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.652819 autotrain-advanced-0.7.91/src/autotrain/trainers/clm/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/clm/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/clm/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/clm/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/clm/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/clm/train_clm_default.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/clm/train_clm_dpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/clm/train_clm_orpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/clm/train_clm_reward.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/clm/train_clm_sft.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20504 2024-05-09 12:46:57.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/clm/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8195 2024-05-06 12:50:40.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/common.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.656819 autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/train.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/train_xl.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.656819 autotrain-advanced-0.7.91/src/autotrain/trainers/generic/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/generic/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/generic/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/generic/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/generic/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.656819 autotrain-advanced-0.7.91/src/autotrain/trainers/image_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/image_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7406 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/image_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/image_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1824 2024-05-13 09:34:02.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/image_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/image_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.656819 autotrain-advanced-0.7.91/src/autotrain/trainers/object_detection/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/object_detection/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7094 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/object_detection/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/object_detection/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1982 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/object_detection/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7854 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/object_detection/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.656819 autotrain-advanced-0.7.91/src/autotrain/trainers/seq2seq/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/seq2seq/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8817 2024-04-29 09:01:25.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/seq2seq/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/seq2seq/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2424 2024-04-25 05:53:33.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/seq2seq/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/seq2seq/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.656819 autotrain-advanced-0.7.91/src/autotrain/trainers/tabular/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/tabular/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/tabular/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/tabular/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/tabular/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.656819 autotrain-advanced-0.7.91/src/autotrain/trainers/text_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/text_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7647 2024-04-25 05:44:56.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/text_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/text_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1876 2024-04-25 05:53:42.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/text_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/text_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.656819 autotrain-advanced-0.7.91/src/autotrain/trainers/text_regression/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/text_regression/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6928 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/text_regression/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/text_regression/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1875 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/text_regression/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2117 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/text_regression/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.656819 autotrain-advanced-0.7.91/src/autotrain/trainers/token_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/token_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7428 2024-04-25 05:44:07.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/token_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/token_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1877 2024-04-25 05:53:47.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/token_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1675 2024-04-25 05:15:09.000000 autotrain-advanced-0.7.91/src/autotrain/trainers/token_classification/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.91/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.656819 autotrain-advanced-0.7.91/src/autotrain_advanced.egg-info/
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13452 2024-05-13 17:19:16.000000 autotrain-advanced-0.7.91/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4885 2024-05-13 17:19:16.000000 autotrain-advanced-0.7.91/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-13 17:19:16.000000 autotrain-advanced-0.7.91/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-13 17:19:16.000000 autotrain-advanced-0.7.91/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3687 2024-05-13 17:19:16.000000 autotrain-advanced-0.7.91/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-13 17:19:16.000000 autotrain-advanced-0.7.91/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:19:16.656819 autotrain-advanced-0.7.91/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.91/static/logo.png
```

### Comparing `autotrain-advanced-0.7.90/LICENSE` & `autotrain-advanced-0.7.91/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/PKG-INFO` & `autotrain-advanced-0.7.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.90
+Version: 0.7.91
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
@@ -63,14 +63,15 @@
 Requires-Dist: hf-transfer
 Requires-Dist: pyngrok==7.1.6
 Requires-Dist: authlib==1.3.0
 Requires-Dist: itsdangerous==2.2.0
 Requires-Dist: seqeval==1.2.2
 Requires-Dist: httpx==0.27.0
 Requires-Dist: pyyaml==6.0.1
+Requires-Dist: timm==0.9.16
 Requires-Dist: torchmetrics==1.4.0
 Requires-Dist: pycocotools==2.0.7
 Provides-Extra: dev
 Requires-Dist: albumentations==1.4.4; extra == "dev"
 Requires-Dist: codecarbon==2.3.5; extra == "dev"
 Requires-Dist: datasets[vision]~=2.19.0; extra == "dev"
 Requires-Dist: evaluate==0.4.1; extra == "dev"
@@ -113,14 +114,15 @@
 Requires-Dist: hf-transfer; extra == "dev"
 Requires-Dist: pyngrok==7.1.6; extra == "dev"
 Requires-Dist: authlib==1.3.0; extra == "dev"
 Requires-Dist: itsdangerous==2.2.0; extra == "dev"
 Requires-Dist: seqeval==1.2.2; extra == "dev"
 Requires-Dist: httpx==0.27.0; extra == "dev"
 Requires-Dist: pyyaml==6.0.1; extra == "dev"
+Requires-Dist: timm==0.9.16; extra == "dev"
 Requires-Dist: torchmetrics==1.4.0; extra == "dev"
 Requires-Dist: pycocotools==2.0.7; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: flake8==3.7.9; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: quality
@@ -167,14 +169,15 @@
 Requires-Dist: hf-transfer; extra == "quality"
 Requires-Dist: pyngrok==7.1.6; extra == "quality"
 Requires-Dist: authlib==1.3.0; extra == "quality"
 Requires-Dist: itsdangerous==2.2.0; extra == "quality"
 Requires-Dist: seqeval==1.2.2; extra == "quality"
 Requires-Dist: httpx==0.27.0; extra == "quality"
 Requires-Dist: pyyaml==6.0.1; extra == "quality"
+Requires-Dist: timm==0.9.16; extra == "quality"
 Requires-Dist: torchmetrics==1.4.0; extra == "quality"
 Requires-Dist: pycocotools==2.0.7; extra == "quality"
 Requires-Dist: black; extra == "quality"
 Requires-Dist: isort; extra == "quality"
 Requires-Dist: flake8==3.7.9; extra == "quality"
 Provides-Extra: docs
 Requires-Dist: albumentations==1.4.4; extra == "docs"
@@ -220,14 +223,15 @@
 Requires-Dist: hf-transfer; extra == "docs"
 Requires-Dist: pyngrok==7.1.6; extra == "docs"
 Requires-Dist: authlib==1.3.0; extra == "docs"
 Requires-Dist: itsdangerous==2.2.0; extra == "docs"
 Requires-Dist: seqeval==1.2.2; extra == "docs"
 Requires-Dist: httpx==0.27.0; extra == "docs"
 Requires-Dist: pyyaml==6.0.1; extra == "docs"
+Requires-Dist: timm==0.9.16; extra == "docs"
 Requires-Dist: torchmetrics==1.4.0; extra == "docs"
 Requires-Dist: pycocotools==2.0.7; extra == "docs"
 Requires-Dist: recommonmark; extra == "docs"
 Requires-Dist: sphinx==3.1.2; extra == "docs"
 Requires-Dist: sphinx-markdown-tables; extra == "docs"
 Requires-Dist: sphinx-rtd-theme==0.4.3; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
```

### Comparing `autotrain-advanced-0.7.90/README.md` & `autotrain-advanced-0.7.91/README.md`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/setup.py` & `autotrain-advanced-0.7.91/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/__init__.py` & `autotrain-advanced-0.7.91/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 warnings.filterwarnings("ignore", category=UserWarning, module="peft")
 warnings.filterwarnings("ignore", category=UserWarning, module="accelerate")
 warnings.filterwarnings("ignore", category=UserWarning, module="datasets")
 warnings.filterwarnings("ignore", category=FutureWarning, module="accelerate")
 
 
 logger = Logger().get_logger()
-__version__ = "0.7.90"
+__version__ = "0.7.91"
```

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/api_routes.py` & `autotrain-advanced-0.7.91/src/autotrain/app/api_routes.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/app.py` & `autotrain-advanced-0.7.91/src/autotrain/app/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/db.py` & `autotrain-advanced-0.7.91/src/autotrain/app/db.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/models.py` & `autotrain-advanced-0.7.91/src/autotrain/app/models.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/oauth.py` & `autotrain-advanced-0.7.91/src/autotrain/app/oauth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/params.py` & `autotrain-advanced-0.7.91/src/autotrain/app/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/static/logo.png` & `autotrain-advanced-0.7.91/src/autotrain/app/static/logo.png`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/templates/duplicate.html` & `autotrain-advanced-0.7.91/src/autotrain/app/templates/duplicate.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/templates/error.html` & `autotrain-advanced-0.7.91/src/autotrain/app/templates/error.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/templates/index.html` & `autotrain-advanced-0.7.91/src/autotrain/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/templates/login.html` & `autotrain-advanced-0.7.91/src/autotrain/app/templates/login.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/training_api.py` & `autotrain-advanced-0.7.91/src/autotrain/app/training_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/ui_routes.py` & `autotrain-advanced-0.7.91/src/autotrain/app/ui_routes.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/app/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/app/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/backends/base.py` & `autotrain-advanced-0.7.91/src/autotrain/backends/base.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/backends/endpoints.py` & `autotrain-advanced-0.7.91/src/autotrain/backends/endpoints.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/backends/ngc.py` & `autotrain-advanced-0.7.91/src/autotrain/backends/ngc.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/backends/nvcf.py` & `autotrain-advanced-0.7.91/src/autotrain/backends/nvcf.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/backends/spaces.py` & `autotrain-advanced-0.7.91/src/autotrain/backends/spaces.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_api.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_image_classification.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_object_detection.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_object_detection.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_seq2seq.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_seq2seq.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_spacerunner.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_spacerunner.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_tabular.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_text_classification.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_text_regression.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_text_regression.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_token_classification.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_token_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/run_tools.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/run_tools.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/cli/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/cli/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/commands.py` & `autotrain-advanced-0.7.91/src/autotrain/commands.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/dataset.py` & `autotrain-advanced-0.7.91/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/help.py` & `autotrain-advanced-0.7.91/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/logging.py` & `autotrain-advanced-0.7.91/src/autotrain/logging.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/parser.py` & `autotrain-advanced-0.7.91/src/autotrain/parser.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.7.91/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.7.91/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.7.91/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.7.91/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/project.py` & `autotrain-advanced-0.7.91/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/tasks.py` & `autotrain-advanced-0.7.91/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/tools/convert_to_kohya.py` & `autotrain-advanced-0.7.91/src/autotrain/tools/convert_to_kohya.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/tools/merge_adapter.py` & `autotrain-advanced-0.7.91/src/autotrain/tools/merge_adapter.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/clm/__main__.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/clm/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/clm/callbacks.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/clm/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/clm/params.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/clm/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/clm/train_clm_default.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/clm/train_clm_default.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/clm/train_clm_dpo.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/clm/train_clm_dpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/clm/train_clm_orpo.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/clm/train_clm_orpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/clm/train_clm_reward.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/clm/train_clm_reward.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/clm/train_clm_sft.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/clm/train_clm_sft.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/clm/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/clm/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/common.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/common.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/__main__.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/train.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/train.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/train_xl.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/train_xl.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/dreambooth/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/generic/__main__.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/generic/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/generic/params.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/generic/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/generic/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/generic/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/image_classification/__main__.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/image_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/image_classification/dataset.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/image_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/image_classification/params.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/image_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/image_classification/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/image_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/object_detection/__main__.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/object_detection/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/object_detection/dataset.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/object_detection/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/object_detection/params.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/object_detection/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/object_detection/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/seq2seq/__main__.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/seq2seq/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/seq2seq/dataset.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/seq2seq/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/seq2seq/params.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/seq2seq/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/seq2seq/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/seq2seq/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/tabular/__main__.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/tabular/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/tabular/params.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/tabular/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/tabular/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/text_classification/__main__.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/text_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/text_classification/dataset.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/text_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/text_classification/params.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/text_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/text_classification/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/text_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/text_regression/__main__.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/text_regression/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/text_regression/dataset.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/text_regression/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/text_regression/params.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/text_regression/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/text_regression/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/text_regression/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/token_classification/__main__.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/token_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/token_classification/dataset.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/token_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/token_classification/params.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/token_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/trainers/token_classification/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/trainers/token_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain/utils.py` & `autotrain-advanced-0.7.91/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.7.91/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.90
+Version: 0.7.91
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
@@ -63,14 +63,15 @@
 Requires-Dist: hf-transfer
 Requires-Dist: pyngrok==7.1.6
 Requires-Dist: authlib==1.3.0
 Requires-Dist: itsdangerous==2.2.0
 Requires-Dist: seqeval==1.2.2
 Requires-Dist: httpx==0.27.0
 Requires-Dist: pyyaml==6.0.1
+Requires-Dist: timm==0.9.16
 Requires-Dist: torchmetrics==1.4.0
 Requires-Dist: pycocotools==2.0.7
 Provides-Extra: dev
 Requires-Dist: albumentations==1.4.4; extra == "dev"
 Requires-Dist: codecarbon==2.3.5; extra == "dev"
 Requires-Dist: datasets[vision]~=2.19.0; extra == "dev"
 Requires-Dist: evaluate==0.4.1; extra == "dev"
@@ -113,14 +114,15 @@
 Requires-Dist: hf-transfer; extra == "dev"
 Requires-Dist: pyngrok==7.1.6; extra == "dev"
 Requires-Dist: authlib==1.3.0; extra == "dev"
 Requires-Dist: itsdangerous==2.2.0; extra == "dev"
 Requires-Dist: seqeval==1.2.2; extra == "dev"
 Requires-Dist: httpx==0.27.0; extra == "dev"
 Requires-Dist: pyyaml==6.0.1; extra == "dev"
+Requires-Dist: timm==0.9.16; extra == "dev"
 Requires-Dist: torchmetrics==1.4.0; extra == "dev"
 Requires-Dist: pycocotools==2.0.7; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: flake8==3.7.9; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: quality
@@ -167,14 +169,15 @@
 Requires-Dist: hf-transfer; extra == "quality"
 Requires-Dist: pyngrok==7.1.6; extra == "quality"
 Requires-Dist: authlib==1.3.0; extra == "quality"
 Requires-Dist: itsdangerous==2.2.0; extra == "quality"
 Requires-Dist: seqeval==1.2.2; extra == "quality"
 Requires-Dist: httpx==0.27.0; extra == "quality"
 Requires-Dist: pyyaml==6.0.1; extra == "quality"
+Requires-Dist: timm==0.9.16; extra == "quality"
 Requires-Dist: torchmetrics==1.4.0; extra == "quality"
 Requires-Dist: pycocotools==2.0.7; extra == "quality"
 Requires-Dist: black; extra == "quality"
 Requires-Dist: isort; extra == "quality"
 Requires-Dist: flake8==3.7.9; extra == "quality"
 Provides-Extra: docs
 Requires-Dist: albumentations==1.4.4; extra == "docs"
@@ -220,14 +223,15 @@
 Requires-Dist: hf-transfer; extra == "docs"
 Requires-Dist: pyngrok==7.1.6; extra == "docs"
 Requires-Dist: authlib==1.3.0; extra == "docs"
 Requires-Dist: itsdangerous==2.2.0; extra == "docs"
 Requires-Dist: seqeval==1.2.2; extra == "docs"
 Requires-Dist: httpx==0.27.0; extra == "docs"
 Requires-Dist: pyyaml==6.0.1; extra == "docs"
+Requires-Dist: timm==0.9.16; extra == "docs"
 Requires-Dist: torchmetrics==1.4.0; extra == "docs"
 Requires-Dist: pycocotools==2.0.7; extra == "docs"
 Requires-Dist: recommonmark; extra == "docs"
 Requires-Dist: sphinx==3.1.2; extra == "docs"
 Requires-Dist: sphinx-markdown-tables; extra == "docs"
 Requires-Dist: sphinx-rtd-theme==0.4.3; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
```

### Comparing `autotrain-advanced-0.7.90/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.7.91/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.90/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.7.91/src/autotrain_advanced.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 hf-transfer
 pyngrok==7.1.6
 authlib==1.3.0
 itsdangerous==2.2.0
 seqeval==1.2.2
 httpx==0.27.0
 pyyaml==6.0.1
+timm==0.9.16
 torchmetrics==1.4.0
 pycocotools==2.0.7
 
 [:sys_platform == "linux"]
 bitsandbytes==0.43.1
 
 [dev]
@@ -93,14 +94,15 @@
 hf-transfer
 pyngrok==7.1.6
 authlib==1.3.0
 itsdangerous==2.2.0
 seqeval==1.2.2
 httpx==0.27.0
 pyyaml==6.0.1
+timm==0.9.16
 torchmetrics==1.4.0
 pycocotools==2.0.7
 black
 isort
 flake8==3.7.9
 pytest
 
@@ -150,14 +152,15 @@
 hf-transfer
 pyngrok==7.1.6
 authlib==1.3.0
 itsdangerous==2.2.0
 seqeval==1.2.2
 httpx==0.27.0
 pyyaml==6.0.1
+timm==0.9.16
 torchmetrics==1.4.0
 pycocotools==2.0.7
 recommonmark
 sphinx==3.1.2
 sphinx-markdown-tables
 sphinx-rtd-theme==0.4.3
 sphinx-copybutton
@@ -208,14 +211,15 @@
 hf-transfer
 pyngrok==7.1.6
 authlib==1.3.0
 itsdangerous==2.2.0
 seqeval==1.2.2
 httpx==0.27.0
 pyyaml==6.0.1
+timm==0.9.16
 torchmetrics==1.4.0
 pycocotools==2.0.7
 black
 isort
 flake8==3.7.9
 
 [quality:sys_platform == "linux"]
```

### Comparing `autotrain-advanced-0.7.90/static/logo.png` & `autotrain-advanced-0.7.91/static/logo.png`

 * *Files identical despite different names*

