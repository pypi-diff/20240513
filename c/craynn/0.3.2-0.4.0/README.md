# Comparing `tmp/craynn-0.3.2.tar.gz` & `tmp/craynn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/craynn-0.3.2.tar", last modified: Tue Dec 22 10:10:18 2020, max compression
+gzip compressed data, was "craynn-0.4.0.tar", last modified: Mon May 13 13:51:53 2024, max compression
```

## Comparing `craynn-0.3.2.tar` & `craynn-0.4.0.tar`

### file list

```diff
@@ -1,98 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/
--rw-r--r--   0 root         (0) root         (0)     2732 2020-12-22 10:10:18.000000 craynn-0.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1662 2020-12-22 10:10:17.000000 craynn-0.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/
--rw-rw-rw-   0 root         (0) root         (0)      757 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/info/
--rw-rw-rw-   0 root         (0) root         (0)       21 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4856 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/info/layers.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/info/nodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/layers/
--rw-rw-rw-   0 root         (0) root         (0)      192 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11311 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/layers/conv_ops/
--rw-rw-rw-   0 root         (0) root         (0)       89 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/conv_ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5881 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/conv_ops/_conv.py
--rw-rw-rw-   0 root         (0) root         (0)     4611 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/conv_ops/_deconv.py
--rw-rw-rw-   0 root         (0) root         (0)     5914 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/conv_ops/_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     1838 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/conv_ops/_upscale.py
--rw-rw-rw-   0 root         (0) root         (0)     4438 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/conv_ops/conv_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5218 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/dense_ops.py
--rw-rw-rw-   0 root         (0) root         (0)      851 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/gates.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/gmm.py
--rw-rw-rw-   0 root         (0) root         (0)     6112 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/meta.py
--rw-rw-rw-   0 root         (0) root         (0)      378 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/meta_ops.py
--rw-rw-rw-   0 root         (0) root         (0)     1956 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/noise_ops.py
--rw-rw-rw-   0 root         (0) root         (0)     3593 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/layers/normalization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/networks/
--rw-rw-rw-   0 root         (0) root         (0)       19 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/networks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7387 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/networks/meta.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/networks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/nonlinearities/
--rw-rw-rw-   0 root         (0) root         (0)       45 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/nonlinearities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1315 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/nonlinearities/common.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/nonlinearities/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/nonlinearities/meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/objectives/
--rw-rw-rw-   0 root         (0) root         (0)      156 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/objectives/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6617 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/objectives/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     2998 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/objectives/common.py
--rw-rw-rw-   0 root         (0) root         (0)     1895 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/objectives/elbo.py
--rw-rw-rw-   0 root         (0) root         (0)     1397 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/objectives/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     1339 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/objectives/regression.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/objectives/regularization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/parameters/
--rw-rw-rw-   0 root         (0) root         (0)      215 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/binary.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/common.py
--rw-rw-rw-   0 root         (0) root         (0)     1324 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)      288 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/glorot.py
--rw-rw-rw-   0 root         (0) root         (0)      864 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/masked.py
--rw-rw-rw-   0 root         (0) root         (0)    11264 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/meta.py
--rw-rw-rw-   0 root         (0) root         (0)      864 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/noisy.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/normed.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/orthogonal.py
--rw-rw-rw-   0 root         (0) root         (0)      464 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/parameter_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/parameters/restricted.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/regularization/
--rw-rw-rw-   0 root         (0) root         (0)       42 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/regularization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/regularization/common.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/regularization/meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/subnetworks/
--rw-rw-rw-   0 root         (0) root         (0)      824 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/subnetworks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/subnetworks/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/subnetworks/meta_nets.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/subnetworks/normalization.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/subnetworks/residual_nets.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/subnetworks/skip.py
--rw-rw-rw-   0 root         (0) root         (0)      520 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/subnetworks/vae_nets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/updates/
--rw-rw-rw-   0 root         (0) root         (0)       49 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/updates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2236 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/updates/common.py
--rw-rw-rw-   0 root         (0) root         (0)     3366 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/updates/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/updates/subsets.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/updates/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2720 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/updates/variable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/utils/
--rw-rw-rw-   0 root         (0) root         (0)       64 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/utils/axes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/utils/data/
--rw-rw-rw-   0 root         (0) root         (0)       96 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/utils/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3831 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/utils/data/common.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/utils/data/concept_learning.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/utils/data/images.py
--rw-rw-rw-   0 root         (0) root         (0)     3140 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/utils/data/text.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/utils/tf_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn/viz/
--rw-rw-rw-   0 root         (0) root         (0)       72 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/viz/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4665 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/viz/visualize.py
--rw-rw-rw-   0 root         (0) root         (0)     4452 2020-12-22 10:10:17.000000 craynn-0.3.2/craynn/viz/watcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2732 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2253 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2020-12-22 10:10:18.000000 craynn-0.3.2/craynn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-12-22 10:10:18.000000 craynn-0.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1213 2020-12-22 10:10:17.000000 craynn-0.3.2/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.141054 craynn-0.4.0/
+-rw-rw-r--   0 max       (1000) max       (1000)     1071 2022-05-05 19:29:29.000000 craynn-0.4.0/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)     2300 2024-05-13 13:51:53.137054 craynn-0.4.0/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     1492 2024-05-13 13:09:59.000000 craynn-0.4.0/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.121054 craynn-0.4.0/craynn/
+-rw-rw-r--   0 max       (1000) max       (1000)      442 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/__init__.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.125054 craynn-0.4.0/craynn/dag/
+-rw-rw-r--   0 max       (1000) max       (1000)       87 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/dag/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      401 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/dag/common.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.125054 craynn-0.4.0/craynn/dag/evaluate/
+-rw-rw-r--   0 max       (1000) max       (1000)       65 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/dag/evaluate/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3552 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/dag/evaluate/common.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4717 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/dag/evaluate/dynamic.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4489 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/dag/evaluate/static.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.125054 craynn-0.4.0/craynn/dag/lang/
+-rw-rw-r--   0 max       (1000) max       (1000)       23 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/dag/lang/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1207 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/dag/lang/achain.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1203 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/dag/lang/language.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3577 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/dag/lang/selector.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3491 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/dag/meta.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.125054 craynn-0.4.0/craynn/info/
+-rw-rw-r--   0 max       (1000) max       (1000)       21 2022-05-05 19:29:29.000000 craynn-0.4.0/craynn/info/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4755 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/info/layers.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.129054 craynn-0.4.0/craynn/layers/
+-rw-rw-r--   0 max       (1000) max       (1000)      138 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/layers/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    14161 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/layers/common.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.129054 craynn-0.4.0/craynn/layers/conv_ops/
+-rw-rw-r--   0 max       (1000) max       (1000)       65 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/layers/conv_ops/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    12986 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/layers/conv_ops/_conv.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4044 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/layers/conv_ops/_pool.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2671 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/layers/conv_ops/_upscale.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5656 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/layers/conv_ops/conv_utils.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4298 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/layers/dense_ops.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2791 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/layers/gates.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4587 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/layers/meta.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3074 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/layers/noise_ops.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.129054 craynn-0.4.0/craynn/networks/
+-rw-rw-r--   0 max       (1000) max       (1000)       44 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/networks/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     9053 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/networks/meta.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1385 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/networks/utils.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.129054 craynn-0.4.0/craynn/nonlinearities/
+-rw-rw-r--   0 max       (1000) max       (1000)       76 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/nonlinearities/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2382 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/nonlinearities/common.py
+-rw-rw-r--   0 max       (1000) max       (1000)      331 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/nonlinearities/defaults.py
+-rw-rw-r--   0 max       (1000) max       (1000)      516 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/nonlinearities/meta.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.129054 craynn-0.4.0/craynn/objectives/
+-rw-rw-r--   0 max       (1000) max       (1000)      106 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/objectives/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3895 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/objectives/classification.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2529 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/objectives/elbo.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1799 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/objectives/regression.py
+-rw-rw-r--   0 max       (1000) max       (1000)      961 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/objectives/regularization.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.133054 craynn-0.4.0/craynn/parameters/
+-rw-rw-r--   0 max       (1000) max       (1000)      245 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/parameters/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4131 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/parameters/common.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1365 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/parameters/decomposition.py
+-rw-rw-r--   0 max       (1000) max       (1000)      280 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/parameters/defaults.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1345 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/parameters/glorot.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2181 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/parameters/masked.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5833 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/parameters/meta.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1002 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/parameters/noisy.py
+-rw-rw-r--   0 max       (1000) max       (1000)      765 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/parameters/orthogonal.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1939 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/parameters/restricted.py
+-rw-rw-r--   0 max       (1000) max       (1000)      187 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/parameters/utils.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.133054 craynn-0.4.0/craynn/subnetworks/
+-rw-rw-r--   0 max       (1000) max       (1000)      797 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/subnetworks/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      537 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/subnetworks/gates.py
+-rw-rw-r--   0 max       (1000) max       (1000)      757 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/subnetworks/meta.py
+-rw-rw-r--   0 max       (1000) max       (1000)      554 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/subnetworks/residual_nets.py
+-rw-rw-r--   0 max       (1000) max       (1000)      318 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/subnetworks/skip.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.133054 craynn-0.4.0/craynn/train/
+-rw-rw-r--   0 max       (1000) max       (1000)       21 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/train/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     6223 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/train/common.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.137054 craynn-0.4.0/craynn/updates/
+-rw-rw-r--   0 max       (1000) max       (1000)       46 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/updates/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      953 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/updates/array.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1632 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/updates/common.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2257 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/updates/meta.py
+-rw-rw-r--   0 max       (1000) max       (1000)      944 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/updates/subsets.py
+-rw-rw-r--   0 max       (1000) max       (1000)      961 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/updates/utils.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.137054 craynn-0.4.0/craynn/utils/
+-rw-rw-r--   0 max       (1000) max       (1000)       82 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/utils/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      538 2024-04-08 10:17:09.000000 craynn-0.4.0/craynn/utils/axes.py
+-rw-rw-r--   0 max       (1000) max       (1000)     9631 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/utils/clazz.py
+-rw-rw-r--   0 max       (1000) max       (1000)      981 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/utils/func.py
+-rw-rw-r--   0 max       (1000) max       (1000)      501 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/utils/math.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.137054 craynn-0.4.0/craynn/viz/
+-rw-rw-r--   0 max       (1000) max       (1000)       21 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/viz/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4867 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/viz/common.py
+-rw-rw-r--   0 max       (1000) max       (1000)    10302 2024-05-13 13:09:59.000000 craynn-0.4.0/craynn/viz/viz.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-13 13:51:53.137054 craynn-0.4.0/craynn.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     2300 2024-05-13 13:51:53.000000 craynn-0.4.0/craynn.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     2064 2024-05-13 13:51:53.000000 craynn-0.4.0/craynn.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2024-05-13 13:51:53.000000 craynn-0.4.0/craynn.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       95 2024-05-13 13:51:53.000000 craynn-0.4.0/craynn.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        7 2024-05-13 13:51:53.000000 craynn-0.4.0/craynn.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2024-05-13 13:51:53.141054 craynn-0.4.0/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)     1180 2024-05-13 13:51:43.000000 craynn-0.4.0/setup.py
```

### Comparing `craynn-0.3.2/PKG-INFO` & `craynn-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 Metadata-Version: 2.1
 Name: craynn
-Version: 0.3.2
+Version: 0.4.0
 Summary: Yet another neural network toolkit.
 Home-page: https://gitlab.com/craynn/craynn
 Author: Maxim Borisyak and contributors.
 Author-email: maximus.been@gmail.com
 Maintainer: Maxim Borisyak
 Maintainer-email: maximus.been@gmail.com
 License: MIT
