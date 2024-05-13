# Comparing `tmp/ontrac-0.0.6.post2.tar.gz` & `tmp/ontrac-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontrac-0.0.6.post2.tar", last modified: Tue May  7 18:27:55 2024, max compression
+gzip compressed data, was "ontrac-0.0.7.tar", last modified: Mon May 13 18:31:47 2024, max compression
```

## Comparing `ontrac-0.0.6.post2.tar` & `ontrac-0.0.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.543236 ontrac-0.0.6.post2/
--rw-r--r--   0 wwang      (501) staff       (20)     1116 2024-04-25 17:21:18.000000 ontrac-0.0.6.post2/LICENSE
--rw-r--r--   0 wwang      (501) staff       (20)       60 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/MANIFEST.in
--rw-r--r--   0 wwang      (501) staff       (20)     7220 2024-05-07 18:27:55.543019 ontrac-0.0.6.post2/PKG-INFO
--rw-r--r--   0 wwang      (501) staff       (20)     5930 2024-04-25 17:24:03.000000 ontrac-0.0.6.post2/README.md
--rw-r--r--   0 wwang      (501) staff       (20)     1754 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/pyproject.toml
--rw-r--r--   0 wwang      (501) staff       (20)       38 2024-05-07 18:27:55.543277 ontrac-0.0.6.post2/setup.cfg
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.532613 ontrac-0.0.6.post2/src/
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.534646 ontrac-0.0.6.post2/src/ONTraC/
--rw-r--r--   0 wwang      (501) staff       (20)       32 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/__init__.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.537239 ontrac-0.0.6.post2/src/ONTraC/analysis/
--rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)    10263 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/cell_type.py
--rw-r--r--   0 wwang      (501) staff       (20)      114 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/constants.py
--rw-r--r--   0 wwang      (501) staff       (20)    13983 2024-05-06 02:05:26.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/data.py
--rw-r--r--   0 wwang      (501) staff       (20)     2695 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/meta_info.py
--rw-r--r--   0 wwang      (501) staff       (20)    15098 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/niche_cluster.py
--rw-r--r--   0 wwang      (501) staff       (20)    11483 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/spatial.py
--rw-r--r--   0 wwang      (501) staff       (20)     1284 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/train_loss.py
--rw-r--r--   0 wwang      (501) staff       (20)      915 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/analysis/utils.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.538202 ontrac-0.0.6.post2/src/ONTraC/bin/
--rw-r--r--   0 wwang      (501) staff       (20)     3720 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/bin/GP.py
--rw-r--r--   0 wwang      (501) staff       (20)     1516 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/bin/NTScore.py
--rw-r--r--   0 wwang      (501) staff       (20)     4003 2024-05-07 17:42:25.000000 ontrac-0.0.6.post2/src/ONTraC/bin/ONTraC.py
--rwxr-xr-x   0 wwang      (501) staff       (20)     3755 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/bin/ONTraC_analysis.py
--rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/bin/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)     1244 2024-05-07 17:42:25.000000 ontrac-0.0.6.post2/src/ONTraC/bin/createDataSet.py
--rw-r--r--   0 wwang      (501) staff       (20)     3725 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/data.py
--rw-r--r--   0 wwang      (501) staff       (20)      884 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/log.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.538963 ontrac-0.0.6.post2/src/ONTraC/model/
--rw-r--r--   0 wwang      (501) staff       (20)       21 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/model/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)     6500 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/model/_model.py
--rw-r--r--   0 wwang      (501) staff       (20)     6517 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/model/dmon_exp_pool.py
--rw-r--r--   0 wwang      (501) staff       (20)     3133 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/model/norm_dense_gcn_conv.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.540206 ontrac-0.0.6.post2/src/ONTraC/optparser/
--rw-r--r--   0 wwang      (501) staff       (20)     2232 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_GP.py
--rw-r--r--   0 wwang      (501) staff       (20)     4521 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_IO.py
--rw-r--r--   0 wwang      (501) staff       (20)     1489 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_NT.py
--rw-r--r--   0 wwang      (501) staff       (20)     3198 2024-05-07 17:42:25.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_ONTraC.py
--rw-r--r--   0 wwang      (501) staff       (20)      260 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)     2899 2024-05-07 17:42:25.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_create_dataset.py
--rw-r--r--   0 wwang      (501) staff       (20)     7020 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/optparser/_train.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.540531 ontrac-0.0.6.post2/src/ONTraC/run/
--rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/run/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)    10506 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/run/processes.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.541417 ontrac-0.0.6.post2/src/ONTraC/train/
--rw-r--r--   0 wwang      (501) staff       (20)       28 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/train/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)     9452 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/train/_batch_train.py
--rw-r--r--   0 wwang      (501) staff       (20)     5974 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/train/inspect_funcs.py
--rw-r--r--   0 wwang      (501) staff       (20)     4601 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/train/loss_funs.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.542397 ontrac-0.0.6.post2/src/ONTraC/utils/
--rw-r--r--   0 wwang      (501) staff       (20)     4993 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/utils/NTScore.py
--rw-r--r--   0 wwang      (501) staff       (20)       21 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/utils/__init__.py
--rw-r--r--   0 wwang      (501) staff       (20)     3049 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/utils/_utils.py
--rw-r--r--   0 wwang      (501) staff       (20)     3219 2024-05-06 01:06:13.000000 ontrac-0.0.6.post2/src/ONTraC/utils/decorators.py
--rw-r--r--   0 wwang      (501) staff       (20)     7673 2024-05-07 18:24:02.000000 ontrac-0.0.6.post2/src/ONTraC/utils/niche_net_constr.py
--rw-r--r--   0 wwang      (501) staff       (20)       27 2024-05-07 18:24:24.000000 ontrac-0.0.6.post2/src/ONTraC/version.py
-drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-07 18:27:55.542667 ontrac-0.0.6.post2/src/ONTraC.egg-info/
--rw-r--r--   0 wwang      (501) staff       (20)     7220 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/PKG-INFO
--rw-r--r--   0 wwang      (501) staff       (20)     1470 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/SOURCES.txt
--rw-r--r--   0 wwang      (501) staff       (20)        1 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/dependency_links.txt
--rw-r--r--   0 wwang      (501) staff       (20)      204 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/entry_points.txt
--rw-r--r--   0 wwang      (501) staff       (20)       95 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/requires.txt
--rw-r--r--   0 wwang      (501) staff       (20)        7 2024-05-07 18:27:55.000000 ontrac-0.0.6.post2/src/ONTraC.egg-info/top_level.txt
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-13 18:31:47.395492 ontrac-0.0.7/
+-rw-r--r--   0 wwang      (501) staff       (20)     1116 2024-05-09 20:41:20.000000 ontrac-0.0.7/LICENSE
+-rw-r--r--   0 wwang      (501) staff       (20)       60 2024-05-09 20:41:20.000000 ontrac-0.0.7/MANIFEST.in
+-rw-r--r--   0 wwang      (501) staff       (20)     8024 2024-05-13 18:31:47.395255 ontrac-0.0.7/PKG-INFO
+-rw-r--r--   0 wwang      (501) staff       (20)     6727 2024-05-13 17:55:47.000000 ontrac-0.0.7/README.md
+-rw-r--r--   0 wwang      (501) staff       (20)     1767 2024-05-13 18:31:31.000000 ontrac-0.0.7/pyproject.toml
+-rw-r--r--   0 wwang      (501) staff       (20)       38 2024-05-13 18:31:47.395537 ontrac-0.0.7/setup.cfg
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-13 18:31:47.382298 ontrac-0.0.7/src/
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-13 18:31:47.384283 ontrac-0.0.7/src/ONTraC/
+-rw-r--r--   0 wwang      (501) staff       (20)       32 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/__init__.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-13 18:31:47.387884 ontrac-0.0.7/src/ONTraC/analysis/
+-rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/analysis/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)    10232 2024-05-13 14:41:44.000000 ontrac-0.0.7/src/ONTraC/analysis/cell_type.py
+-rw-r--r--   0 wwang      (501) staff       (20)      114 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/analysis/constants.py
+-rw-r--r--   0 wwang      (501) staff       (20)    13983 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/analysis/data.py
+-rw-r--r--   0 wwang      (501) staff       (20)     2695 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/analysis/meta_info.py
+-rw-r--r--   0 wwang      (501) staff       (20)    15098 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/analysis/niche_cluster.py
+-rw-r--r--   0 wwang      (501) staff       (20)    11483 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/analysis/spatial.py
+-rw-r--r--   0 wwang      (501) staff       (20)     1284 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/analysis/train_loss.py
+-rw-r--r--   0 wwang      (501) staff       (20)      915 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/analysis/utils.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-13 18:31:47.389370 ontrac-0.0.7/src/ONTraC/bin/
+-rw-r--r--   0 wwang      (501) staff       (20)     3917 2024-05-13 14:45:28.000000 ontrac-0.0.7/src/ONTraC/bin/GP.py
+-rw-r--r--   0 wwang      (501) staff       (20)     1653 2024-05-13 14:45:28.000000 ontrac-0.0.7/src/ONTraC/bin/NTScore.py
+-rw-r--r--   0 wwang      (501) staff       (20)     4334 2024-05-13 14:45:28.000000 ontrac-0.0.7/src/ONTraC/bin/ONTraC.py
+-rwxr-xr-x   0 wwang      (501) staff       (20)     3755 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/bin/ONTraC_analysis.py
+-rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/bin/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)     1244 2024-05-13 14:36:06.000000 ontrac-0.0.7/src/ONTraC/bin/createDataSet.py
+-rw-r--r--   0 wwang      (501) staff       (20)     3366 2024-05-13 14:45:28.000000 ontrac-0.0.7/src/ONTraC/data.py
+-rw-r--r--   0 wwang      (501) staff       (20)      884 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/log.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-13 18:31:47.390310 ontrac-0.0.7/src/ONTraC/model/
+-rw-r--r--   0 wwang      (501) staff       (20)       21 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/model/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)     6500 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/model/_model.py
+-rw-r--r--   0 wwang      (501) staff       (20)     6517 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/model/dmon_exp_pool.py
+-rw-r--r--   0 wwang      (501) staff       (20)     3133 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/model/norm_dense_gcn_conv.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-13 18:31:47.391546 ontrac-0.0.7/src/ONTraC/optparser/
+-rw-r--r--   0 wwang      (501) staff       (20)     2232 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/optparser/_GP.py
+-rw-r--r--   0 wwang      (501) staff       (20)     4521 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/optparser/_IO.py
+-rw-r--r--   0 wwang      (501) staff       (20)     1489 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/optparser/_NT.py
+-rw-r--r--   0 wwang      (501) staff       (20)     3198 2024-05-13 14:36:06.000000 ontrac-0.0.7/src/ONTraC/optparser/_ONTraC.py
+-rw-r--r--   0 wwang      (501) staff       (20)      260 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/optparser/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)     2899 2024-05-13 14:36:06.000000 ontrac-0.0.7/src/ONTraC/optparser/_create_dataset.py
+-rw-r--r--   0 wwang      (501) staff       (20)     7406 2024-05-13 17:30:39.000000 ontrac-0.0.7/src/ONTraC/optparser/_train.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-13 18:31:47.391922 ontrac-0.0.7/src/ONTraC/run/
+-rw-r--r--   0 wwang      (501) staff       (20)        0 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/run/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)    10774 2024-05-13 14:45:28.000000 ontrac-0.0.7/src/ONTraC/run/processes.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-13 18:31:47.392769 ontrac-0.0.7/src/ONTraC/train/
+-rw-r--r--   0 wwang      (501) staff       (20)       28 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/train/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)     9452 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/train/_batch_train.py
+-rw-r--r--   0 wwang      (501) staff       (20)     5974 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/train/inspect_funcs.py
+-rw-r--r--   0 wwang      (501) staff       (20)     4601 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/train/loss_funs.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-13 18:31:47.393613 ontrac-0.0.7/src/ONTraC/utils/
+-rw-r--r--   0 wwang      (501) staff       (20)     5330 2024-05-13 14:45:28.000000 ontrac-0.0.7/src/ONTraC/utils/NTScore.py
+-rw-r--r--   0 wwang      (501) staff       (20)       21 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/utils/__init__.py
+-rw-r--r--   0 wwang      (501) staff       (20)     2529 2024-05-13 14:45:28.000000 ontrac-0.0.7/src/ONTraC/utils/_utils.py
+-rw-r--r--   0 wwang      (501) staff       (20)     3219 2024-05-09 20:41:20.000000 ontrac-0.0.7/src/ONTraC/utils/decorators.py
+-rw-r--r--   0 wwang      (501) staff       (20)     7820 2024-05-13 14:45:28.000000 ontrac-0.0.7/src/ONTraC/utils/niche_net_constr.py
+-rw-r--r--   0 wwang      (501) staff       (20)       22 2024-05-13 18:25:48.000000 ontrac-0.0.7/src/ONTraC/version.py
+drwxr-xr-x   0 wwang      (501) staff       (20)        0 2024-05-13 18:31:47.394822 ontrac-0.0.7/src/ONTraC.egg-info/
+-rw-r--r--   0 wwang      (501) staff       (20)     8024 2024-05-13 18:31:47.000000 ontrac-0.0.7/src/ONTraC.egg-info/PKG-INFO
+-rw-r--r--   0 wwang      (501) staff       (20)     1470 2024-05-13 18:31:47.000000 ontrac-0.0.7/src/ONTraC.egg-info/SOURCES.txt
+-rw-r--r--   0 wwang      (501) staff       (20)        1 2024-05-13 18:31:47.000000 ontrac-0.0.7/src/ONTraC.egg-info/dependency_links.txt
+-rw-r--r--   0 wwang      (501) staff       (20)      204 2024-05-13 18:31:47.000000 ontrac-0.0.7/src/ONTraC.egg-info/entry_points.txt
+-rw-r--r--   0 wwang      (501) staff       (20)       95 2024-05-13 18:31:47.000000 ontrac-0.0.7/src/ONTraC.egg-info/requires.txt
+-rw-r--r--   0 wwang      (501) staff       (20)        7 2024-05-13 18:31:47.000000 ontrac-0.0.7/src/ONTraC.egg-info/top_level.txt
```

### Comparing `ontrac-0.0.6.post2/LICENSE` & `ontrac-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/PKG-INFO` & `ontrac-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ONTraC
-Version: 0.0.6.post2
+Version: 0.0.7
 Summary: A niche-centered, machine learning method for constructing spatially continuous trajectories
 Author-email: Wen Wang <wwang.bio@gmail.com>, Shiwei Zheng <swzheng29@gmail.com>, Crystal Shin <sjcshin5040@gmail.com>, Guo-Cheng Yuan <gcyuan@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gyuanlab/ONTraC
 Project-URL: Repository, https://github.com/gyuanlab/ONTraC
 Project-URL: Issue Tracker, https://github.com/gyuanlab/ONTraC/issues
 Keywords: deep-learning,pytorch,pytorch geometric,trajectory inference,spatial omics
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: ==3.11.*
@@ -24,14 +24,20 @@
 Requires-Dist: torch-geometric==2.5.0
 Provides-Extra: analysis
 Requires-Dist: matplotlib; extra == "analysis"
 Requires-Dist: seaborn; extra == "analysis"
 
 # **ONTraC**
 