-Description: # craynn
-        
-        Yet Another toolkit for Neural Network slightly flavoured by Ultra-High Energy Cosmic Rays. 
-        
-        ## Philosophy
-        
-        `CrayNN` is highly influenced by [Lasange](https://github.com/Lasagne/Lasagne):
-        
-            Simplicity: Be easy to use, easy to understand and easy to extend, to facilitate use in research
-            Transparency: Do not hide Theano behind abstractions, directly process and return Theano expressions or Python / numpy data types
-            Modularity: Allow all parts (layers, regularizers, optimizers, ...) to be used independently of Lasagne
-            Pragmatism: Make common use cases easy, do not overrate uncommon cases
-            Restraint: Do not obstruct users with features they decide not to use
-            Focus: "Do one thing and do it well"
-        
-        Just replace `theano` with `tensorflow`.
-        
-        ## Installation
-        
-        ### via PyPi
-        
-        `pip install craynn`
-        
-        ### via git
-        
-        `craynn` can be installed directly from `gitlab.com`:
-        `pip install git+https://gitlab.com/craynn/craynn.git`
-        however, as repository updates frequently, it is recommend to clone the repository
-        and install the package in development mode:
-        ```
-        git clone git@gitlab.com:craynn/craynn.git
-        cd craynn/
-        pip install -e .
-        ```
-        
-        **NB**: don't forget to install proper version of `craygraph` in a similar manner:
-        ```
-        git clone git@gitlab.com:craynn/craygraph.git
-        cd craygraph/
-        pip install -e .
-        ``` 
-        
-        ## Usage
-        
-        Check out jupyter notebooks in `examples/`. 
-        
-        ## Quick guide
-        
-        `craynn` is designed for rapidly defining networks of all sorts:
-        ```python
-        from craynn import network, conv, max_pool
-        
-        net = network((None, 1, 28, 28))(
-          conv(16), conv(24), max_pool(),
-          conv(16), conv(24), max_pool(),
-          conv(16), conv(24), max_pool(),
-        )
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: jax>=0.3.8
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: matplotlib>=3.0.2
+Requires-Dist: pydotplus>=2.0.2
 Provides-Extra: test
+Requires-Dist: pytest>=4.0.0; extra == "test"
+Requires-Dist: scipy>=1.3.0; extra == "test"
+
+# craynn
+
+Yet Another toolkit for Neural Network slightly flavoured by Ultra-High Energy Cosmic Rays. 
+
+## Philosophy
+
+`CrayNN` is highly influenced by [Lasange](https://github.com/Lasagne/Lasagne):
+
+    Simplicity: Be easy to use, easy to understand and easy to extend, to facilitate use in research
+    Transparency: Do not hide Theano behind abstractions, directly process and return Theano expressions or Python / numpy data types
+    Modularity: Allow all parts (layers, regularizers, optimizers, ...) to be used independently of Lasagne
+    Pragmatism: Make common use cases easy, do not overrate uncommon cases
+    Restraint: Do not obstruct users with features they decide not to use
+    Focus: "Do one thing and do it well"
+
+Just replace `theano` with `jax`.
+
+## Installation
+
+### via PyPi
+
+`pip install craynn`
+
+### via git
+
+`craynn` can be installed directly from `gitlab.com`:
+`pip install git+https://gitlab.com/craynn/craynn.git`
+however, as repository updates frequently, it is recommended to clone the repository
+and install the package in development mode:
+```
+git clone git@gitlab.com:craynn/craynn.git
+cd craynn/
+pip install -e .
+```
+
+## Usage
+
+Take a look at jupyter notebooks in `examples/`. 
+
+## Quick guide
+
+`craynn` is designed for rapidly defining networks of all sorts:
+```python
+from craynn import network, conv, max_pool
+
+net = network((None, 1, 28, 28))(
+  conv(16), conv(24), max_pool(),
+  conv(16), conv(24), max_pool(),
+  conv(16), conv(24), max_pool(),
+)
+```
```

### Comparing `craynn-0.3.2/README.md` & `craynn-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,44 +9,37 @@
     Simplicity: Be easy to use, easy to understand and easy to extend, to facilitate use in research
     Transparency: Do not hide Theano behind abstractions, directly process and return Theano expressions or Python / numpy data types
     Modularity: Allow all parts (layers, regularizers, optimizers, ...) to be used independently of Lasagne
     Pragmatism: Make common use cases easy, do not overrate uncommon cases
     Restraint: Do not obstruct users with features they decide not to use
     Focus: "Do one thing and do it well"
 
-Just replace `theano` with `tensorflow`.
+Just replace `theano` with `jax`.
 
 ## Installation
 
 ### via PyPi
 
 `pip install craynn`
 
 ### via git
 
 `craynn` can be installed directly from `gitlab.com`:
 `pip install git+https://gitlab.com/craynn/craynn.git`
-however, as repository updates frequently, it is recommend to clone the repository
+however, as repository updates frequently, it is recommended to clone the repository
 and install the package in development mode:
 ```
 git clone git@gitlab.com:craynn/craynn.git
 cd craynn/
 pip install -e .
 ```
 
-**NB**: don't forget to install proper version of `craygraph` in a similar manner:
-```
-git clone git@gitlab.com:craynn/craygraph.git
-cd craygraph/
-pip install -e .
-``` 
-
 ## Usage
 
-Check out jupyter notebooks in `examples/`. 
+Take a look at jupyter notebooks in `examples/`. 
 
 ## Quick guide
 
 `craynn` is designed for rapidly defining networks of all sorts:
 ```python
 from craynn import network, conv, max_pool
```

### Comparing `craynn-0.3.2/craynn/info/layers.py` & `craynn-0.4.0/craynn/info/layers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,48 @@
+import math
 import numpy as np
 
-from craygraph import Node, propagate, reduce_graph, get_name
+from .. import dag
 
-from ..layers.meta import Layer, get_output_shape, get_layers
-from ..parameters import get_all_variables, get_parameters
+from ..layers import Layer, get_layers
+from ..parameters import Parameter, FreeParameter, get_all_free_parameters, get_parameters
 
 __all__ = [
   'get_number_of_parameters',
   'get_total_number_of_parameters',
   'graph_description',
   'get_network_core'
 ]
 
 def _get_number_of_parameters(layer):
-  variables = getattr(layer, 'variables', list)()
-  if len(variables) > 0:
-    return sum(
-      np.prod(var.shape, dtype='int64')
-      for var in variables
-    )
+  if isinstance(layer, FreeParameter):
+    return math.prod(layer.shape)
   else:
     return 0
 
 def get_number_of_parameters(layer_or_layers):
-  def incoming(node : Node):
+  def incoming(node: dag.Node):
     if isinstance(node, Layer):
-      return node.parameters()
+      return node.parameters
     else:
-      return node.incoming()
+      return node.incoming
 
   def reducer(layer, inputs):
     own_variables = _get_number_of_parameters(layer)
-    num_parameters = len(getattr(layer, 'parameters', tuple)())
+    num_parameters = len(getattr(layer, 'parameters', ()))
 
     if num_parameters > 0:
       return sum(inputs[:num_parameters]) + own_variables
     else:
       return own_variables
 
-  return reduce_graph(reducer, layer_or_layers, incoming=incoming)
+  return dag.reduce(reducer, layer_or_layers)
 
 def get_total_number_of_parameters(layer, **properties):
-  variables = get_all_variables(layer, **properties)
+  variables = get_all_free_parameters(layer, **properties)
 
   return sum(
     np.prod(var.shape, dtype='int64')
     for var in variables
   )
 
 def get_attributes(layer, attributes):
@@ -59,40 +56,40 @@
     elif callable(attr):
       values[name] = attr(layer)
 
   return values
 
 def param_description(param):
   return '{name} {shape}: {properties}'.format(
-    name=get_name(param),
-    shape=tuple(param().shape.as_list()),
+    name=dag.get_name(param),
+    shape=tuple(param.shape),
     properties=', '.join(
       '%s=%s' % (k, v)
-      for k, v in getattr(param, 'properties', dict)().items()
+      for k, v in getattr(param, 'properties', dict()).items()
     )
   )
 
 def layer_description(layer, attributes, short=True):
   attrs = get_attributes(layer, attributes)
   additional = [ '%s=%s' % (k, v) for k, v in attrs.items() ]
 
   number_of_parameters = get_number_of_parameters(layer)
-  output_shape = get_output_shape(layer)
+  output_shape = dag.get_output_shape(layer)
 
   if short:
     return '{name}{clazz} ({nparams} params): {out_shape}{additional}'.format(
-      name='' if get_name(layer) is None else ('%s ' % get_name(layer)),
+      name='' if dag.get_name(layer) is None else ('%s ' % dag.get_name(layer)),
       clazz=layer.__class__.__name__,
       out_shape=output_shape,
       nparams=number_of_parameters,
       additional='' if len(additional) == 0 else ('\n  %s' % ', '.join(additional))
     )
   else:
     head = '{name}{clazz}: {out_shape}{additional}'.format(
-      name='' if get_name(layer) is None else ('%s ' % get_name(layer)),
+      name='' if dag.get_name(layer) is None else ('%s ' % dag.get_name(layer)),
       clazz=layer.__class__.__name__,
       out_shape=output_shape,
       additional='' if len(additional) == 0 else ('\n  %s' % '\n  '.join(additional))
     )
 
     params = get_parameters(layer)
     if len(params) == 0:
@@ -120,23 +117,23 @@
       for layer in all_layers
       if len(getattr(layer, 'incoming', tuple)()) == 0
     ]
 
   outputs = layer_or_layers
 
   input_summary = ', '.join(
-    '{shape}'.format(shape=get_output_shape(layer))
-    if get_name(layer) is None else
-    '{name}: {shape}'.format(name=get_name(layer), shape=get_output_shape(layer))
+    '{shape}'.format(shape=dag.get_output_shape(layer))
+    if dag.get_name(layer) is None else
+    '{name}: {shape}'.format(name=dag.get_name(layer), shape=dag.get_output_shape(layer))
 
     for layer in inputs
   )
 
   output_summary = ', '.join(
-    '{shape}'.format(shape=get_output_shape(layer))
+    '{shape}'.format(shape=dag.get_output_shape(layer))
     for layer in outputs
   )
 
   layer_delim = '\n' if short else '\n\n'
 
   layers_info = layer_delim.join(
     layer_description(
@@ -155,25 +152,25 @@
     layers_description=layers_info
   )
 
   return summary
 
 def get_network_core(layers):
   """
-  Network core, in this case, is a network with parameters
-  that does not depend onm any `Layer` excluded.
+  Network dag, in this case, is a network with parameters
+  that does not depend on any `Layer` excluded.
   :param layers: an instance of `Layer` or a list/tuple of `Layer`s
-  :return: collection of Layers included in the network core.
+  :return: collection of Layers included in the network dag.
   """
   def operator(node, inputs):
     return isinstance(node, Layer) or any(inputs)
 
   if not isinstance(layers, (tuple, list)):
     layers = (layers, )
 
-  results = propagate(operator, layers)
+  results = dag.propagate(operator, layers)
 
   return tuple(
     node
     for node in results
     if results[node]
   )
```

### Comparing `craynn-0.3.2/craynn/layers/common.py` & `craynn-0.4.0/craynn/layers/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,141 +1,173 @@
-import tensorflow as tf
-from craygraph import derive
+import functools
+import math
 
-from .meta import Layer, InputLayer
-from .meta import model_from
+import jax
+import jax.numpy as jnp
 
-from ..parameters import default_input_init
+from ..utils import normalize_axis, soft_maximum, soft_minimum
+from ..parameters import constant_parameter
+
+from .meta import Layer, InputLayer, LayerModel
 
 __all__ = [
   'const_input',
-  
-  'FunctionLayer', 'custom', 'nonlinearity',
+
+  'CustomLayer', 'custom_layer',
+  'FunctionLayer', 'function_layer',
+
   'ConcatLayer', 'concat',
   'FlattenLayer', 'flatten',
   'ReshapeLayer', 'reshape',
-  'TransposeLayer', 'transpose',
   'ExpandLayer', 'expand',
-  'RepeatLayer', 'repeat',
 
   'ElementwiseLayer', 'ElementwiseSumLayer', 'ElementwiseMeanLayer',
   'ElementwiseMaxLayer', 'ElementwiseMinLayer',
 
   'elementwise', 'elementwise_sum', 'elementwise_mean',
   'elementwise_max', 'elementwise_min',
 
-  'SquareDifference', 'square_difference',
+  'BroadcastLayer', 'broadcast',
+  'ExpandConcatLayer', 'expand_concat',
 
-  'BroadcastConcatLayer', 'broadcast_concat',
+  'GeneralPoolLayer', 'GeneralMaxPoolLayer', 'GeneralMeanPoolLayer', 'GeneralSumPoolLayer',
+  'general_max_pool', 'general_mean_pool', 'general_sum_pool',
 
-  'GeneralPoolLayer', 'GeneralMaxPoolLayer', 'GeneralMeanPoolLayer',
-  'general_max_pool', 'general_mean_pool',
+  'BatchPoolLayer', 'MaxBatchPoolLayer', 'MeanBatchPoolLayer', 'SumBatchPoolLayer',
+  'max_batch_pool', 'mean_batch_pool', 'sum_batch_pool',
 
-  'BatchPool', 'MaxBatchPool', 'MeanBatchPool',
-  'max_batch_pool', 'mean_batch_pool'
+  'CumSumLayer', 'cumsum'
 ]
 
+
 class ConstInput(InputLayer):
   def __init__(self, const, name=None):
-    self.value = tf.constant(const)
+    self.value = jnp.array(const)
     super(ConstInput, self).__init__(shape=const.shape, name=name)
 
   def get_output_for(self):
     return self.value
 
-const_input = model_from(ConstInput)()
+class const_input(LayerModel):
+  LayerType = ConstInput
+
+  def __init__(self, const, name=None):
+    super().__init__(const, name=name)
 
 
 _default_shape_f = lambda *input_shapes: input_shapes[0]
 
 class CustomLayer(Layer):
-  def __init__(self, f, shape_f=_default_shape_f, *incoming, name=None):
-    super(CustomLayer, self).__init__(*incoming, name=name)
+  def __init__(self, *incoming, f, shape_f=_default_shape_f, name=None):
     self.f = f
     self.shape_f = shape_f
 
+    super(CustomLayer, self).__init__(*incoming, name=name)
+
   def get_output_for(self, *inputs):
     return self.f(*inputs)
 
   def get_output_shape_for(self, *input_shapes):
     return self.shape_f(*input_shapes)
 
-custom_layer = model_from(CustomLayer)()
+class custom_layer(LayerModel):
+  LayerType = CustomLayer
+
+  def __init__(self, f, shape_f=_default_shape_f, name=None):
+    super().__init__(f, shape_f=shape_f, name=name)
 
 
 class FunctionLayer(Layer):
-  def __init__(self, f, *incoming, name=None):
+  def __init__(self, *incoming, f, name=None):
     if name is None:
       name = f.__name__
 
-    super(FunctionLayer, self).__init__(*incoming, name=name)
-
     self.f = f
 
+    super(FunctionLayer, self).__init__(*incoming, name=name)
+
   def get_output_for(self, *incoming):
     return self.f(*incoming)
 
   def get_output_shape_for(self, *input_shapes):
     return input_shapes[0]
 
-custom = model_from(FunctionLayer)()
-nonlinearity = custom
+class function_layer(LayerModel):
+  LayerType = FunctionLayer
+
+  def __init__(self, f, name=None):
+    super().__init__(f, name=name)
 
 
 class ConcatLayer(Layer):
   def __init__(self, *incoming, axis=-1, name=None):
     assert len(incoming) > 0
     self.axis = axis
 
     super(ConcatLayer, self).__init__(*incoming, name=name)
 
   def get_output_for(self, *inputs):
-    return tf.concat(values=inputs, axis=self.axis, name=str(self) + '_concat')
+    return jnp.concatenate(inputs, axis=self.axis)
 
   def get_output_shape_for(self, *input_shapes):
+    from ..utils.axes import normalize_axis
+
     first = input_shapes[0]
-    axis = (self.axis + len(first)) % len(first)
+    axis = normalize_axis(first, self.axis)
+
+    def gsum(xs):
+      total = 0
+      for x in xs:
+        if x is None:
+          return None
+        else:
+          total += x
+
+      return total
 
     return tuple(
-      first[i] if i != axis else sum(s[i] for s in input_shapes)
+      first[i] if i != axis else gsum(s[i] for s in input_shapes)
       for i in range(len(first))
     )
 
-concat = model_from(ConcatLayer)()
+class concat(LayerModel):
+  LayerType = ConcatLayer
+
+  def __init__(self, axis: int=-1, name=None):
+    super().__init__(axis=axis, name=name)
 
 
 from functools import reduce as _reduce
 
 class FlattenLayer(Layer):
   def __init__(self, incoming, outdim=2, name=None):
     self.outdim = outdim
 
     super(FlattenLayer, self).__init__(incoming, name=name)
 
   def get_output_for(self, incoming):
-    in_shape = tf.shape(incoming)
-
-    out_shape = tf.stack([
-      in_shape[i] for i in range(self.outdim - 1)
-    ] + [
-      tf.reduce_prod(in_shape[self.outdim - 1:])
-    ])
-
-    return tf.reshape(incoming, out_shape)
+    keep = self.outdim - 1
+    return jnp.reshape(incoming, newshape=(*incoming.shape[:keep], -1))
 
   def get_output_shape_for(self, input_shapes):
-    return input_shapes[:self.outdim - 1] + (
+    keep = self.outdim - 1
+    return (
+      *input_shapes[:keep],
       _reduce(
         lambda a, b: a * b if a is not None and b is not None else None,
         input_shapes[self.outdim - 1:],
         1
       ),
     )
 
-flatten = model_from(FlattenLayer)()
+class flatten(LayerModel):
+  LayerType = FlattenLayer
+
+  def __init__(self, outdim: int=2, name=None):
+    super().__init__(outdim=outdim, name=name)
 
 
 class ReshapeLayer(Layer):
   def __init__(self, incoming, new_shape, name=None):
 
     assert len([dim for dim in new_shape if (dim is None or dim < 0)]) < 2, 'ambiguous new shape'
 
@@ -143,263 +175,371 @@
       (-1 if s is None else s)
       for s in new_shape
     )
 
     super(ReshapeLayer, self).__init__(incoming, name=name)
 
   def get_output_for(self, incoming):
-    return tf.reshape(incoming, self.new_shape, name=str(self) + '_reshape')
+    return jnp.reshape(incoming, self.new_shape)
 
   def get_output_shape_for(self, input_shape):
     import numpy as np
 
     if -1 in self.new_shape:
       if all(dim is not None for dim in input_shape):
-        total = np.prod(input_shape, dtype='int64')
+        total = math.prod(input_shape)
         known_dims = np.prod([ dim for dim in self.new_shape if dim is not None], dtype='int64')
         assert total % known_dims == 0, 'can not broadcast %s into %s' % (input_shape, self.new_shape)
         inferred = total // known_dims
 
         return tuple(dim if dim is not None else inferred for dim in self.new_shape)
 
       else:
         return tuple(dim if dim >= 0 else None for dim in self.new_shape)
 
     else:
       return self.new_shape
 
-reshape = model_from(ReshapeLayer)()
-
-
-class TransposeLayer(Layer):
-  def __init__(self, incoming, perm, name=None):
-    super(TransposeLayer, self).__init__(incoming, name=name)
-    self.perm = perm
+class reshape(LayerModel):
+  LayerType = ReshapeLayer
 
-  def get_output_shape_for(self, input_shape):
-    return tuple(input_shape[i] for i in self.perm)
-
-  def get_output_for(self, input):
-    return tf.transpose(input, perm=self.perm)
-
-transpose = model_from(TransposeLayer)()
+  def __init__(self, new_shape: tuple[int, ...], name=None):
+    super().__init__(new_shape, name=name)
 
 
 class ExpandLayer(Layer):
   def __init__(self, incoming, item, name=None):
+    super(ExpandLayer, self).__init__(incoming, name=name)
+
     assert all(
-      it == slice(None, None, None) or it is None
-      for it in item
+      dim == slice(None, None, None) or (isinstance(dim, int) and dim > 0)
+      for dim in item
     )
     self.item = item
 
-    super(ExpandLayer, self).__init__(incoming, name=name)
-
   def get_output_shape_for(self, input_shape):
-    result = list()
-    input_shape_indx = 0
-
-    for i, it in enumerate(self.item):
-      if it is None:
-        result.append(1)
-      else:
-        result.append(input_shape[input_shape_indx])
-        input_shape_indx += 1
-
-    return tuple(result)
+    return tuple(
+      dim if s == slice(None, None, None) else s
+      for dim, s in zip(input_shape, self.item)
+    )
 
   def get_output_for(self, input):
-    return input[self.item]
+    shape = tuple(
+      dim if s == slice(None, None, None) else s
+      for dim, s in zip(input.shape, self.item)
+    )
+    return jnp.broadcast_to(input, shape)
+
+class _expand(LayerModel):
+  LayerType = ExpandLayer
 
-_expand = model_from(ExpandLayer)()
+  def __init__(self, item, name=None):
+    super().__init__(item, name=name)
 
-class ExpandConstructor(object):
+class ExpandExpression(object):
   def __call__(self, item, name=None):
     return _expand(item, name=name)
 
   def __getitem__(self, item):
     return _expand(item)
 
-expand = ExpandConstructor()
+expand = ExpandExpression()
 
 
-class RepeatLayer(Layer):
-  def __init__(self, incoming, repeats, axis=1, name=None):
-    self.repeats = repeats
+class ExpandConcatLayer(Layer):
+  def __init__(self, *incoming, axis=-1, name=None):
     self.axis = axis
 
-    super(RepeatLayer, self).__init__(incoming, name=name)
+    super(ExpandConcatLayer, self).__init__(*incoming, name=name)
 
-  def get_output_for(self, input):
-    expanded = tf.expand_dims(input, axis=self.axis)
-    return tf.repeat(expanded, [self.repeats], axis=self.axis)
+  def get_output_shape_for(self, *input_shapes):
+    axis = normalize_axis(len(input_shapes[0]), self.axis)
 
-  def get_output_shape_for(self, input_shape):
-    return input_shape[:self.axis] + (self.repeats, ) + input_shape[self.axis:]
+    def get_shape(dims, i):
+      if i == axis:
+        if any(dim is None for dim in dims):
+          return None
+        else:
+          return sum(dims)
+
+      concrete_dims = [d for d in dims if d is not None]
+      if len(concrete_dims) > 0:
+        return max(concrete_dims)
+      else:
+        return None
 
-repeat = model_from(RepeatLayer)()
+    return tuple(
+      get_shape(dims, i)
+      for i, dims in enumerate(zip(*input_shapes))
+    )
 
+  def get_output_for(self, *inputs):
+    axis = normalize_axis(inputs[0].ndim, self.axis)
 
-class BroadcastConcatLayer(Layer):
-  def __init__(self, *incoming, axis=-1, name=None):
-    from .meta import get_output_shape
+    shape = tuple(
+      max(dims) if i != axis else None
+      for i, dims in enumerate(zip(*(x.shape for x in inputs)))
+    )
 
-    assert len(incoming) > 0
-    self.axis = axis
-    self.ndim = len(get_output_shape(incoming[0]))
+    return jnp.concatenate([
+      jnp.broadcast_to(
+        x,
+        tuple(s if s is not None else x.shape[i] for i, s, in enumerate(shape))
+      ) for x in inputs
+    ], axis=self.axis)
+
+class expand_concat(LayerModel):
+  LayerType = ExpandConcatLayer
+
+  def __init__(self, axis=-1, name=None):
+    super().__init__(axis=axis, name=name)
+
+
+class BroadcastLayer(Layer):
+  def __init__(self, incoming, broadcast_spec, name=None):
+    self.broadcast_spec = broadcast_spec
+    super(BroadcastLayer, self).__init__(incoming, name=name)
 
-    super(BroadcastConcatLayer, self).__init__(*incoming, name=name)
+  def get_output_for(self, X):
+    return X[self.broadcast_spec]
 
-  def get_output_for(self, *inputs):
-    from ..utils import normalize_axis
-    if len(inputs) == 1:
-      return inputs[0]
-
-    original, rest = inputs[0], inputs[1:]
-    shape = tf.shape(original)
-
-    normalized_axis = normalize_axis(original, self.axis)
-
-    broadcasted = [original]
-    for x in rest:
-      x_shape = tf.shape(x)
-      new_shape = tuple(
-        (x_shape[axis] if axis == normalized_axis else shape[axis])
-        for axis in range(self.ndim)
-      )
-      broadcasted.append(tf.broadcast_to(x, shape=new_shape))
+  def get_output_shape_for(self, input_shape):
+    output_shape = []
+    current_axis = 0
 
-    return tf.concat(broadcasted, axis=normalized_axis)
+    for b in self.broadcast_spec:
+      if b is None:
+        output_shape.append(None)
+      else:
+        output_shape.append(input_shape[current_axis])
+        current_axis += 1
 
-  def get_output_shape_for(self, *input_shapes):
-    from ..utils import normalize_axis, gsum
-    if len(input_shapes) == 1:
-      return input_shapes
+    output_shape.extend(input_shape[current_axis:])
+    return tuple(output_shape)
 
-    original, rest = input_shapes[0], input_shapes[1:]
-    normalized_axis = normalize_axis(original, self.axis)
+class _broadcast(LayerModel):
+  LayerType = BroadcastLayer
 
-    return tuple(
-      gsum(shape[i] for shape in input_shapes)if i == normalized_axis else original[i]
-      for i in range(len(original))
-    )
+  def __init__(self, broadcasting, name=None):
+    super(_broadcast, self).__init__(broadcasting, name=name)
+
+class BroadcastExpression(object):
+  def __getitem__(self, item):
+    return _broadcast(item)
 
-broadcast_concat = model_from(BroadcastConcatLayer)()
+broadcast = BroadcastExpression()
 
 
 class ElementwiseLayer(Layer):
-  def __init__(self, *incoming, op, name=None):
+  @staticmethod
+  def operator(*inputs):
+    raise NotImplementedError()
+
+  def __init__(self, *incoming, name=None):
     super(ElementwiseLayer, self).__init__(*incoming, name=name)
-    self.op = op
 
   def get_output_for(self, *inputs):
-    return self.op(*inputs)
+    return self.operator(*inputs)
 
   def get_output_shape_for(self, *input_shapes):
-    for shape in input_shapes[1:]:
-      if tuple(shape) != tuple(input_shapes[0]):
-        raise ValueError('An elementwise operation requires all input shapes to be the same!')
-
     return input_shapes[0]
 
-elementwise = model_from(ElementwiseLayer)()
-
-
-ElementwiseSumLayer = derive('ElementwiseSumLayer').based_on(ElementwiseLayer).with_fixed(
-  op=lambda *inputs: sum(inputs)
-)
-elementwise_sum = model_from(ElementwiseSumLayer)()
-
-ElementwiseMeanLayer = derive('ElementwiseMeanLayer').based_on(ElementwiseLayer).with_fixed(
-  op=lambda *inputs: sum(inputs) / len(inputs)
-)
-elementwise_mean = model_from(ElementwiseMeanLayer)()
-
-from functools import reduce
-
-ElementwiseMaxLayer = derive('ElementwiseMaxLayer').based_on(ElementwiseLayer).with_fixed(
-  op=lambda *inputs: reduce(tf.maximum, inputs)
-)
-elementwise_max = model_from(ElementwiseMaxLayer)()
-
-ElementwiseMinLayer = derive('ElementwiseMinLayer').based_on(ElementwiseLayer).with_fixed(
-  op=lambda *inputs: reduce(tf.minimum, inputs)
-)
-elementwise_min = model_from(ElementwiseMinLayer)()
-
+class elementwise(LayerModel):
+  def __init__(self, name=None):
+    super().__init__(name)
+
+
+class ElementwiseSumLayer(ElementwiseLayer):
+  @staticmethod
+  def operator(*inputs):
+    return functools.reduce(lambda a, b: a + b, inputs)
+
+class elementwise_sum(elementwise):
+  LayerType = ElementwiseSumLayer
+
+class ElementwiseMeanLayer(ElementwiseLayer):
+  @staticmethod
+  def operator(*inputs):
+    return ElementwiseSumLayer.operator(*inputs) / len(inputs)
+
+class elementwise_mean(elementwise):
+  LayerType = ElementwiseMeanLayer
+
+class ElementwiseMaxLayer(ElementwiseLayer):
+  @staticmethod
+  def operator(*inputs):
+    return functools.reduce(lambda a, b: jnp.maximum(a, b), inputs)
+
+class elementwise_max(elementwise):
+  LayerType = ElementwiseMaxLayer
+
+class ElementwiseMinLayer(ElementwiseLayer):
+  @staticmethod
+  def operator(*inputs):
+    return functools.reduce(lambda a, b: jnp.minimum(a, b), inputs)
+
+class elementwise_min(elementwise):
+  LayerType = ElementwiseMinLayer
+
+class ElementwiseSoftmaxLayer(ElementwiseLayer):
+  @staticmethod
+  def operator(alpha, *inputs):
+    return soft_maximum(alpha, *inputs)
+
+  def __init__(self, *incoming, alpha=constant_parameter(1.0), name=None):
+    super(ElementwiseLayer, self).__init__(
+      *incoming,
+      parameters=(
+        alpha(shape=()),
+      ),
+      name=name
+    )
 
-class SquareDifference(Layer):
-  def __init__(self, incoming1, incoming2, axes=None, name=None):
-    from .meta import get_output_shape
+class elementwise_softmax(LayerModel):
+  LayerType = ElementwiseSoftmaxLayer
 
-    if axes is None:
-      shape = get_output_shape(incoming1)
-      self.axes = list(range(len(shape)))[1:]
-    else:
-      self.axes = axes
+  def __init__(self, alpha=constant_parameter(1.0), name=None):
+    super().__init__(alpha=alpha, name=name)
 
-    super(SquareDifference, self).__init__(incoming1, incoming2, name=name)
-
-  def get_output_for(self, input1, input2):
-    return tf.reduce_mean(
-      (input1 - input2) ** 2,
-      axis=self.axes
+class ElementwiseSoftminLayer(ElementwiseLayer):
+  @staticmethod
+  def operator(alpha, *inputs):
+    return soft_minimum(alpha, *inputs)
+
+  def __init__(self, *incoming, alpha=constant_parameter(1.0), name=None):
+    super(ElementwiseLayer, self).__init__(
+      *incoming,
+      parameters=(
+        alpha(shape=()),
+      ),
+      name=name
     )
 
-  def get_output_shape_for(self, shape1, shape2):
-    return tuple(
-      s for i, s in enumerate(shape1)
-      if i not in self.axes
-    )
+class elementwise_softmin(LayerModel):
+  LayerType = ElementwiseSoftminLayer
 
-square_difference = model_from(SquareDifference, incoming_args=['incoming1', 'incoming2'])()
+  def __init__(self, alpha=constant_parameter(1.0), name=None):
+    super().__init__(alpha=alpha, name=name)
 
 
 class GeneralPoolLayer(Layer):
-  def __init__(self, incoming, op, axis=(-1, ), name=None):
-    super(GeneralPoolLayer, self).__init__(incoming, name=name)
-    self.op = op
-    if isinstance(axis, int):
-      axis = (axis, )
+  @staticmethod
+  def operator(xs, axis):
+    raise NotImplementedError()
 
-    self.axis = axis
+  def __init__(self, incoming, axis=(-1, ), name=None):
+    self.axis = (axis, ) if isinstance(axis, int) else axis
+    super(GeneralPoolLayer, self).__init__(incoming, name=name)
 
-  def get_output_for(self, input):
-    return self.op(input, axis=self.axis, keepdims=False)
+  def get_output_for(self, X):
+    return self.operator(X, axis=self.axis)
 
   def get_output_shape_for(self, input_shape):
+    from ..utils.axes import normalize_axis
     normalized_axis = tuple(
-      (ax + len(input_shape)) % len(input_shape)
+      normalize_axis(input_shape, ax)
       for ax in self.axis
     )
 
     return tuple(
       dim
       for axis, dim in enumerate(input_shape)
       if axis not in normalized_axis
     )
 
-GeneralMaxPoolLayer = derive('GeneralMaxPoolLayer').based_on(GeneralPoolLayer).with_fixed(op=tf.reduce_max)
-GeneralMeanPoolLayer = derive('GeneralMeanPoolLayer').based_on(GeneralPoolLayer).with_fixed(op=tf.reduce_mean)
+class GeneralPoolModel(LayerModel):
+  def __init__(self, axis=(-1, ), name=None):
+    super().__init__(axis=axis, name=name)
+
+class GeneralMaxPoolLayer(GeneralPoolLayer):
+  @staticmethod
+  def operator(xs, axis):
+    return jnp.max(xs, axis=axis)
+
+class GeneralMinPoolLayer(GeneralPoolLayer):
+  @staticmethod
+  def operator(xs, axis):
+    return jnp.min(xs, axis=axis)
+
+class GeneralMeanPoolLayer(GeneralPoolLayer):
+  @staticmethod
+  def operator(xs, axis):
+    return jnp.mean(xs, axis=axis)
+
+class GeneralSumPoolLayer(GeneralPoolLayer):
+  @staticmethod
+  def operator(xs, axis):
+    return jnp.sum(xs, axis=axis)
+
+class general_max_pool(GeneralPoolModel):
+  LayerType = GeneralMaxPoolLayer
+
+class general_min_pool(GeneralPoolModel):
+  LayerType = GeneralMinPoolLayer
+
+class general_mean_pool(GeneralPoolModel):
+  LayerType = GeneralMeanPoolLayer
+
+class general_sum_pool(GeneralPoolModel):
+  LayerType = GeneralSumPoolLayer
+
+
+class BatchPoolLayer(Layer):
+  @staticmethod
+  def operator(X, axis):
+    raise NotImplementedError()
 
-general_max_pool = model_from(GeneralMaxPoolLayer)()
-general_mean_pool = model_from(GeneralMeanPoolLayer)()
+  def __init__(self, incoming, axis=(0, ), name=None):
+    super(BatchPoolLayer, self).__init__(incoming, name=name)
+    self.axis = axis
 
+  def get_output_shape_for(self, input_shape):
+    return input_shape
 
-class BatchPool(Layer):
-  def __init__(self, incoming, op, axis=(0, )):
-    super(BatchPool, self).__init__(incoming)
+  def get_output_for(self, X):
+    averaged = self.operator(X, axis=self.axis)
+    return jnp.broadcast_to(averaged, shape=X.shape)
+
+class BatchPoolLayerModel(LayerModel):
+  def __init__(self, axis=-2, name=None):
+    super().__init__(axis=axis, name=name)
+
+class MeanBatchPoolLayer(BatchPoolLayer):
+  @staticmethod
+  def operator(X, axis):
+    return jnp.mean(X, axis=axis, keepdims=True)
+
+class SumBatchPoolLayer(BatchPoolLayer):
+  @staticmethod
+  def operator(X, axis):
+    return jnp.sum(X, axis=axis, keepdims=True)
+
+class MaxBatchPoolLayer(BatchPoolLayer):
+  @staticmethod
+  def operator(X, axis):
+    return jnp.max(X, axis=axis, keepdims=True)
+
+class mean_batch_pool(BatchPoolLayerModel):
+  LayerType = MeanBatchPoolLayer
+
+class sum_batch_pool(BatchPoolLayerModel):
+  LayerType = SumBatchPoolLayer
+
+class max_batch_pool(BatchPoolLayerModel):
+  LayerType = MaxBatchPoolLayer
+
+class CumSumLayer(Layer):
+  def __init__(self, incoming, axis=-2, name=None):
+    super(CumSumLayer, self).__init__(incoming, name=name)
     self.axis = axis
-    self.op = op
 
   def get_output_shape_for(self, input_shape):
     return input_shape
 
-  def get_output_for(self, input):
-    averaged = self.op(input, axis=self.axis, keepdims=True)
-    return tf.broadcast_to(averaged, shape=tf.shape(input))
+  def get_output_for(self, X):
+    return jnp.cumsum(X, axis=self.axis)
 
-MeanBatchPool = derive('MeanBatchPool').based_on(BatchPool).with_fixed(op=tf.reduce_mean)
-MaxBatchPool = derive('MaxBatchPool').based_on(BatchPool).with_fixed(op=tf.reduce_max)
+class cumsum(LayerModel):
+  LayerType = CumSumLayer
 
-mean_batch_pool = model_from(MeanBatchPool)()
-max_batch_pool = model_from(MaxBatchPool)()
+  def __init__(self, axis=-2, name=None):
+    super().__init__(axis=axis, name=name)
```

### Comparing `craynn-0.3.2/craynn/layers/dense_ops.py` & `craynn-0.4.0/craynn/layers/dense_ops.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import tensorflow as tf
+import jax.numpy as jnp
 
+from .. import dag
 from ..nonlinearities import default_semibounded_nonlinearity
 from ..parameters import default_weight_init, default_bias_init
 
-from .meta import Layer, get_output_shape, model_from
+from .meta import Layer, LayerModel, LayerSignature
 
 __all__ = [
   'DenseLayer',
   'dense',
 
   'TensorDenseLayer',
   'tensor_dense',
-
-  'BatchDenseLayer',
-  'batch_dense',
 ]
 
 class DenseLayer(Layer):
-  def __init__(self, incoming, num_units,
-               activation=default_semibounded_nonlinearity,
-               W=default_weight_init,
-               b=default_bias_init,
-               name=None):
+  def __init__(
+    self, incoming, num_units,
+    activation=default_semibounded_nonlinearity,
+    W=default_weight_init,
+    b=default_bias_init,
+    name=None
+  ):
     """
     Dense (also called fully-connected) layer.
     Dense layer consists of `num_units` units, each of which takes
     weighted sum of inputs and applies `activation` function. In matrix form:
         f(X `dot` W + b)
     where:
       - W --- a weight matrix of size `(input_dim, num_units)`;
@@ -37,55 +37,76 @@
     :param incoming: incoming layer;
     :param num_units: number of output units;
     :param activation: activation function `f`;
     :param W: weight matrix, parameter with default properties `weights=True`, `trainable=True`;
     :param b: bias vector, parameter with default properties `biases=True`, `trainable=True`;
     :param name: name for the layer.
     """
-    input_shape = get_output_shape(incoming)
+    input_shape = dag.get_output_shape(incoming)
     self.num_units = num_units
 
     if len(input_shape) < 2:
-      raise ValueError('Dense layer accepts only tensors of dimensionality higher than 2 [got %s]!' % (input_shape, ))
+      raise ValueError(
+        'Dense layer accepts only tensors of dimensionality higher than or equal to 2 [got %s]!' % (input_shape, )
+      )
 
     self.activation = activation
 
+    self.W = W(
+      shape=(input_shape[-1], num_units),
+      name='W', weights=True, trainable=True
+    )
+    self.b = b(
+      shape=(num_units,),
+      name='b', biases=True, trainable=True
+    )
+
     super(DenseLayer, self).__init__(
       incoming,
       name=name,
-      parameters=(
-        W(shape=(input_shape[-1], num_units), name='W', weights=True, trainable=True),
-        b(shape=(num_units,), name='b', biases=True, trainable=True)
-      )
+      parameters=(self.W, self.b)
     )
 
-  def get_output_for(self, W, b, input):
-    b_broadcast = tuple(None for _ in input.shape[:-1]) + (slice(None, None, None), )
-
+  def get_output_for(self, W, b, X):
     return self.activation(
-      tf.matmul(input, W) + b[b_broadcast]
+      jnp.matmul(X, W) + b
     )
 
-  def get_output_shape_for(self, W_shape, b_shape, input_shape):
-    if len(input_shape) < 2:
+  def get_output_shape_for(self, W_shape, b_shape, X_shape):
+    if len(X_shape) < 2:
       raise ValueError('Dense layer accepts only 2+ dimensional tensors!')
 
-    return input_shape[:-1] + (self.num_units, )
+    return X_shape[:-1] + (self.num_units,  )
 
-dense = model_from(DenseLayer).with_fixed().with_defaults()()
-meta_dense = model_from(DenseLayer, incoming_args=('incoming', 'W', 'b')).with_fixed().with_defaults()()
+  def signature(self) -> LayerSignature:
+    return (
+      ('I', ),
+      ('IO', 'O'),
+      'O'
+    )
+
+class dense(LayerModel):
+  LayerType = DenseLayer
+
+  def __init__(
+    self, num_units,
+    activation=default_semibounded_nonlinearity,
+    W=default_weight_init, b=default_bias_init,
+    name=None
+  ):
+    super().__init__(num_units, activation=activation, W=W, b=b, name=name)
 
 class TensorDenseLayer(Layer):
   def __init__(self, incoming, num_units,
                activation=default_semibounded_nonlinearity,
                W=default_weight_init,
                b=default_bias_init,
                axis=-1,
                name=None):
-    input_shape = get_output_shape(incoming)
+    input_shape = dag.get_output_shape(incoming)
     self.num_units = num_units
     self.axis = (len(input_shape) + axis) % len(input_shape)
 
     self.b_broadcast = tuple(
       (None if i != self.axis else slice(None, None, None))
       for i in range(len(input_shape))
     )
@@ -98,66 +119,32 @@
       parameters=(
         W(shape=(input_shape[self.axis], num_units), name='W', weights=True, trainable=True),
         b(shape=(num_units,), name='b', biases=True, trainable=True)
       ),
     )
 
   def get_output_for(self, W, b, input):
-    return self.activation(
-      tf.tensordot(input, W, axes=[(self.axis, ), (0, )]) + b[self.b_broadcast]
+    product = jnp.transpose(
+      jnp.tensordot(input, W, axes=[(self.axis, ), (0, )]),
+      axes=(*range(self.axis, ), -1, *range(self.axis, input.ndim - 1))
     )
 
+    return self.activation(product + b[self.b_broadcast])
+
   def get_output_shape_for(self, W_shape, b_shape, input_shape):
     return tuple([
       (input_shape[i] if i != self.axis else self.num_units)
       for i in range(len(input_shape))
     ])
 
-tensor_dense = model_from(TensorDenseLayer).with_fixed().with_defaults()()
-
-
-class BatchDenseLayer(Layer):
-  def __init__(self, incoming, num_units, num_batches=None,
-               activation=default_semibounded_nonlinearity,
-               W=default_weight_init,
-               b=default_bias_init,
-               name=None):
-    input_shape = get_output_shape(incoming)
-
-    if num_batches is None:
-      if len(input_shape) < 3:
-        raise Exception('Please specify number of batches for the batch dense layer')
-
-      self.num_batches = input_shape[0]
-    else:
-      self.num_batches = num_batches
-
-    self.num_units = num_units
-    self.in_units = input_shape[-1]
-
-    self.activation = activation
-
-    self.W = W(shape=(self.num_batches, self.in_units, num_units), name='W', weights=True, trainable=True)
-    self.b = b(shape=(self.num_batches, num_units,), name='b', biases=True, trainable=True)
-
-    super(BatchDenseLayer, self).__init__(
-      incoming,
-      name=name,
-      parameters=(self.W, self.b)
-    )
-
-  def get_output_for(self, W, b, input):
-    return self.activation(
-      tf.matmul(input, W) + b[:, None, :]
-    )
-
-  def get_output_shape_for(self, W_shape, b_shape, input_shape):
-    if len(input_shape) == 3:
-      return (
-        self.num_batches, input_shape[1], self.num_units
-      )
-    else:
-      return (
-        self.num_batches, input_shape[0], self.num_units
-      )
+class tensor_dense(LayerModel):
+  LayerType = TensorDenseLayer
 
-batch_dense = model_from(BatchDenseLayer).with_fixed().with_defaults()()
+  def __init__(
+    self, num_units,
+    activation=default_semibounded_nonlinearity,
+    W=default_weight_init,
+    b=default_bias_init,
+    axis=-1,
+    name=None
+  ):
+    super().__init__(num_units, activation=activation, W=W, b=b, axis=axis, name=name)
```

### Comparing `craynn-0.3.2/craynn/layers/noise_ops.py` & `craynn-0.4.0/craynn/layers/noise_ops.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,113 @@
-import tensorflow as tf
+import jax
+import jax.numpy as jnp
 
-from craygraph import derive
-from .meta import Layer, model_from, get_output_shape
+from .meta import Layer, LayerModel
 
 __all__ = [
-  'NoiseLayer', 'noise',
+  'NoiseLayer', 'NoiseLayerModel',
   'GaussianNoiseLayer', 'gaussian_noise',
 
-  'GaussianRandomVariableLayer', 'gaussian_rv',
-  'DropoutLayer', 'dropout'
+  'DropoutLayer', 'dropout',
+  'RandomExpScalingLayer', 'random_exp_scaling',
+  'RandomLogNormScalingLayer', 'random_lognorm_scaling'
 ]
 
 class NoiseLayer(Layer):
-  def __init__(self, incoming, noise_op, scale=1.0e-3, name=None):
-    self.noise_op = noise_op
-    self.scale = tf.constant(scale, dtype=tf.float32)
+  def operator(self, X: jax.Array, rng: jax.Array):
+    raise NotImplementedError()
+
+  def __init__(self, incoming, scale: float=1.0e-2, name=None):
+    self.scale = scale
 
     super(NoiseLayer, self).__init__(incoming, name=name)
 
-  def get_output_for(self, input, deterministic=False):
-    if deterministic:
-      return input
+  def get_output_for(self, X, rng: jax.Array | None=None):
+    if rng is None:
+      return X
     else:
-      return input + self.noise_op(shape=tf.shape(input), dtype=input.dtype) * self.scale
+      return X + self.scale * self.operator(X, rng)
 
   def get_output_shape_for(self, input_shape):
     return input_shape
 
+class NoiseLayerModel(LayerModel):
+  def __init__(self, scale: float=1.0e-3, name=None):
+    super().__init__(scale=scale, name=name)
+
+
+class GaussianNoiseLayer(NoiseLayer):
+  def operator(self, X: jax.Array, rng: jax.Array):
+    return X + self.scale * jax.random.normal(rng, shape=X.shape, dtype=X.dtype)
 
-noise = model_from(NoiseLayer)()
+class gaussian_noise(NoiseLayerModel):
+  LayerType = GaussianNoiseLayer
 
-GaussianNoiseLayer = derive('GaussianNoiseLayer').based_on(NoiseLayer).with_fixed(noise_op=tf.random.normal)
-gaussian_noise = model_from(GaussianNoiseLayer)()
 
 class DropoutLayer(Layer):
   def __init__(self, incoming, p=0.2, name=None):
     self.p = p
 
     super(DropoutLayer, self).__init__(incoming, name=name)
 
-  def get_output_for(self, input, deterministic=False):
-    if deterministic:
-      return input
+  def get_output_for(self, X, rng=None):
+    if rng is None:
+      return X
     else:
-      return tf.nn.dropout(input, rate=self.p, noise_shape=None, name=self.name())
+      mask = jax.random.bernoulli(rng, shape=X.shape, p=1 - self.p)
+      return mask * X / (1 - self.p)
 
   def get_output_shape_for(self, input_shape):
     return input_shape
 
-dropout = model_from(DropoutLayer)()
+class dropout(LayerModel):
+  LayerType = DropoutLayer
+
+  def __init__(self, p: float=0.2, name=None):
+    super().__init__(p=p, name=name)
+
+
+class RandomExpScalingLayer(Layer):
+  def __init__(self, incoming, name=None):
+    super(RandomExpScalingLayer, self).__init__(incoming, name=name)
 
+  def get_output_for(self, X, rng: jax.Array | None=None):
+    if rng is None:
+      return X
+    else:
+      mask = jax.random.exponential(rng, shape=X.shape, dtype=X.dtype)
+      ### mean of exp is 1
+      return mask * X
+
+  def get_output_shape_for(self, input_shape):
+    return input_shape
 
-class GaussianRandomVariableLayer(Layer):
-  def __init__(self, *incoming, name=None):
-    assert len(incoming) == 2
+class random_exp_scaling(LayerModel):
+  LayerType = RandomExpScalingLayer
 
-    super(GaussianRandomVariableLayer, self).__init__(*incoming, name=name)
+  def __init__(self, name=None):
+    super().__init__(name=name)
 
-  def get_output_for(self, mean, std, deterministic=False):
-    if deterministic:
-      return mean
+class RandomLogNormScalingLayer(Layer):
+  def __init__(self, incoming, sigma: float=1.0, name=None):
+    import math
+
+    self.sigma = sigma
+    self.mean = math.exp(0.5 * sigma * sigma)
+    super(RandomLogNormScalingLayer, self).__init__(incoming, name=name)
+
+  def get_output_for(self, X, rng: jax.Array | None=None):
+    if rng is None:
+      return X
     else:
-      u = tf.random.normal(shape=tf.shape(mean), dtype=mean.dtype)
-      return u * std + mean
+      mask = jax.random.lognormal(rng, sigma=self.sigma, shape=X.shape, dtype=X.dtype)
+      ### mean of exp is 1
+      return mask * X / self.mean
 
-  def get_output_shape_for(self, *input_shapes):
-    return input_shapes[0]
+  def get_output_shape_for(self, input_shape):
+    return input_shape
 
-gaussian_rv = model_from(GaussianRandomVariableLayer)()
+class random_lognorm_scaling(LayerModel):
+  LayerType = RandomLogNormScalingLayer
 
+  def __init__(self, sigma: float=1.0, name=None):
+    super().__init__(sigma=sigma, name=name)
```

### Comparing `craynn-0.3.2/craynn/networks/meta.py` & `craynn-0.4.0/craynn/networks/meta.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,79 @@
-import tensorflow as tf
+import jax
 
+from .. import dag
 from .. import layers
 from .. import parameters
-from ..subnetworks import achain
 
-from .utils import get_signature, get_named_layers
+from .utils import get_signature, get_named_layers, pdict
 
 __all__ = [
   'Network', 'network',
-  'modify_network'
 ]
 
+
 class Network(object):
   def __init__(self, inputs, outputs, **modes):
     self._inputs = inputs
     self._outputs = outputs
     self._modes = modes
 
     try:
       self.__call__.__signature__ = get_signature(inputs)
     except:
       pass
 
-    self._named_layers = get_named_layers(self.layers())
-    self._mode_cache = dict()
+    all_layers = self.nodes()
+    self._rng_layers = dag.get_mode_nodes(all_layers, mode='rng')
+    self._named_layers = get_named_layers(all_layers)
+    self._free_parameters = parameters.get_all_free_parameters(self.outputs(), )
 
   def outputs(self):
     if isinstance(self._outputs, (list, tuple)):
       return self._outputs
     else:
       return (self._outputs, )
 
   def inputs(self):
     return self._inputs
 
+  def parameters(self, **properties):
+    parameters.get_parameters(self._outputs, **properties)
+
+  def free_parameters(self, **properties):
+    if len(properties) == 0:
+      return self._free_parameters
+    else:
+      check = parameters.check_properties(**properties)
+      return [param for param in self._free_parameters if check(param)]
+
+  def initialize(self, rng, **properties) -> pdict:
+    from .. import train
+    return train.initialize_parameters(rng, self, **properties)
+
+  def normalize(
+    self, key: jax.Array, *args,
+    weights=True, biases=True,
+    learning_rate: float=0.1, iterations: int=128,
+    preactivation: bool=True,
+    batch: int | None = None,
+    progress=None
+  ) -> pdict:
+    from .. import train
+    substitutes = self._map_inputs(args)
+    inputs = {l: v for l, v in substitutes.items() if not isinstance(l, parameters.FreeParameter)}
+    params = {l: v for l, v in substitutes.items() if isinstance(l, parameters.FreeParameter)}
+
+    return train.normalize_parameters(
+      key, self, inputs, params, weights=weights, biases=biases,
+      learning_rate=learning_rate, iterations=iterations,
+      preactivation=preactivation, batch=batch, progress=progress
+    )
+
+
   def find_layer(self, layer_or_name):
     if isinstance(layer_or_name, str):
       return self._named_layers[layer_or_name]
     elif isinstance(layer_or_name, layers.Layer):
       return layer_or_name
     else:
       raise Exception("%s is not a layer or a layer's name" % (layer_or_name, ))
@@ -55,136 +91,157 @@
     inputs = self._inputs if inputs is None else self.find_layers(inputs)
     inputs = inputs if isinstance(inputs, (list, tuple)) else (inputs, )
 
     outputs = self._outputs if outputs is None else self.find_layers(outputs)
 
     return Network(inputs, outputs)
 
-  def _as_subnet(self, *incoming):
+  def as_subnet(self, *incoming):
     from ..subnetworks import subnetwork
     return subnetwork(self.inputs(), self.outputs())(*incoming)
 
-  def _map_inputs(self, args, kwargs):
-    substitutes = dict(zip(self.inputs(), args))
+  def _map_parameters(self, values):
+    from ..utils.axes import check_shape_consistency
+
+    if len(values) != len(self._free_parameters):
+      raise ValueError(
+        'number of provided values (%d) does not match number of free parameters (%d)' % (
+          len(values), len(self._free_parameters)
+        )
+      )
+
+    for parameter, value in zip(self._free_parameters, values):
+      if not check_shape_consistency(value.shape, parameter.shape):
+        raise ValueError(
+          'Shape of a value (%s) is not consistent with the shape of the corresponding parameter (%s)' % (
+            value.shape, parameter.shape()
+          )
+        )
+
+    return {
+      parameter: value
+      for parameter, value in zip(self._free_parameters, values)
+    }
+
+  def _map_inputs(self, args):
+    inputs = list()
+    substitutes = dict()
+
+    for arg in args:
+      if isinstance(arg, dict):
+        for l, X in arg.items():
+          if isinstance(l, str):
+            if l not in self._named_layers:
+              raise Exception(f'There is no layer with name {l}')
+            layer = self._named_layers[l]
+
+          elif isinstance(l, dag.Node):
+            layer = l
+
+          else:
+            raise ValueError(
+              f'Input dictionaries only accept str or Nodes (Layers and Parameters) as keys, got {l}.'
+            )
+
+          if layer in substitutes:
+            raise ValueError(f'Two or more values are provided for the layer {l}.')
+
+          substitutes[layer] = X
 
-    for name, value in kwargs.items():
-      if name in self._named_layers:
-        layer = self._named_layers[name]
       else:
-        raise Exception('There is no layer with name %s' % (name,))
+        inputs.append(arg)
 
-      if layer in substitutes:
-        raise Exception('Value for layer %s is provided twice, via a positional and a keyword arguments' % (name,))
+    for input_layer, arg in zip(self.inputs(), args):
+      if input_layer in substitutes:
+        raise ValueError(f'Two or more values are provided for the layer {input_layer}')
 
-      substitutes[layer] = value
+      substitutes[input_layer] = arg
 
     return substitutes
 
-  @tf.function(autograph=False)
-  def __call__(self, *args, **kwargs):
-    is_arg_layer = [isinstance(arg, layers.Layer) for arg in args]
-
-    if all(is_arg_layer) and len(is_arg_layer) > 0:
-      if len(kwargs) != 0:
-        raise Exception('Network as a SubnetworkLayer does not accept kwargs')
-      return self._as_subnet(*args)
+  def __call__(self, *args, rng=None, **kwargs):
+    """
+    Returns result of network evaluation.
+
+    Each element of `*args` must be either a tensor or a dictionary of type layer/parameter -> tensor.
+    Keyword arguments allow to provide "modes" to the layer.
+    Standalone tensors are matched with the network's inputs in the same order as inputs were defined.
+    Dictionaries are directly matched to the corresponding layers/parameters.
+
+    Note that it is not necessary to provide values for all input layers. For instance, for the following network:
+    ```python
+    net = network(x=(None, 2), y=(None, 2))(
+      dense(4, name='z'),
+      dense(2)
+    )
+    params = ...
+    ```
 
-    if any(is_arg_layer) or any([ isinstance(arg, layers.Layer) for arg in kwargs.values() ]):
-      raise NotImplementedError('Network can not be called on a mixture of layers and tensors yet.')
+    `net(params, {'z': jnp.zeros(shape=(3, 4))})` will be properly evaluated since input layers are not required for
+    evaluation of the result. The same principle applies to the free parameters of the network.
 
-    substitutes = self._map_inputs(args, kwargs)
+    :param args: substitutes for layers/parameters: tensors are matched to the network's inputs,
+      dictionaries are mapped directly;
+    :param kwargs: modes for layers.
+    :return: result of the network evaluation.
+    """
+
+    substitutes = self._map_inputs(args)
 
     try:
-      return layers.get_output(self._outputs, substitutes=substitutes, **self._modes)
+      if rng is not None:
+        rng = {
+          layer: dict(rng=v)
+          for layer, v in zip(self._rng_layers, jax.random.split(rng, num=len(self._rng_layers)))
+        }
+      else:
+        rng = None
+
+      return dag.get_output(self._outputs, substitutes=substitutes, individual_kwargs=rng, **self._modes)
 
     except Exception as e:
+      import itertools
       inputs_wo_substitute = [
         layer
-        for layer in self.inputs()
+        for layer in itertools.chain(self.inputs(), self.free_parameters())
         if layer not in substitutes
       ]
 
       if len(inputs_wo_substitute) > 0:
-        raise ValueError('Not all inputs were provided value, this might be the cause of the error.') from e
+        raise ValueError(
+          'Not all inputs were provided value, this might be the cause of the error: %s' % (inputs_wo_substitute, )
+        ) from e
       else:
         raise
 
-  def mode(self, **modes):
-    if len(modes) == 0:
-      return self
-
-    new_modes = self._modes.copy()
-    for k, v in modes.items():
-      new_modes[k] = v
-
-    mode_key = tuple(new_modes.items())
-    if mode_key not in self._mode_cache:
-      self._mode_cache[mode_key] = Network(self._inputs, self._outputs, **new_modes)
-
-    self._mode_cache[mode_key]._mode_cache = self._mode_cache
-
-    return self._mode_cache[mode_key]
-
-
-  def reset(self):
-    return [
-      param.reset()
-      for param in self.parameters()
-    ]
-
-  def parameters(self, **properties):
-    return parameters.get_all_parameters(self.outputs(), **properties)
-
-  def variables(self, trainable=None, **properties):
-    return parameters.get_all_variables(self.outputs(), trainable=trainable, **properties)
-
-  def assign(self, variable_values, trainable=True, **properties):
-    variables = self.variables(trainable=trainable, **properties)
-    assert len(variables) == len(variable_values), \
-      'number of variables is not the same as the number of values (%d vs %d)' % (len(variables), len(variable_values))
-
-    for var, value in zip(variables, variable_values):
-      var.assign(value)
-
   def description(self, short=True, **attributes):
     from craynn.info.layers import graph_description
     return graph_description(self.outputs(), short=short, inputs=self.inputs(), **attributes)
 
   def __str__(self):
     return self.description(short=True)
 
   def __repr__(self):
     return self.description(short=True)
 
   def total_number_of_parameters(self):
     from ..info.layers import get_total_number_of_parameters
     return get_total_number_of_parameters(self.outputs())
 
+  def nodes(self):
+    return dag.get_nodes(self.outputs())
+
   def layers(self):
     return layers.get_layers(self.outputs())
 
   def input_shapes(self):
-    return layers.get_output_shape(self.inputs())
+    return dag.get_output_shape(self.inputs())
 
   def output_shapes(self):
-    return layers.get_output_shape(self.outputs())
-
-  def reg_l2(self, weights=True, **properties):
-    from ..regularization import apply_regularization, reg_l2
-
-    return apply_regularization(
-      self.outputs(), reg_l2(), weights=weights, **properties,
-    )
-
-  def reg_l1(self, weights=True, **properties):
-    from ..regularization import apply_regularization, reg_l1
-
-    return apply_regularization(
-      self.outputs(), reg_l1(), weights=weights, **properties,
-    )
+    return dag.get_output_shape(self.outputs())
 
 
 def __is_shape(shape_or_layer):
   return hasattr(shape_or_layer, '__iter__') and all([ (type(s) is int or s is None) for s in shape_or_layer ])
 
 def _get_input_layer(shape_or_layer, name=None, index=None):
   if __is_shape(shape_or_layer) :
@@ -214,41 +271,27 @@
   assert len(set(explicit_names)) == len(explicit_names)
 
   outputs = factory(*input_layers)
 
   return Network(input_layers, outputs)
 
 
-network = lambda *inputs, **named_inputs: lambda *factory: \
-  _make_network(achain(*factory), inputs, named_inputs)
-
-network.__doc__ = \
-"""
-Allows nice syntax:
-```
-  net(session)(input1, input2, ..., named_input=)(
-    constructor
-  )
-```
-
-or
-
-```
-  net(session)(input)(
-    constructor
-  )
-```
-
-for single input.
-"""
-
-def modify_network(operator, nn : Network):
+def network(*inputs, **named_inputs):
   """
-  Performs `craynn.layers.meta.modify_graph` of network's graph...
-  See `craynn.layers.meta.modify_graph` documentation for details.
-  :param operator: modification operator.
-  :param nn: an instance of Network.
-  :return: modified network.
+  Allows nice syntax:
+  ```
+    net(<shape of input 1>, <shape of input 2>, ..., named_input=<shape of the named_input>)(
+      constructor
+    )
+  ```
+  or
+  ```
+    net(<input shape>)(
+      constructor
+    )
+  ```
+  for single input.
   """
-  import craygraph
-  modified = craygraph.modify_graph(operator, nn.outputs)
-  return nn.__class__(nn.inputs, modified)
+  def constructor(*factory):
+    return _make_network(dag.achain(*factory), inputs, named_inputs)
+
+  return constructor
```

### Comparing `craynn-0.3.2/craynn/parameters/noisy.py` & `craynn-0.4.0/craynn/parameters/noisy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-import tensorflow as tf
+import jax
 
-from .meta import Parameter, parameter_model
+from .meta import Parameter, ParameterModel
 from .defaults import default_weight_init
 
 __all__ = [
   'NoisyParameter', 'noisy_parameter'
 ]
 
 class NoisyParameter(Parameter):
   def __init__(self, shape, eps=1e-3, w=default_weight_init, name=None, **properties):
-    self.eps = tf.constant(eps, dtype=tf.float32, shape=())
+    self.eps = eps
 
     self.w = w(
       shape=shape, **properties,
       name=(name + '_w') if name is not None else None
     )
 
     super(NoisyParameter, self).__init__(
       self.w, shape=shape, name=name,
       **properties
     )
 
-  def get_output_for(self, w, deterministic=False):
-    if deterministic:
+  def get_output_for(self, w, rng: jax.Array):
+    if rng is None:
       return w
     else:
-      return w + tf.random.normal(shape=tf.shape(w), stddev=self.eps, dtype=w.dtype)
+      return w + self.eps * jax.random.normal(rng, shape=w.shape, dtype=w.dtype)
 
   def get_output_shape_for(self, w_shape):
     return w_shape
 
-noisy_parameter = parameter_model(NoisyParameter)()
+class noisy_parameter(ParameterModel):
+  ParameterType = NoisyParameter
+
+  def __init__(self, eps=1e-3, w=default_weight_init, name=None, composite=True, **properties):
+    super().__init__(dict(**properties, composite=composite), eps=eps, w=w, name=name)
```

### Comparing `craynn-0.3.2/craynn/parameters/restricted.py` & `craynn-0.4.0/craynn/parameters/restricted.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-import tensorflow as tf
+import jax
+import jax.numpy as jnp
+import jax.nn as jnn
 
 from .common import zeros_init
-from .glorot import glorot_normal_init
+from .glorot import glorot_normal_init, glorot_uniform_init
 from .meta import Parameter, parameter_model
 
 __all__ = [
   'SoftmaxParameter', 'softmax_parameter',
   'SoftplusParameter', 'softplus_parameter',
 ]
 
 class SoftmaxParameter(Parameter):
   def __init__(self, shape, scale=1, w=zeros_init(), name=None, **properties):
-    self.scale = None if scale == 1 else tf.constant(scale, dtype=tf.float32)
+    self.scale = None if scale == 1 else scale
 
     self.w = w(shape=shape, **properties, name=(name + '_w') if name is not None else None)
 
     super(SoftmaxParameter, self).__init__(
       self.w, shape=shape, name=name,
       **properties
     )
 
   def get_output_for(self, w):
-    restricted = tf.nn.softmax(w)
+    restricted = jnn.softmax(w, axis=-1)
+
     if self.scale is not None:
       return self.scale * restricted
     else:
       return restricted
 
   def get_output_shape_for(self, w_shape):
     return w_shape
@@ -39,13 +42,31 @@
 
     super(SoftplusParameter, self).__init__(
       self.w, shape=shape, name=name,
       **properties
     )
 
   def get_output_for(self, w):
-    return tf.nn.softplus(w)
+    return jnn.softplus(w)
+
+  def get_output_shape_for(self, w_shape):
+    return w_shape
+
+softplus_parameter = parameter_model(SoftplusParameter)()
+
+
+class TanhParameter(Parameter):
+  def __init__(self, shape, w=glorot_uniform_init(), name=None, **properties):
+    self.w = w(shape=shape, **properties, name=(name + '_w') if name is not None else None)
+
+    super(TanhParameter, self).__init__(
+      self.w, shape=shape, name=name,
+      **properties
+    )
+
+  def get_output_for(self, w):
+    return jnn.tanh(w)
 
   def get_output_shape_for(self, w_shape):
     return w_shape
 
-softplus_parameter = parameter_model(SoftplusParameter)()
+tanh_parameter = parameter_model(TanhParameter)()
```

### Comparing `craynn-0.3.2/craynn/subnetworks/__init__.py` & `craynn-0.4.0/craynn/subnetworks/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,12 +9,10 @@
   with popular default parameters.
 """
 
 from .meta import *
 
 from .skip import *
 from .residual_nets import *
-from .vae_nets import *
+from .gates import *
 
-from .normalization import *
-
-from .meta_nets import *
+# from .normalization import *
```

### Comparing `craynn-0.3.2/craynn/updates/meta.py` & `craynn-0.4.0/craynn/updates/meta.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,90 @@
-import tensorflow as tf
-from .utils import get_rng
+import jax
 
 __all__ = [
   'Dataset'
 ]
 
 class Dataset(object):
-  def __init__(self, seed=None):
+  def __init__(self):
     ### allows nice `dataset.subset[:100] syntax`
     self.subset = SubsetConstructor(self)
-    self.rng = get_rng(seed)
 
-  def set_seed(self, seed=None):
-    self.rng = get_rng(seed)
+  def __getitem__(self, item):
+    raise NotImplementedError()
 
-  ### for a single item
-  def _get_single(self, item):
+  def size(self):
     raise NotImplementedError()
 
-  ### for slices
-  def _get_slice(self, item):
+  def __len__(self):
+    return int(self.size())
+
+  def materialize(self, batch_size=1, jit=True):
     raise NotImplementedError()
 
-  ### for any index arrays
-  def _get_sparse(self, item):
+  def shapes(self):
     raise NotImplementedError()
 
   def get_subset(self, item):
     from .subsets import SlicedSubset, IndexedSubset
     if isinstance(item, slice):
       return SlicedSubset(self, item)
     else:
       return IndexedSubset(self, item)
 
-  def size(self):
-    raise NotImplementedError()
-
-  def _data(self, batch_size=1):
-    """
-    Returns tensors held by the dataset. Must always return a tuple.
-    Warning: may result in allocation of a new dataset.
-    """
-    raise NotImplementedError()
-
-  def data(self, batch_size=1):
-    result = self._data(batch_size=batch_size)
-    return result
-
-  def numpy(self, batch_size=1):
-    return tuple(
-      d.numpy()
-      for d in self._data(batch_size=batch_size)
-    )
-
-  def materialize(self):
-    from .variable import variable_dataset
-    return variable_dataset(
-      *self._data()
-    )
-
-  def shapes(self):
-    raise NotImplementedError()
-
-  def __getitem__(self, item):
-    if isinstance(item, int):
-      return self._get_single(item)
-
-    elif isinstance(item, slice):
-      return self._get_slice(item)
-
-    else:
-      return self._get_sparse(item)
-
-  def __len__(self):
-    return int(self.size())
-
   def seq(self, batch_size=1):
     from .utils import sliced_seq
 
     if batch_size is None:
       for i in range(len(self)):
-        yield self._get_single(i)
+        yield self[i]
+
     else:
       for indx in sliced_seq(self.size(), batch_size=batch_size):
-        yield self._get_slice(indx)
+        yield self[indx]
 
   def indexed_seq(self, batch_size=1):
     from .utils import sliced_seq
 
     if batch_size is None:
       for i in range(len(self)):
-        yield i, self._get_single(i)
+        yield i, self[i]
+
     else:
       for indx in sliced_seq(self.size(), batch_size=batch_size):
-        yield indx, self._get_slice(indx)
+        yield indx, self[indx]
 
-  def batch(self, batch_size=1):
-    if batch_size is None:
-      indx = self.rng.uniform(
-        shape=(),
-        dtype=tf.int32,
-        minval=0,
-        maxval=self.size()
+  def batch(self, rng, size=1):
+    if size is None:
+      indx = jax.random.randint(
+        rng, shape=(), dtype=jax.numpy.int32, minval=0, maxval=self.size()
       )
 
-      return self._get_single(indx)
     else:
-      indx = self.rng.uniform(
-        shape=(batch_size, ),
-        dtype=tf.int32,
-        minval=0,
-        maxval=self.size()
+      indx = jax.random.randint(
+        rng, shape=(size, ), dtype=jax.numpy.int32, minval=0, maxval=self.size()
       )
 
-      return self._get_sparse(indx)
+    return self[indx]
 
-  def eval(self, f=None, batch_size=1):
+  def eval(self, f=None, batch_size=1, jit=True):
     if f is None:
-      return self.numpy(batch_size=batch_size)
+      return self.materialize(batch_size=batch_size, jit=jit)
     else:
-      return self.map(f).numpy(batch_size=batch_size)
+      return self.map(f).materialize(batch_size=batch_size, jit=jit)
 
   def map(self, f):
     from .common import MappedDataset
     return MappedDataset(self, f)
 
   def zip(self, other):
     from .common import ZippedDataset
     return ZippedDataset(self, other)
 
+
 class SubsetConstructor(object):
   def __init__(self, dataset : Dataset):
     self.dataset = dataset
 
   def __getitem__(self, item):
     return self(item)
```

### Comparing `craynn-0.3.2/craynn/viz/visualize.py` & `craynn-0.4.0/craynn/viz/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from craygraph import visualize
-
+from .. import dag
 from .. import layers
 from .. import parameters
 from ..info.layers import get_number_of_parameters
 
+from . import viz
+
 __all__ = [
   'draw_to_file',
   'draw_to_notebook',
 
   'all_nodes', 'only_layers'
 ]
 
@@ -18,15 +19,15 @@
   if any(p.kind == inspect.Parameter.VAR_POSITIONAL for p in signature.parameters.values()):
     return incoming
   else:
     assert len(signature.parameters) >= len(incoming)
     return dict(zip(signature.parameters, incoming))
 
 def all_nodes(node, args):
-  incoming = node.incoming()
+  incoming = node.incoming
 
   if len([arg for arg in args if arg is not None]) > 1:
     return map_inputs(node, incoming)
   else:
     return incoming
 
 def only_layers(node, args):
@@ -34,14 +35,23 @@
     return all_nodes(node, args)
 
   if isinstance(node, parameters.Parameter):
     return None
   else:
     return all_nodes(node, args)
 
+def layers_alike(node, args):
+  if any(arg is not None for arg in args):
+    return all_nodes(node, args)
+
+  if isinstance(node, parameters.FreeParameter):
+    return None
+  else:
+    return all_nodes(node, args)
+
 _color_set = (
   ### blue
   (('conv', ), ('#a6cee3', '#1f78b4')),
   ### green
   (('dense', layers.DenseLayer), ('#b2df8a', '#33a02c')),
   ### red
   (('input', layers.InputLayer), ('#fb9a99', '#e31a1c')),
@@ -81,22 +91,24 @@
 
     _, colors = color_set[-1]
     j = hashed % len(colors)
     return colors[j]
 
   return get_color
 
-def viz_params(**kwargs):
+def viz_params():
   def f(layer, _):
-    param_info = get_number_of_parameters(layer, **kwargs).items()
+    param_info = get_number_of_parameters(layer).items()
     if len(param_info) > 0:
       return ','.join([ '%s: %d' % (k.name, v) for k, v in param_info ])
     else:
       return None
 
+  return f
+
 def viz_all_params(**properties):
   def number_of_params(layer):
     n = get_number_of_parameters(layer)
 
     if n > 0:
       return '#params: %d' % n
     else:
@@ -114,41 +126,41 @@
 
     kernel_info = []
     if hasattr(layer, 'kernel_size'):
       kernel_info.append(
         'x'.join('%d' % k for k in layer.kernel_size)
       )
 
-    if hasattr(layer, 'stride'):
-      if any(s != 1 for s in layer.stride):
+    if hasattr(layer, 'strides'):
+      if any(s != 1 for s in layer.strides):
         kernel_info.append(
-          'stride=%s' % (
-            'x'.join('%d' % k for k in layer.stride),
+          'strides=%s' % (
+            'x'.join('%d' % k for k in layer.strides),
           )
         )
 
     if hasattr(layer, 'padding'):
       if layer.padding != 'valid':
-        kernel_info.append('pad=%s' % layer.padding)
+        kernel_info.append('pad=%s' % (layer.padding, ))
 
-    if layer.name() is None or force_class_name:
+    if layer.name is None or force_class_name:
       result = layer_class
     else:
-      result = '%s : %s' % (layer.name(), layer_class)
+      result = '%s : %s' % (layer.name, layer_class)
 
     if kernel_info:
       return '%s %s' % (result, ', '.join(kernel_info))
     else:
       return result
 
   return name
 
 def viz_output_shape():
   def output_shape(layer):
-    shape = layers.get_output_shape(layer)
+    shape = dag.get_output_shape(layer)
     return str(shape)
 
   return output_shape
 
 def viz_activation():
   def activation(layer):
     return getattr(layer, 'activation', None)
@@ -162,16 +174,16 @@
   _shape_ = viz_output_shape(),
   __style__ = 'filled',
   __fillcolor__ = layer_color(color_set=_color_set),
   __color__ = 'black',
   __shape__ = 'box'
 )
 
-def draw_to_file(path, network, selector=only_layers, **properties):
+def draw_to_file(path, network, selector=layers_alike, **properties):
   props = default_display_properties.copy()
   props.update(properties)
-  return visualize.draw_to_file(path, network, selector=selector, **props)
+  return viz.draw_to_file(path, network, selector=selector, **props)
 
-def draw_to_notebook(network, selector=only_layers, **properties):
+def draw_to_notebook(network, selector=layers_alike, **properties):
   props = default_display_properties.copy()
   props.update(properties)
-  return visualize.draw_to_notebook(network, selector=selector, **props)
+  return viz.draw_to_notebook(network, selector=selector, **props)
```

### Comparing `craynn-0.3.2/craynn.egg-info/PKG-INFO` & `craynn-0.4.0/craynn.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 Metadata-Version: 2.1
 Name: craynn
-Version: 0.3.2
+Version: 0.4.0
 Summary: Yet another neural network toolkit.
 Home-page: https://gitlab.com/craynn/craynn
 Author: Maxim Borisyak and contributors.
 Author-email: maximus.been@gmail.com
 Maintainer: Maxim Borisyak
 Maintainer-email: maximus.been@gmail.com
 License: MIT
-Description: # craynn
-        
-        Yet Another toolkit for Neural Network slightly flavoured by Ultra-High Energy Cosmic Rays. 
-        
-        ## Philosophy
-        
-        `CrayNN` is highly influenced by [Lasange](https://github.com/Lasagne/Lasagne):
-        
-            Simplicity: Be easy to use, easy to understand and easy to extend, to facilitate use in research
-            Transparency: Do not hide Theano behind abstractions, directly process and return Theano expressions or Python / numpy data types
-            Modularity: Allow all parts (layers, regularizers, optimizers, ...) to be used independently of Lasagne
-            Pragmatism: Make common use cases easy, do not overrate uncommon cases
-            Restraint: Do not obstruct users with features they decide not to use
-            Focus: "Do one thing and do it well"
-        
-        Just replace `theano` with `tensorflow`.
-        
-        ## Installation
-        
-        ### via PyPi
-        
-        `pip install craynn`
-        
-        ### via git
-        
-        `craynn` can be installed directly from `gitlab.com`:
-        `pip install git+https://gitlab.com/craynn/craynn.git`
-        however, as repository updates frequently, it is recommend to clone the repository
-        and install the package in development mode:
-        ```
-        git clone git@gitlab.com:craynn/craynn.git
-        cd craynn/
-        pip install -e .
-        ```
-        
-        **NB**: don't forget to install proper version of `craygraph` in a similar manner:
-        ```
-        git clone git@gitlab.com:craynn/craygraph.git
-        cd craygraph/
-        pip install -e .
-        ``` 
-        
-        ## Usage
-        
-        Check out jupyter notebooks in `examples/`. 
-        
-        ## Quick guide
-        
-        `craynn` is designed for rapidly defining networks of all sorts:
-        ```python
-        from craynn import network, conv, max_pool
-        
-        net = network((None, 1, 28, 28))(
-          conv(16), conv(24), max_pool(),
-          conv(16), conv(24), max_pool(),
-          conv(16), conv(24), max_pool(),
-        )
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: jax>=0.3.8
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: matplotlib>=3.0.2
+Requires-Dist: pydotplus>=2.0.2
 Provides-Extra: test
+Requires-Dist: pytest>=4.0.0; extra == "test"
+Requires-Dist: scipy>=1.3.0; extra == "test"
+
+# craynn
+
+Yet Another toolkit for Neural Network slightly flavoured by Ultra-High Energy Cosmic Rays. 
+
+## Philosophy
+
+`CrayNN` is highly influenced by [Lasange](https://github.com/Lasagne/Lasagne):
+
+    Simplicity: Be easy to use, easy to understand and easy to extend, to facilitate use in research
+    Transparency: Do not hide Theano behind abstractions, directly process and return Theano expressions or Python / numpy data types
+    Modularity: Allow all parts (layers, regularizers, optimizers, ...) to be used independently of Lasagne
+    Pragmatism: Make common use cases easy, do not overrate uncommon cases
+    Restraint: Do not obstruct users with features they decide not to use
+    Focus: "Do one thing and do it well"
+
+Just replace `theano` with `jax`.
+
+## Installation
+
+### via PyPi
+
+`pip install craynn`
+
+### via git
+
+`craynn` can be installed directly from `gitlab.com`:
+`pip install git+https://gitlab.com/craynn/craynn.git`
+however, as repository updates frequently, it is recommended to clone the repository
+and install the package in development mode:
+```
+git clone git@gitlab.com:craynn/craynn.git
+cd craynn/
+pip install -e .
+```
+
+## Usage
+
+Take a look at jupyter notebooks in `examples/`. 
+
+## Quick guide
+
+`craynn` is designed for rapidly defining networks of all sorts:
+```python
+from craynn import network, conv, max_pool
+
+net = network((None, 1, 28, 28))(
+  conv(16), conv(24), max_pool(),
+  conv(16), conv(24), max_pool(),
+  conv(16), conv(24), max_pool(),
+)
+```
```

### Comparing `craynn-0.3.2/craynn.egg-info/SOURCES.txt` & `craynn-0.4.0/craynn.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,77 @@
+LICENSE
 README.md
 setup.py
 craynn/__init__.py
 craynn.egg-info/PKG-INFO
 craynn.egg-info/SOURCES.txt
 craynn.egg-info/dependency_links.txt
 craynn.egg-info/requires.txt
 craynn.egg-info/top_level.txt
+craynn/dag/__init__.py
+craynn/dag/common.py
+craynn/dag/meta.py
+craynn/dag/evaluate/__init__.py
+craynn/dag/evaluate/common.py
+craynn/dag/evaluate/dynamic.py
+craynn/dag/evaluate/static.py
+craynn/dag/lang/__init__.py
+craynn/dag/lang/achain.py
+craynn/dag/lang/language.py
+craynn/dag/lang/selector.py
 craynn/info/__init__.py
 craynn/info/layers.py
-craynn/info/nodes.py
 craynn/layers/__init__.py
 craynn/layers/common.py
 craynn/layers/dense_ops.py
 craynn/layers/gates.py
-craynn/layers/gmm.py
 craynn/layers/meta.py
-craynn/layers/meta_ops.py
 craynn/layers/noise_ops.py
-craynn/layers/normalization.py
 craynn/layers/conv_ops/__init__.py
 craynn/layers/conv_ops/_conv.py
-craynn/layers/conv_ops/_deconv.py
 craynn/layers/conv_ops/_pool.py
 craynn/layers/conv_ops/_upscale.py
 craynn/layers/conv_ops/conv_utils.py
 craynn/networks/__init__.py
 craynn/networks/meta.py
 craynn/networks/utils.py
 craynn/nonlinearities/__init__.py
 craynn/nonlinearities/common.py
 craynn/nonlinearities/defaults.py
 craynn/nonlinearities/meta.py
 craynn/objectives/__init__.py
 craynn/objectives/classification.py
-craynn/objectives/common.py
 craynn/objectives/elbo.py
-craynn/objectives/meta.py
 craynn/objectives/regression.py
 craynn/objectives/regularization.py
 craynn/parameters/__init__.py
-craynn/parameters/binary.py
 craynn/parameters/common.py
 craynn/parameters/decomposition.py
 craynn/parameters/defaults.py
 craynn/parameters/glorot.py
 craynn/parameters/masked.py
 craynn/parameters/meta.py
 craynn/parameters/noisy.py
-craynn/parameters/normed.py
 craynn/parameters/orthogonal.py
-craynn/parameters/parameter_utils.py
 craynn/parameters/restricted.py
-craynn/regularization/__init__.py
-craynn/regularization/common.py
-craynn/regularization/meta.py
+craynn/parameters/utils.py
 craynn/subnetworks/__init__.py
+craynn/subnetworks/gates.py
 craynn/subnetworks/meta.py
-craynn/subnetworks/meta_nets.py
-craynn/subnetworks/normalization.py
 craynn/subnetworks/residual_nets.py
 craynn/subnetworks/skip.py
-craynn/subnetworks/vae_nets.py
+craynn/train/__init__.py
+craynn/train/common.py
 craynn/updates/__init__.py
+craynn/updates/array.py
 craynn/updates/common.py
 craynn/updates/meta.py
 craynn/updates/subsets.py
 craynn/updates/utils.py
-craynn/updates/variable.py
 craynn/utils/__init__.py
 craynn/utils/axes.py
-craynn/utils/tf_utils.py
-craynn/utils/data/__init__.py
-craynn/utils/data/common.py
-craynn/utils/data/concept_learning.py
-craynn/utils/data/images.py
-craynn/utils/data/text.py
+craynn/utils/clazz.py
+craynn/utils/func.py
+craynn/utils/math.py
 craynn/viz/__init__.py
-craynn/viz/visualize.py
-craynn/viz/watcher.py
+craynn/viz/common.py
+craynn/viz/viz.py
```

### Comparing `craynn-0.3.2/setup.py` & `craynn-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 
 here = os.path.dirname(__file__)
 
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
   long_description=f.read()
 
-version = '0.3.2'
+version = '0.4.0'
 
 setup(
   name = 'craynn',
   version=version,
   description="""Yet another neural network toolkit.""",
 
   long_description=long_description,
@@ -43,17 +43,16 @@
     'test': [
       'pytest >= 4.0.0',
       'scipy >= 1.3.0'
     ],
   },
 
   install_requires=[
-    'craygraph >= 0.3.0',
-    'tensorflow >= 2.3.0',
-    'numpy >= 1.17.1',
+    'jax >= 0.3.8',
+    'numpy >= 1.17.0',
     'matplotlib >= 3.0.2',
     'pydotplus >= 2.0.2',
   ],
 
   python_requires='>=3.7',
 )
```