+[![PyPI Latest Release](https://img.shields.io/pypi/v/ONTraC.svg)](https://pypi.org/project/ONTraC/)
+[![Downloads](https://static.pepy.tech/badge/ONTraC)](https://pepy.tech/project/ONTraC)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/ONTraC.svg?label=PyPI%20downloads)](https://pypi.org/project/ONTraC/)
+[![GitHub stars](https://badgen.net/github/stars/gyuanlab/ONTraC)](https://github.com/gyuanlab/ONTraC)
+[![GitHub license](https://img.shields.io/github/license/gyuanlab/ONTraC.svg)](https://github.com/gyuanlab/ONTraC/blob/master/LICENSE)
+
 ONTraC (Ordered Niche Trajectory Construction) is a niche-centered, machine learning
 method for constructing spatially continuous trajectories. ONTraC differs from existing tools in
 that it treats a niche, rather than an individual cell, as the basic unit for spatial trajectory
 analysis. In this context, we define niche as a multicellular, spatially localized region where
 different cell types may coexist and interact with each other.  ONTraC seamlessly integrates
 cell-type composition and spatial information by using the graph neural network modeling
 framework. Its output, which is called the niche trajectory, can be viewed as a one dimensional
@@ -154,7 +160,9 @@
 The intermediate and final results are located in `preprocessing-dir`, `GNN-dir`, and `NTScore-dir` directories. Please see [IO files explanation](tutorials/IO_files.md#output-files) for detailed infromation.
 
 ### Visualization
 
 Please see [post analysis tutorial](tutorials/post_analysis.md).
 
 ## Citation
+
+**Wang, W.\*, Zheng, S.\*, Shin, C. S. & Yuan, G. C.$**. [Characterizing Spatially Continuous Variations in Tissue Microenvironment through Niche Trajectory Analysis]((https://www.biorxiv.org/content/10.1101/2024.04.23.590827v1)). *bioRxiv*, 2024.
```

### Comparing `ontrac-0.0.6.post2/README.md` & `ontrac-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # **ONTraC**
 
+[![PyPI Latest Release](https://img.shields.io/pypi/v/ONTraC.svg)](https://pypi.org/project/ONTraC/)
+[![Downloads](https://static.pepy.tech/badge/ONTraC)](https://pepy.tech/project/ONTraC)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/ONTraC.svg?label=PyPI%20downloads)](https://pypi.org/project/ONTraC/)
+[![GitHub stars](https://badgen.net/github/stars/gyuanlab/ONTraC)](https://github.com/gyuanlab/ONTraC)
+[![GitHub license](https://img.shields.io/github/license/gyuanlab/ONTraC.svg)](https://github.com/gyuanlab/ONTraC/blob/master/LICENSE)
+
 ONTraC (Ordered Niche Trajectory Construction) is a niche-centered, machine learning
 method for constructing spatially continuous trajectories. ONTraC differs from existing tools in
 that it treats a niche, rather than an individual cell, as the basic unit for spatial trajectory
 analysis. In this context, we define niche as a multicellular, spatially localized region where
 different cell types may coexist and interact with each other.  ONTraC seamlessly integrates
 cell-type composition and spatial information by using the graph neural network modeling
 framework. Its output, which is called the niche trajectory, can be viewed as a one dimensional
@@ -126,7 +132,9 @@
 The intermediate and final results are located in `preprocessing-dir`, `GNN-dir`, and `NTScore-dir` directories. Please see [IO files explanation](tutorials/IO_files.md#output-files) for detailed infromation.
 
 ### Visualization
 
 Please see [post analysis tutorial](tutorials/post_analysis.md).
 
 ## Citation
+
+**Wang, W.\*, Zheng, S.\*, Shin, C. S. & Yuan, G. C.$**. [Characterizing Spatially Continuous Variations in Tissue Microenvironment through Niche Trajectory Analysis]((https://www.biorxiv.org/content/10.1101/2024.04.23.590827v1)). *bioRxiv*, 2024.
```

### Comparing `ontrac-0.0.6.post2/pyproject.toml` & `ontrac-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
           ]
 description = "A niche-centered, machine learning method for constructing spatially continuous trajectories"
 readme = "README.md"
 requires-python = "==3.11.*"
 keywords = ["deep-learning", "pytorch", "pytorch geometric", "trajectory inference", "spatial omics"]
 license = {text = "MIT"}
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC/analysis/cell_type.py` & `ontrac-0.0.7/src/ONTraC/analysis/cell_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,18 +143,17 @@
     cell_type_dis_melt_df = pd.melt(
         data_df,
         id_vars='cluster',  # type: ignore
         var_name='Cell type',
         value_vars=cell_type,  # type: ignore
         value_name='Number')
     # g = sns.catplot(cell_type_dis_melt_df, kind="bar", x="Number", y="Cell type", col="cluster", col_order= nc_order, height=4,
-    g = sns.catplot(cell_type_dis_melt_df, kind="bar", x="Number", y="Cell type", col="cluster", height=4,
+    g = sns.catplot(cell_type_dis_melt_df, kind="bar", x="Number", y="Cell type", col="cluster", height=2 + len(cell_type) / 6,
                     aspect=.5)  # type: ignore
     g.add_legend()
-    g.figure.figsize = (2 + len(cell_type) / 3, 20)
     g.tight_layout()
     g.set_xticklabels(rotation='vertical')
     if ana_data.options.output is not None:
         g.savefig(f'{ana_data.options.output}/cell_type_loading_in_niche_clusters.pdf', transparent=True)
         return None
     else:
         return g
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC/analysis/data.py` & `ontrac-0.0.7/src/ONTraC/analysis/data.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/analysis/meta_info.py` & `ontrac-0.0.7/src/ONTraC/analysis/meta_info.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/analysis/niche_cluster.py` & `ontrac-0.0.7/src/ONTraC/analysis/niche_cluster.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/analysis/spatial.py` & `ontrac-0.0.7/src/ONTraC/analysis/spatial.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/analysis/train_loss.py` & `ontrac-0.0.7/src/ONTraC/analysis/train_loss.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/analysis/utils.py` & `ontrac-0.0.7/src/ONTraC/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/bin/GP.py` & `ontrac-0.0.7/src/ONTraC/bin/GP.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import torch
 
 from ..model import GraphPooling
 from ..optparser import opt_GP_validate, prepare_GP_optparser
 from ..run.processes import *
 from ..train import GPBatchTrain, SubBatchTrainProtocol
 from ..train.inspect_funcs import loss_record
-from ..utils import device_validate, write_version_info
+from ..utils import write_version_info
 from ..utils.niche_net_constr import load_original_data
 
 # ------------------------------------
 # Classes
 # ------------------------------------
 
 
@@ -43,30 +43,29 @@
 
     # write version information
     write_version_info()
 
     # ----- prepare -----
     # load parameters
     options = load_parameters(opt_validate_func=opt_GP_validate, prepare_optparser_func=prepare_GP_optparser)
-    # device
-    device: torch.device = device_validate(device_name=options.device)
     # load data
+    info('------------------------ GNN ------------------------ ')
     dataset, sample_loader = load_data(options=options)
     # random seed
     n_seed = t_seed = r_seed = options.seed
     random.seed(a=r_seed)
     torch.manual_seed(seed=t_seed)
     np.random.seed(seed=n_seed)
 
     # ----- train -----
     inspect_funcs_list = get_inspect_funcs()
     batch_train: SubBatchTrainProtocol = train(nn_model=GraphPooling,
                                                options=options,
                                                BatchTrain=GPBatchTrain,
-                                               device=device,
+                                               device=torch.device(options.device),
                                                dataset=dataset,
                                                sample_loader=sample_loader,
                                                inspect_funcs=inspect_funcs_list,
                                                model_name='GraphPooling')
 
     # --- evaluate ---
     evaluate(batch_train=batch_train, model_name='GraphPooling')
@@ -82,21 +81,24 @@
         ori_data_df = load_original_data(options=options)
         graph_pooling_output(ori_data_df=ori_data_df,
                              dataset=dataset,
                              rel_params=get_rel_params(
                                  options=options, params=read_yaml_file(f'{options.preprocessing_dir}/samples.yaml')),
                              consolidate_s_array=consolidate_s_array,
                              output_dir=options.GNN_dir)
+    info('---------------------- GNN end ---------------------- ')
 
     # ----- NT score -----
     if consolidate_s_array is not None and consolidate_out_adj_array is not None:
+        info('----------------- Niche trajectory ------------------ ')
         NTScore(options=options,
                 dataset=dataset,
                 consolidate_s_array=consolidate_s_array,
                 consolidate_out_adj_array=consolidate_out_adj_array)
+        info('--------------- Niche trajectory end ---------------- ')
 
 
 # ------------------------------------
 # Program running
 # ------------------------------------
 if __name__ == '__main__':
     try:
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC/bin/NTScore.py` & `ontrac-0.0.7/src/ONTraC/bin/NTScore.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,25 +22,27 @@
     # write version information
     write_version_info()
 
     # ----- prepare -----
     # --- load parameters ---
     options = load_parameters(opt_validate_func=opt_NT_validate, prepare_optparser_func=prepare_NT_optparser)
     # --- load data ---
-    dataset, _ = load_dataset(options=options)
+    dataset = load_dataset(options=options)
     # load consolidated s_array and out_adj_array
     consolidate_s_array = np.loadtxt(fname=f'{options.GNN_dir}/consolidate_s.csv.gz', delimiter=',')
     consolidate_out_adj_array = np.loadtxt(fname=f'{options.GNN_dir}/consolidate_out_adj.csv.gz', delimiter=',')
 
-    # ----- Pseudotime -----
+    # ----- NT score -----
     if consolidate_s_array is not None and consolidate_out_adj_array is not None:
+        info('----------------- Niche trajectory ------------------ ')
         NTScore(options=options,
                 dataset=dataset,
                 consolidate_s_array=consolidate_s_array,
                 consolidate_out_adj_array=consolidate_out_adj_array)
+        info('--------------- Niche trajectory end ---------------- ')
 
 
 # ------------------------------------
 # Program running
 # ------------------------------------
 if __name__ == '__main__':
     try:
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC/bin/ONTraC.py` & `ontrac-0.0.7/src/ONTraC/bin/ONTraC.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from ..log import *
 from ..model import GraphPooling
 from ..optparser import opt_ontrac_validate, prepare_ontrac_optparser
 from ..run.processes import *
 from ..train import GPBatchTrain, SubBatchTrainProtocol
 from ..train.inspect_funcs import loss_record
-from ..utils import device_validate, write_version_info
+from ..utils import write_version_info
 from ..utils.niche_net_constr import construct_niche_network, gen_samples_yaml, load_original_data
 
 
 # ------------------------------------
 # Functions
 # ------------------------------------
 def get_inspect_funcs() -> Optional[list[Callable]]:
@@ -42,39 +42,40 @@
     # write version information
     write_version_info()
 
     # prepare options
     options = load_parameters(opt_validate_func=opt_ontrac_validate, prepare_optparser_func=prepare_ontrac_optparser)
 
     # ----- Niche Network Construct -----
+    info('------------- Niche network construct --------------- ')
     # load original data
     ori_data_df = load_original_data(options=options)
 
     # define edges for each sample
     construct_niche_network(options=options, ori_data_df=ori_data_df)
 
     # save samples.yaml
     gen_samples_yaml(options=options, ori_data_df=ori_data_df)
+    info('------------ Niche network construct end ------------ ')
 
     # ----- Graph Pooling -----
-    # device
-    device: torch.device = device_validate(device_name=options.device)
+    info('------------------------ GNN ------------------------ ')
     # load data
     dataset, sample_loader = load_data(options=options)
     # random seed
     n_seed = t_seed = r_seed = options.seed
     random.seed(a=r_seed)
     torch.manual_seed(seed=t_seed)
     np.random.seed(seed=n_seed)
     # train
     inspect_funcs_list = get_inspect_funcs()
     batch_train: SubBatchTrainProtocol = train(nn_model=GraphPooling,
                                                options=options,
                                                BatchTrain=GPBatchTrain,
-                                               device=device,
+                                               device=torch.device(options.device),
                                                dataset=dataset,
                                                sample_loader=sample_loader,
                                                inspect_funcs=inspect_funcs_list,
                                                model_name='GraphPooling')
     # evaluate
     evaluate(batch_train=batch_train, model_name='GraphPooling')
     # predict
@@ -86,21 +87,24 @@
     if consolidate_s_array is not None:
         graph_pooling_output(ori_data_df=ori_data_df,
                              dataset=dataset,
                              rel_params=get_rel_params(
                                  options=options, params=read_yaml_file(f'{options.preprocessing_dir}/samples.yaml')),
                              consolidate_s_array=consolidate_s_array,
                              output_dir=options.GNN_dir)
+    info('---------------------- GNN end ---------------------- ')
 
     # ----- NT score -----
     if consolidate_s_array is not None and consolidate_out_adj_array is not None:
+        info('----------------- Niche trajectory ------------------ ')
         NTScore(options=options,
                 dataset=dataset,
                 consolidate_s_array=consolidate_s_array,
                 consolidate_out_adj_array=consolidate_out_adj_array)
+        info('--------------- Niche trajectory end ---------------- ')
 
 
 # ------------------------------------
 # Program running
 # ------------------------------------
 if __name__ == '__main__':
     try:
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC/bin/ONTraC_analysis.py` & `ontrac-0.0.7/src/ONTraC/bin/ONTraC_analysis.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/bin/createDataSet.py` & `ontrac-0.0.7/src/ONTraC/bin/createDataSet.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/data.py` & `ontrac-0.0.7/src/ONTraC/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 from optparse import Values
-from typing import Dict, List, Tuple
+from typing import Dict, List
 
 import numpy as np
 import pandas as pd
 import torch
 import torch_geometric.transforms as T
 from torch_geometric.data import Data, InMemoryDataset
-from torch_geometric.loader import DenseDataLoader
 
 from .log import *
-from .utils import count_lines, device_validate, get_rel_params, read_yaml_file
+from .utils import count_lines, get_rel_params, read_yaml_file
 
 
 # ------------------------------------
 # Classes
 # ------------------------------------
 class SpatailOmicsDataset(InMemoryDataset):
 
     def __init__(self, root, params: Dict, transform=None, pre_transform=None):
         self.params = params
         super(SpatailOmicsDataset, self).__init__(root, transform, pre_transform)
-        self.data, self.slices = torch.load(self.processed_paths[0])
 
     @property
-    def raw_file_names(self):
+    def raw_file_names(self):  # required by InMemoryDataset
         # return list(
         #     flatten([[sample for name, sample in data.items() if name != 'Name'] for data in self.params['Data']]))
         return []
 
     @property
     def processed_file_names(self):
         return ['data.pt']
 
     def download(self):
         pass
 
     def process(self):
         data_list = []
         for index, sample in enumerate(self.params['Data']):
-            info(f'Processing sample {index + 1} of {len(self.params["Data"])}')
+            info(f'Processing sample {index + 1} of {len(self.params["Data"])}: {sample["Name"]}')
             data = Data(
                 x=torch.from_numpy(np.loadtxt(sample['Features'], dtype=np.float32, delimiter=',')),
                 edge_index=torch.from_numpy(np.loadtxt(sample['EdgeIndex'], dtype=np.int64,
                                                        delimiter=',')).t().contiguous(),
                 # TODO: support 3D coordinates
                 pos=torch.from_numpy(pd.read_csv(sample['Coordinates'])[['x', 'y']].values),
                 name=sample['Name'])
             data_list.append(data)
-        data, slices = self.collate(data_list)
-        torch.save((data, slices), self.processed_paths[0])
+        self.data, self.slices = self.collate(data_list)
 
 
 # ------------------------------------
 # Misc functions
 # ------------------------------------
 def max_nodes(samples: List[Dict[str, str]]) -> int:
     """
@@ -62,41 +59,40 @@
     """
     max_nodes = 0
     for sample in samples:
         max_nodes = max(max_nodes, count_lines(sample['Coordinates']))
     return max_nodes
 
 
-def load_dataset(options: Values) -> Tuple[SpatailOmicsDataset, Data]:
-    device = device_validate()
+def load_dataset(options: Values) -> SpatailOmicsDataset:
+    """
+    Load dataset
+    :param options: Values, input options
+    :return: SpatailOmicsDataset, torch dataset
+    """
     params = read_yaml_file(f'{options.preprocessing_dir}/samples.yaml')
     rel_params = get_rel_params(options, params)
     dataset = create_torch_dataset(options, rel_params)
-    all_sample_loader = DenseDataLoader(dataset, batch_size=len(dataset))
-    data = next(iter(all_sample_loader)).to(device)
-    return dataset, data
+    return dataset
 
 
 # ------------------------------------
 # Flow control functions
 # ------------------------------------
 def create_torch_dataset(options: Values, params: Dict) -> SpatailOmicsDataset:
     """
     Create torch dataset
     :param params: Dict, input samples
     :return: None
     """
 
-    # ------------------------------------
     # Step 1: Get the maximum number of nodes
     m_nodes = max_nodes(params['Data'])
     # upcelling m_nodes to the nearest 100
     m_nodes = int(np.ceil(m_nodes / 100.0)) * 100
-    info(f'Maximum number of nodes: {m_nodes}')
-    # ------------------------------------
+    info(f'Maximum number of cell in one sample is: {m_nodes}.')
 
-    # ------------------------------------
     # Step 2: Create torch dataset
     dataset = SpatailOmicsDataset(root=options.preprocessing_dir, params=params,
                                   transform=T.ToDense(m_nodes))  # transform edge_index to adj matrix
-    # dataset = SpatailOmicsDataset(root=options.input, params=params)
+    dataset.process()
     return dataset
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC/log.py` & `ontrac-0.0.7/src/ONTraC/log.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/model/_model.py` & `ontrac-0.0.7/src/ONTraC/model/_model.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/model/dmon_exp_pool.py` & `ontrac-0.0.7/src/ONTraC/model/dmon_exp_pool.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/model/norm_dense_gcn_conv.py` & `ontrac-0.0.7/src/ONTraC/model/norm_dense_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/optparser/_GP.py` & `ontrac-0.0.7/src/ONTraC/optparser/_GP.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/optparser/_IO.py` & `ontrac-0.0.7/src/ONTraC/optparser/_IO.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/optparser/_NT.py` & `ontrac-0.0.7/src/ONTraC/optparser/_NT.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/optparser/_ONTraC.py` & `ontrac-0.0.7/src/ONTraC/optparser/_ONTraC.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/optparser/_create_dataset.py` & `ontrac-0.0.7/src/ONTraC/optparser/_create_dataset.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/optparser/_train.py` & `ontrac-0.0.7/src/ONTraC/optparser/_train.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     :return: None.
     """
 
     # GNN options group
     group_train.add_option('--hidden-feats',
                            dest='hidden_feats',
                            type='int',
-                           default=32,
+                           default=4,
                            help='Number of hidden features. Default is 4.')
 
 
 def add_NP_options_group(group_train: OptionGroup) -> None:
     """
     Add Node Pooling options group to optparser.
     :param optparser: OptionParser object.
@@ -77,58 +77,64 @@
     """
 
     # NP options group
     group_train.add_option('-k',
                            '--k-clusters',
                            dest='k',
                            type='int',
-                           default=8,
+                           default=6,
                            help='Number of niche clusters. Default is 6.')
     group_train.add_option('--modularity-loss-weight',
                            dest='modularity_loss_weight',
                            type='float',
-                           default=1,
+                           default=0.3,
                            help='Weight for modularity loss. Default is 0.3.')
     group_train.add_option('--purity-loss-weight',
                            dest='purity_loss_weight',
                            type='float',
-                           default=0,
+                           default=300,
                            help='Weight for purity loss. Default is 300.')
     group_train.add_option('--regularization-loss-weight',
                            dest='regularization_loss_weight',
                            type='float',
-                           default=1,
+                           default=0.1,
                            help='Weight for regularization loss. Default is 0.1.')
     group_train.add_option('--beta',
                            dest='beta',
                            type='float',
-                           default=1,
+                           default=0.3,
                            help='Beta value control niche cluster assignment matrix. Default is 0.3.')
 
 
 def validate_train_options(optparser: OptionParser, options: Values) -> Values:
     """
     Validate train options.
     :param optparser: OptionParser object.
     :param options: Options object.
     :return: Validated options object.
     """
 
     # device
-    if not options.device:
+    if options.device is None:
+        info('Device not specified, choose automatically.')
+    elif options.device.startswith(('cuda', 'cpu')):
+        if options.device.startswith('cuda') and not torch.cuda.is_available():
+            warning('CUDA is not available, use CPU instead.')
+            options.device = 'cpu'
+    else:
+        warning(f'Invalid device {options.device}! Choose automatically.')
+        options.device = None
+    if options.device is None:
         if torch.cuda.is_available():
             options.device = 'cuda'
-        elif torch.backends.mps.is_available():
-            options.device = 'mps'
+        # elif torch.backends.mps.is_available():  # TODO: MPS compatibility with torch_geometric.data.InMemoryDataset
+        #     options.device = 'mps'
         else:
             options.device = 'cpu'
-    if not options.device.startswith(('cuda', 'mps', 'cpu')):
-        error(f'Invalid device {options.device}, exit!')
-        sys.exit(1)
-
+    
     # determin random seed
     if getattr(options, 'seed') is None:
         options.seed = randint(0, 10000)
 
     return options
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC/run/processes.py` & `ontrac-0.0.7/src/ONTraC/run/processes.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 import numpy as np
 import pandas as pd
 import torch
 from numpy import ndarray
 from scipy.sparse import load_npz
 from torch_geometric.loader import DenseDataLoader
 
-from ONTraC.data import SpatailOmicsDataset, create_torch_dataset
+from ONTraC.data import SpatailOmicsDataset, load_dataset
 from ONTraC.log import *
 from ONTraC.train import SubBatchTrainProtocol
 from ONTraC.utils import get_rel_params, read_yaml_file
-from ONTraC.utils.NTScore import (NTScore_table, get_niche_NTScore,
-                                  niche_to_cell_NTScore)
+from ONTraC.utils.NTScore import NTScore_table, get_niche_NTScore, niche_to_cell_NTScore
 
 
 def load_parameters(opt_validate_func: Callable, prepare_optparser_func: Callable) -> Values:
     """
     Load parameters
     :param opt_validate_func: validate function
     :param prepare_optparser_func: prepare optparser function
@@ -30,26 +29,28 @@
 
 def load_data(options: Values) -> Tuple[SpatailOmicsDataset, DenseDataLoader]:
     """
     Load data
     :param options: options
     :return: dataset, sample_loader
     """
-    params = read_yaml_file(f'{options.preprocessing_dir}/samples.yaml')
-    rel_params = get_rel_params(options, params)
-    dataset = create_torch_dataset(options, rel_params)
+
+    info('Loading dataset.')
+
+    dataset = load_dataset(options=options)
     batch_size = options.batch_size if options.batch_size > 0 else len(dataset)
     sample_loader = DenseDataLoader(dataset, batch_size=batch_size)
+
     return dataset, sample_loader
 
 
 def train(nn_model: Type[torch.nn.Module], options: Values, BatchTrain: Type[SubBatchTrainProtocol],
           device: torch.device, dataset: SpatailOmicsDataset, sample_loader: DenseDataLoader,
           inspect_funcs: Optional[List[Callable]], model_name: str) -> SubBatchTrainProtocol:
-    info(message=f'{model_name} train start.')
+    info(message=f'Training process start.')
     model = nn_model(input_feats=dataset.num_features,
                      hidden_feats=options.hidden_feats,
                      k=options.k,
                      exponent=options.beta)
     optimizer = torch.optim.Adam(model.parameters(), lr=options.lr)
     batch_train = BatchTrain(model=model, device=device, data_loader=sample_loader)  # type: ignore
     batch_train.save(path=f'{options.GNN_dir}/epoch_0.pt')
@@ -64,25 +65,27 @@
                       max_epochs=options.epochs,
                       max_patience=options.patience,
                       min_delta=options.min_delta,
                       min_epochs=options.min_epochs,
                       output=options.GNN_dir,
                       **loss_weight_args)
     batch_train.save(path=f'{options.GNN_dir}/model_state_dict.pt')
+    info(message=f'Training process end.')
     return batch_train
 
 
 def evaluate(batch_train: SubBatchTrainProtocol, model_name: str) -> None:
     """
     Evaluate process
     :return: None
     """
-    info(message=f'{model_name} eval start.')
+    info(message=f'Evaluating process start.')
     loss_dict: Dict[str, np.floating] = batch_train.evaluate()  # type: ignore
     info(message=f'Evaluate loss, {repr(loss_dict)}')
+    info(message=f'Evaluating process end.')
 
 
 def graph_pooling_output(ori_data_df: pd.DataFrame, dataset: SpatailOmicsDataset, rel_params: Dict,
                          consolidate_s_array: np.ndarray, output_dir: str) -> None:
     """
     Write the graph pooling results as the Niche cluster (max probability for each niche & cell).
     :param ori_data_df: pd.DataFrame, original data
@@ -111,37 +114,44 @@
         consolidate_s_cell_df_ = pd.DataFrame(consolidate_s_cell,
                                               columns=[f'NicheCluster_{i}' for i in range(consolidate_s_cell.shape[1])])
         consolidate_s_cell_df_['Cell_ID'] = ori_data_df[ori_data_df['Sample'] == data.name]['Cell_ID'].values
         consolidate_s_cell_df = pd.concat([consolidate_s_cell_df, consolidate_s_cell_df_], axis=0)
 
     consolidate_s_niche_df = consolidate_s_niche_df.set_index('Cell_ID')
     consolidate_s_niche_df = consolidate_s_niche_df.loc[ori_data_df['Cell_ID'], :]
-    consolidate_s_niche_df.to_csv(f'{output_dir}/niche_level_niche_cluster.csv.gz', index=True, index_label='Cell_ID', header=True)
+    consolidate_s_niche_df.to_csv(f'{output_dir}/niche_level_niche_cluster.csv.gz',
+                                  index=True,
+                                  index_label='Cell_ID',
+                                  header=True)
     consolidate_s_niche_df['Niche_Cluster'] = consolidate_s_niche_df.values.argmax(axis=1)
     consolidate_s_niche_df['Niche_Cluster'].to_csv(f'{output_dir}/niche_level_max_niche_cluster.csv.gz',
                                                    index=True,
                                                    header=True)
     consolidate_s_cell_df = consolidate_s_cell_df.set_index('Cell_ID')
     consolidate_s_cell_df = consolidate_s_cell_df.loc[ori_data_df['Cell_ID'], :]
-    consolidate_s_cell_df.to_csv(f'{output_dir}/cell_level_niche_cluster.csv.gz', index=True, index_label='Cell_ID', header=True)
+    consolidate_s_cell_df.to_csv(f'{output_dir}/cell_level_niche_cluster.csv.gz',
+                                 index=True,
+                                 index_label='Cell_ID',
+                                 header=True)
     consolidate_s_cell_df['Niche_Cluster'] = consolidate_s_cell_df.values.argmax(axis=1)
     consolidate_s_cell_df['Niche_Cluster'].to_csv(f'{output_dir}/cell_level_max_niche_cluster.csv.gz',
                                                   index=True,
                                                   header=True)
 
 
 def predict(output_dir: str, batch_train: SubBatchTrainProtocol, dataset: SpatailOmicsDataset,
             model_name: str) -> Tuple[Optional[np.ndarray], Optional[np.ndarray]]:
-    info(f'{model_name} predict start.')
+    info(f'Predicting process start.')
     each_sample_loader = DenseDataLoader(dataset, batch_size=1)
     consolidate_flag = False
     consolidate_s_list = []
     consolidate_out = None
     consolidate_out_adj = None
     for data in each_sample_loader:  # type: ignore
+        info(f'Generating prediction results for {data.name[0]}.')
         data = data.to(batch_train.device)  # type: ignore
         predict_result = batch_train.predict_dict(data=data)  # type: ignore
         for key, value in predict_result.items():
             np.savetxt(fname=f'{output_dir}/{data.name[0]}_{key}.csv.gz',
                        X=value.squeeze(0).detach().cpu().numpy(),
                        delimiter=',')
 
@@ -154,14 +164,15 @@
             s = s.squeeze(0)
             consolidate_s_list.append(s)
             out_adj_ = torch.matmul(torch.matmul(s.T, data.adj.squeeze(0)), s)
             consolidate_out_adj = out_adj_ if consolidate_out_adj is None else consolidate_out_adj + out_adj_
             consolidate_out = out.squeeze(
                 0) * data.mask.sum() if consolidate_out is None else consolidate_out + out.squeeze(0) * data.mask.sum()
 
+    consolidate_s_array, consolidate_out_adj_array = None, None
     if consolidate_flag:
         # consolidate out
         nodes_num = 0
         for data in each_sample_loader:  # type: ignore
             nodes_num += data.mask.sum()
         consolidate_out = consolidate_out / nodes_num  # type: ignore
         consolidate_out_array = consolidate_out.detach().cpu().numpy()
@@ -175,17 +186,16 @@
         d = torch.sqrt(d)[:, None] + 1e-15
         consolidate_out_adj = (consolidate_out_adj / d) / d.transpose(0, 1)
         consolidate_s_array = consolidate_s.detach().cpu().numpy()
         consolidate_out_adj_array = consolidate_out_adj.detach().cpu().numpy()
         np.savetxt(fname=f'{output_dir}/consolidate_s.csv.gz', X=consolidate_s_array, delimiter=',')
         np.savetxt(fname=f'{output_dir}/consolidate_out_adj.csv.gz', X=consolidate_out_adj_array, delimiter=',')
 
-        return consolidate_s_array, consolidate_out_adj_array
-    else:
-        return None, None
+    info(f'Predicting process end.')
+    return consolidate_s_array, consolidate_out_adj_array
 
 
 def NTScore(options: Values, dataset: SpatailOmicsDataset, consolidate_s_array: ndarray,
             consolidate_out_adj_array: ndarray) -> None:
     """
     Pseudotime calculateion process
     :param options: options
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC/train/_batch_train.py` & `ontrac-0.0.7/src/ONTraC/train/_batch_train.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/train/inspect_funcs.py` & `ontrac-0.0.7/src/ONTraC/train/inspect_funcs.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/train/loss_funs.py` & `ontrac-0.0.7/src/ONTraC/train/loss_funs.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/utils/NTScore.py` & `ontrac-0.0.7/src/ONTraC/utils/NTScore.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,23 +3,27 @@
 from typing import Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
 from numpy import ndarray
 from scipy.sparse import load_npz
 
-from ONTraC.data import SpatailOmicsDataset
+from ..data import SpatailOmicsDataset
+from ..log import info
 
 
 def get_niche_trajectory_path(niche_adj_matrix: ndarray) -> List[int]:
     """
     Find niche level trajectory with maximum connectivity using Brute Force
     :param adj_matrix: non-negative ndarray, adjacency matrix of the graph
     :return: List[int], the niche trajectory
     """
+
+    info('Finding niche trajectory with maximum connectivity using Brute Force.')
+
     max_connectivity = float('-inf')
     niche_trajectory_path = []
     for path in itertools.permutations(range(len(niche_adj_matrix))):
         connectivity = 0
         for i in range(len(path) - 1):
             connectivity += niche_adj_matrix[path[i], path[i + 1]]
         if connectivity > max_connectivity:
@@ -32,14 +36,16 @@
 def trajectory_path_to_NC_score(niche_trajectory_path: List[int]) -> ndarray:
     """
     Convert niche cluster trajectory path to NTScore
     :param niche_trajectory_path: List[int], the niche trajectory path
     :return: ndarray, the NTScore
     """
 
+    info('Calculating NTScore for each niche cluster based on the trajectory path.')
+
     niche_NT_score = np.zeros(len(niche_trajectory_path))
     values = np.linspace(0, 1, len(niche_trajectory_path))
 
     for i, index in enumerate(niche_trajectory_path):
         # debug(f'i: {i}, index: {index}')
         niche_NT_score[index] = values[i]
     return niche_NT_score
@@ -49,14 +55,16 @@
     """
     Get niche-level niche trajectory and cell-level niche trajectory
     :param niche_cluster_loading: ndarray, the loading of cell x niche clusters
     :param adj_matrix: ndarray, the adjacency matrix of the graph
     :return: Tuple[ndarray, ndarray], the niche-level niche trajectory and cell-level niche trajectory
     """
 
+    info('Calculating NTScore for each niche.')
+
     niche_trajectory_path = get_niche_trajectory_path(niche_adj_matrix=niche_adj_matrix)
 
     niche_cluster_score = trajectory_path_to_NC_score(niche_trajectory_path)
     niche_level_NTScore = niche_cluster_loading @ niche_cluster_score
     return niche_cluster_score, niche_level_NTScore
 
 
@@ -67,14 +75,16 @@
     :param dataset: SpatailOmicsDataset, dataset
     :param rel_params: Dict, relative paths
     :param niche_level_NTScore: ndarray, niche-level NTScore
     :return: Tuple[ndarray, Dict[str, ndarray], Dict[str, ndarray]], the cell-level NTScore, all niche-level NTScore dict,
     and all cell-level NTScore dict
     """
 
+    info('Projecting NTScore from niche-level to cell-level.')
+
     cell_level_NTScore = np.zeros(niche_level_NTScore.shape[0])
 
     all_niche_level_NTScore_dict: Dict[str, ndarray] = {}
     all_cell_level_NTScore_dict: Dict[str, ndarray] = {}
 
     for i, data in enumerate(dataset):
         # the slice of data in each sample
@@ -105,14 +115,16 @@
     :param options: Values, options
     :param rel_params: Dict, relative paths
     :param all_niche_level_NTScore_dict: Dict[str, ndarray], all niche-level NTScore dict
     :param all_cell_level_NTScore_dict: Dict[str, ndarray], all cell-level NTScore dict
     :return: pd.DataFrame, NTScore table
     """
 
+    info('Output NTScore tables.')
+
     NTScore_table = pd.DataFrame()
     for sample in rel_params['Data']:
         coordinates_df = pd.read_csv(sample['Coordinates'], index_col=0)
         coordinates_df['Niche_NTScore'] = all_niche_level_NTScore_dict[sample['Name']]
         coordinates_df['Cell_NTScore'] = all_cell_level_NTScore_dict[sample['Name']]
         coordinates_df.to_csv(f'{options.NTScore_dir}/{sample["Name"]}_NTScore.csv.gz')
         NTScore_table = pd.concat([NTScore_table, coordinates_df])
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC/utils/_utils.py` & `ontrac-0.0.7/src/ONTraC/utils/_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import sys
 from copy import deepcopy
 from optparse import Values
-from typing import Dict, Optional
+from typing import Dict
 
-import torch
 import yaml
 
-from ..log import warning
-
 
 def write_version_info() -> None:
     """
     Write version information to stdout
     """
     from .. import __version__
-    template = f'''########################################################
+    template = f'''##################################################################################
 
- ▄▄█▀▀██   ▀█▄   ▀█▀ █▀▀██▀▀█                   ▄▄█▀▀▀▄█
-▄█▀    ██   █▀█   █     ██    ▄▄▄ ▄▄   ▄▄▄▄   ▄█▀     ▀
-██      ██  █ ▀█▄ █     ██     ██▀ ▀▀ ▀▀ ▄██  ██
-▀█▄     ██  █   ███     ██     ██     ▄█▀ ██  ▀█▄      ▄
- ▀▀█▄▄▄█▀  ▄█▄   ▀█    ▄██▄   ▄██▄    ▀█▄▄▀█▀  ▀▀█▄▄▄▄▀
+         ▄▄█▀▀██   ▀█▄   ▀█▀ █▀▀██▀▀█                   ▄▄█▀▀▀▄█
+        ▄█▀    ██   █▀█   █     ██    ▄▄▄ ▄▄   ▄▄▄▄   ▄█▀     ▀
+        ██      ██  █ ▀█▄ █     ██     ██▀ ▀▀ ▀▀ ▄██  ██
+        ▀█▄     ██  █   ███     ██     ██     ▄█▀ ██  ▀█▄      ▄
+         ▀▀█▄▄▄█▀  ▄█▄   ▀█    ▄██▄   ▄██▄    ▀█▄▄▀█▀  ▀▀█▄▄▄▄▀
 
-                version: {__version__}
+                        version: {__version__}
 
-########################################################
+##################################################################################
 '''
 
     sys.stdout.write(template)
     sys.stdout.flush()
 
 
 def read_yaml_file(yaml_file: str) -> dict:
@@ -85,24 +82,7 @@
         :param n: int
         :return: bool
         """
         num = len(str(n))
         return n % (10**(num - 1)) == 0
 
     return epoch < 10 or _is_power_of_10(epoch)
-
-
-def device_validate(device_name: Optional[str] = None) -> torch.device:
-    if device_name is None:
-        device_name = 'cpu'
-    elif device_name.startswith('cuda') and not torch.cuda.is_available():
-        warning('CUDA is not available, use CPU instead.')
-        device_name = 'cpu'
-    # elif device_name.startswith('mps') and not torch.backends.mps.is_available():
-    #     warning('MPS is not available, use CPU instead.')
-    #     device_name = 'cpu'
-    else:
-        device_name = 'cpu'
-
-    device = torch.device(device=device_name)
-
-    return device
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC/utils/decorators.py` & `ontrac-0.0.7/src/ONTraC/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ontrac-0.0.6.post2/src/ONTraC/utils/niche_net_constr.py` & `ontrac-0.0.7/src/ONTraC/utils/niche_net_constr.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import pandas as pd
 import yaml
 from scipy.sparse import csr_matrix, save_npz
 from scipy.spatial import cKDTree
 
-from ..log import warning
+from ..log import warning, info
 
 
 def load_original_data(options: Values) -> pd.DataFrame:
     """
     Load original data
     :param options: Values, options
     :return: pd.DataFrame, original data
@@ -84,15 +84,17 @@
     2) save the celltype information
     3) build KDTree
         1. save edge index file
         2. calculate weight matrix
         3. calculate cell type composition and save it
     """
 
-    n_local = 20
+    info(f'Constructing niche network for sample: {sample_name}.')
+
+    n_local = 20  # TODO: make it as an option
     N = sample_data_df.shape[0]
 
     # get coordinates
     # TODO: support 3D coordinates
     coord_df = sample_data_df[['Cell_ID', 'x', 'y']]
     coord_df.to_csv(f'{options.preprocessing_dir}/{sample_name}_Coordinates.csv', index=False)
 
@@ -160,14 +162,16 @@
 def gen_samples_yaml(options: Values, ori_data_df: pd.DataFrame) -> None:
     """
     Generate samples.yaml
     :param ori_data_df: pd.DataFrame, original data
     :return: None
     """
 
+    info('Generating samples.yaml file.')
+
     data: Dict[str, List[Any]] = {'Data': []}
     for sample in ori_data_df['Sample'].unique():
         data['Data'].append({
             'Name': f'{sample}',
             'Coordinates': f'{sample}_Coordinates.csv',
             'EdgeIndex': f'{sample}_EdgeIndex.csv.gz',
             'Features': f'{sample}_CellTypeComposition.csv.gz',
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC.egg-info/PKG-INFO` & `ontrac-0.0.7/src/ONTraC.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ONTraC
-Version: 0.0.6.post2
+Version: 0.0.7
 Summary: A niche-centered, machine learning method for constructing spatially continuous trajectories
 Author-email: Wen Wang <wwang.bio@gmail.com>, Shiwei Zheng <swzheng29@gmail.com>, Crystal Shin <sjcshin5040@gmail.com>, Guo-Cheng Yuan <gcyuan@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gyuanlab/ONTraC
 Project-URL: Repository, https://github.com/gyuanlab/ONTraC
 Project-URL: Issue Tracker, https://github.com/gyuanlab/ONTraC/issues
 Keywords: deep-learning,pytorch,pytorch geometric,trajectory inference,spatial omics
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: ==3.11.*
@@ -24,14 +24,20 @@
 Requires-Dist: torch-geometric==2.5.0
 Provides-Extra: analysis
 Requires-Dist: matplotlib; extra == "analysis"
 Requires-Dist: seaborn; extra == "analysis"
 
 # **ONTraC**
 
+[![PyPI Latest Release](https://img.shields.io/pypi/v/ONTraC.svg)](https://pypi.org/project/ONTraC/)
+[![Downloads](https://static.pepy.tech/badge/ONTraC)](https://pepy.tech/project/ONTraC)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/ONTraC.svg?label=PyPI%20downloads)](https://pypi.org/project/ONTraC/)
+[![GitHub stars](https://badgen.net/github/stars/gyuanlab/ONTraC)](https://github.com/gyuanlab/ONTraC)
+[![GitHub license](https://img.shields.io/github/license/gyuanlab/ONTraC.svg)](https://github.com/gyuanlab/ONTraC/blob/master/LICENSE)
+
 ONTraC (Ordered Niche Trajectory Construction) is a niche-centered, machine learning
 method for constructing spatially continuous trajectories. ONTraC differs from existing tools in
 that it treats a niche, rather than an individual cell, as the basic unit for spatial trajectory
 analysis. In this context, we define niche as a multicellular, spatially localized region where
 different cell types may coexist and interact with each other.  ONTraC seamlessly integrates
 cell-type composition and spatial information by using the graph neural network modeling
 framework. Its output, which is called the niche trajectory, can be viewed as a one dimensional
@@ -154,7 +160,9 @@
 The intermediate and final results are located in `preprocessing-dir`, `GNN-dir`, and `NTScore-dir` directories. Please see [IO files explanation](tutorials/IO_files.md#output-files) for detailed infromation.
 
 ### Visualization
 
 Please see [post analysis tutorial](tutorials/post_analysis.md).
 
 ## Citation
+
+**Wang, W.\*, Zheng, S.\*, Shin, C. S. & Yuan, G. C.$**. [Characterizing Spatially Continuous Variations in Tissue Microenvironment through Niche Trajectory Analysis]((https://www.biorxiv.org/content/10.1101/2024.04.23.590827v1)). *bioRxiv*, 2024.
```

### Comparing `ontrac-0.0.6.post2/src/ONTraC.egg-info/SOURCES.txt` & `ontrac-0.0.7/src/ONTraC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

