# Comparing `tmp/heat-1.4.0.tar.gz` & `tmp/heat-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heat-1.4.0.tar", last modified: Thu Apr 18 08:33:38 2024, max compression
+gzip compressed data, was "heat-1.4.1.tar", last modified: Mon May 13 11:05:43 2024, max compression
```

## Comparing `heat-1.4.0.tar` & `heat-1.4.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.881997 heat-1.4.0/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     1192 2023-07-24 13:32:34.000000 heat-1.4.0/LICENSE
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    13291 2024-04-18 08:33:38.880998 heat-1.4.0/PKG-INFO
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    11851 2024-04-15 09:38:15.000000 heat-1.4.0/README.md
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.499989 heat-1.4.0/heat/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      419 2024-04-03 10:40:08.000000 heat-1.4.0/heat/__init__.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.526019 heat-1.4.0/heat/classification/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       79 2023-07-24 13:32:35.000000 heat-1.4.0/heat/classification/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     4717 2024-04-03 10:40:08.000000 heat-1.4.0/heat/classification/kneighborsclassifier.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.551998 heat-1.4.0/heat/cluster/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      224 2024-04-15 09:38:15.000000 heat-1.4.0/heat/cluster/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    11575 2024-04-15 09:38:15.000000 heat-1.4.0/heat/cluster/_kcluster.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    18439 2024-04-15 09:38:15.000000 heat-1.4.0/heat/cluster/batchparallelclustering.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5481 2024-04-15 09:38:15.000000 heat-1.4.0/heat/cluster/kmeans.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5543 2024-04-15 09:38:15.000000 heat-1.4.0/heat/cluster/kmedians.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     6088 2024-04-03 10:40:08.000000 heat-1.4.0/heat/cluster/kmedoids.py
--rwx------   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     8174 2023-10-30 07:50:09.000000 heat-1.4.0/heat/cluster/spectral.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.669994 heat-1.4.0/heat/core/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      790 2024-02-01 10:00:28.000000 heat-1.4.0/heat/core/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    20752 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/_operations.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)   115820 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/arithmetics.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     8724 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/base.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    75974 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/communication.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     3166 2023-07-24 13:32:35.000000 heat-1.4.0/heat/core/complex_math.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     1072 2023-07-24 13:32:35.000000 heat-1.4.0/heat/core/constants.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     4951 2023-11-22 13:39:03.000000 heat-1.4.0/heat/core/devices.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    75015 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/dndarray.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    10997 2023-07-24 13:32:35.000000 heat-1.4.0/heat/core/exponential.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    58349 2024-04-17 13:50:50.000000 heat-1.4.0/heat/core/factories.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5399 2023-11-22 13:39:03.000000 heat-1.4.0/heat/core/indexing.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    45033 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/io.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.691996 heat-1.4.0/heat/core/linalg/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      160 2024-01-22 14:35:17.000000 heat-1.4.0/heat/core/linalg/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    89776 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/linalg/basics.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    14456 2024-04-18 07:47:42.000000 heat-1.4.0/heat/core/linalg/qr.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    10346 2024-04-17 12:15:23.000000 heat-1.4.0/heat/core/linalg/solver.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      567 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/linalg/svd.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    25582 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/linalg/svdtools.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    18390 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/logical.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)   153593 2024-04-03 12:29:03.000000 heat-1.4.0/heat/core/manipulations.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     3211 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/memory.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    11279 2024-02-01 10:00:28.000000 heat-1.4.0/heat/core/printing.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    37383 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/random.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    13167 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/relational.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    15188 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/rounding.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    11512 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/sanitation.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     7557 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/signal.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    75387 2024-04-08 09:45:59.000000 heat-1.4.0/heat/core/statistics.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     8109 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/stride_tricks.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    52200 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/tiling.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    16274 2023-07-24 13:32:35.000000 heat-1.4.0/heat/core/trigonometrics.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    28107 2024-04-03 10:40:08.000000 heat-1.4.0/heat/core/types.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      533 2024-04-18 07:49:51.000000 heat-1.4.0/heat/core/version.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.748990 heat-1.4.0/heat/datasets/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       50 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    25312 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/diabetes.h5
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     2400 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris.csv
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     6944 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris.h5
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    11040 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris.nc
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     1800 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_X_test.csv
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     1800 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_X_train.csv
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      300 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_labels.csv
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5669 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_y_pred_proba.csv
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      150 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_y_test.csv
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      150 2023-07-24 13:32:35.000000 heat-1.4.0/heat/datasets/iris_y_train.csv
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.755990 heat-1.4.0/heat/fft/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       76 2024-04-03 10:40:08.000000 heat-1.4.0/heat/fft/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    46743 2024-04-03 10:40:08.000000 heat-1.4.0/heat/fft/fft.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.762995 heat-1.4.0/heat/graph/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       86 2023-07-24 13:32:35.000000 heat-1.4.0/heat/graph/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     4963 2024-04-03 10:40:08.000000 heat-1.4.0/heat/graph/laplacian.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.769993 heat-1.4.0/heat/naive_bayes/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       88 2023-07-24 13:32:35.000000 heat-1.4.0/heat/naive_bayes/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    22137 2024-04-03 10:40:08.000000 heat-1.4.0/heat/naive_bayes/gaussianNB.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.780994 heat-1.4.0/heat/nn/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     2265 2023-07-24 13:32:35.000000 heat-1.4.0/heat/nn/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    16358 2024-04-03 10:40:08.000000 heat-1.4.0/heat/nn/data_parallel.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      630 2023-10-30 07:50:10.000000 heat-1.4.0/heat/nn/functional.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.794997 heat-1.4.0/heat/optim/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     2507 2023-07-24 13:32:35.000000 heat-1.4.0/heat/optim/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    39179 2024-04-03 10:40:08.000000 heat-1.4.0/heat/optim/dp_optimizer.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      380 2023-10-30 07:50:10.000000 heat-1.4.0/heat/optim/lr_scheduler.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     7171 2023-07-24 13:32:35.000000 heat-1.4.0/heat/optim/utils.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.801999 heat-1.4.0/heat/preprocessing/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      104 2024-02-01 10:00:28.000000 heat-1.4.0/heat/preprocessing/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    22404 2024-04-08 09:45:59.000000 heat-1.4.0/heat/preprocessing/preprocessing.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.809990 heat-1.4.0/heat/regression/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       80 2023-07-24 13:32:35.000000 heat-1.4.0/heat/regression/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5637 2024-04-03 10:40:08.000000 heat-1.4.0/heat/regression/lasso.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.829994 heat-1.4.0/heat/sparse/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      194 2023-10-30 07:50:10.000000 heat-1.4.0/heat/sparse/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     5682 2024-04-03 10:40:08.000000 heat-1.4.0/heat/sparse/_operations.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     3277 2024-04-03 10:40:08.000000 heat-1.4.0/heat/sparse/arithmetics.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     9923 2024-04-03 10:40:08.000000 heat-1.4.0/heat/sparse/dcsr_matrix.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    10096 2024-04-03 10:40:08.000000 heat-1.4.0/heat/sparse/factories.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     4033 2024-04-03 10:40:08.000000 heat-1.4.0/heat/sparse/manipulations.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.836997 heat-1.4.0/heat/spatial/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       93 2023-07-24 13:32:35.000000 heat-1.4.0/heat/spatial/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    18019 2024-04-03 10:40:08.000000 heat-1.4.0/heat/spatial/distance.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.844008 heat-1.4.0/heat/utils/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      112 2023-07-24 13:32:35.000000 heat-1.4.0/heat/utils/__init__.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.870993 heat-1.4.0/heat/utils/data/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      195 2023-10-30 07:50:10.000000 heat-1.4.0/heat/utils/data/__init__.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    13358 2023-10-30 07:50:10.000000 heat-1.4.0/heat/utils/data/_utils.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    17539 2023-11-22 13:39:03.000000 heat-1.4.0/heat/utils/data/datatools.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     8982 2024-04-03 10:40:08.000000 heat-1.4.0/heat/utils/data/matrixgallery.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     4849 2023-10-30 07:50:10.000000 heat-1.4.0/heat/utils/data/mnist.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    15496 2023-11-22 13:39:03.000000 heat-1.4.0/heat/utils/data/partial_dataset.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     7019 2024-04-15 09:38:15.000000 heat-1.4.0/heat/utils/data/spherical.py
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      606 2023-10-30 07:50:10.000000 heat-1.4.0/heat/utils/vision_transforms.py
-drwxr-xr-x   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        0 2024-04-18 08:33:38.875995 heat-1.4.0/heat.egg-info/
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)    13291 2024-04-18 08:33:38.000000 heat-1.4.0/heat.egg-info/PKG-INFO
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     2469 2024-04-18 08:33:38.000000 heat-1.4.0/heat.egg-info/SOURCES.txt
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        1 2024-04-18 08:33:38.000000 heat-1.4.0/heat.egg-info/dependency_links.txt
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      265 2024-04-18 08:33:38.000000 heat-1.4.0/heat.egg-info/requires.txt
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)        5 2024-04-18 08:33:38.000000 heat-1.4.0/heat.egg-info/top_level.txt
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)       31 2023-07-24 13:32:35.000000 heat-1.4.0/pyproject.toml
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)      327 2024-04-18 08:33:38.885996 heat-1.4.0/setup.cfg
--rw-r--r--   0 hopp_fa  (151518) dlr_hopp_fa_p (440872)     1756 2024-04-17 13:50:50.000000 heat-1.4.0/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.356308 heat-1.4.1/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1192 2023-03-14 14:19:57.000000 heat-1.4.1/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)    13303 2024-05-13 11:05:43.356308 heat-1.4.1/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11863 2024-04-29 09:09:08.000000 heat-1.4.1/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.316308 heat-1.4.1/heat/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      419 2024-02-20 09:04:42.000000 heat-1.4.1/heat/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.320308 heat-1.4.1/heat/classification/
+-rw-rw-r--   0 michael   (1000) michael   (1000)       79 2023-03-14 14:19:57.000000 heat-1.4.1/heat/classification/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4717 2024-02-20 09:04:42.000000 heat-1.4.1/heat/classification/kneighborsclassifier.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.324308 heat-1.4.1/heat/cluster/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      224 2024-04-29 09:09:08.000000 heat-1.4.1/heat/cluster/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11575 2024-04-29 09:09:08.000000 heat-1.4.1/heat/cluster/_kcluster.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    18439 2024-04-29 09:09:08.000000 heat-1.4.1/heat/cluster/batchparallelclustering.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5481 2024-04-29 09:09:08.000000 heat-1.4.1/heat/cluster/kmeans.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5543 2024-04-29 09:09:08.000000 heat-1.4.1/heat/cluster/kmedians.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6088 2024-02-20 09:04:42.000000 heat-1.4.1/heat/cluster/kmedoids.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8174 2023-07-07 15:01:37.000000 heat-1.4.1/heat/cluster/spectral.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.336308 heat-1.4.1/heat/core/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      790 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    20752 2024-04-29 09:09:08.000000 heat-1.4.1/heat/core/_operations.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)   115820 2024-04-29 09:09:08.000000 heat-1.4.1/heat/core/arithmetics.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8724 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    75974 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/communication.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3166 2023-03-14 14:19:57.000000 heat-1.4.1/heat/core/complex_math.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1072 2023-03-14 14:19:57.000000 heat-1.4.1/heat/core/constants.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4951 2023-07-07 15:01:37.000000 heat-1.4.1/heat/core/devices.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    75015 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/dndarray.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10997 2023-03-14 14:19:57.000000 heat-1.4.1/heat/core/exponential.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    58652 2024-05-07 12:03:34.000000 heat-1.4.1/heat/core/factories.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5399 2023-08-01 07:12:31.000000 heat-1.4.1/heat/core/indexing.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    45033 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/io.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.336308 heat-1.4.1/heat/core/linalg/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      160 2023-07-07 15:01:37.000000 heat-1.4.1/heat/core/linalg/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    89776 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/linalg/basics.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14456 2024-04-29 09:09:08.000000 heat-1.4.1/heat/core/linalg/qr.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10346 2024-04-29 09:09:08.000000 heat-1.4.1/heat/core/linalg/solver.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      567 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/linalg/svd.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    25582 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/linalg/svdtools.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    18390 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/logical.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)   153593 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/manipulations.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3211 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/memory.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11279 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/printing.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    37383 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/random.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13167 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/relational.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15188 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/rounding.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11512 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/sanitation.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7557 2024-04-29 09:09:08.000000 heat-1.4.1/heat/core/signal.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    75387 2024-04-29 09:09:08.000000 heat-1.4.1/heat/core/statistics.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8109 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/stride_tricks.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    52200 2024-02-20 09:04:42.000000 heat-1.4.1/heat/core/tiling.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    16274 2023-05-02 10:30:37.000000 heat-1.4.1/heat/core/trigonometrics.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    28107 2024-04-29 09:09:08.000000 heat-1.4.1/heat/core/types.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      533 2024-05-13 11:03:26.000000 heat-1.4.1/heat/core/version.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.340308 heat-1.4.1/heat/datasets/
+-rw-rw-r--   0 michael   (1000) michael   (1000)       50 2023-03-14 14:19:57.000000 heat-1.4.1/heat/datasets/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    25312 2023-03-14 14:19:57.000000 heat-1.4.1/heat/datasets/diabetes.h5
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2400 2023-03-14 14:19:57.000000 heat-1.4.1/heat/datasets/iris.csv
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6944 2023-03-14 14:19:57.000000 heat-1.4.1/heat/datasets/iris.h5
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11040 2023-03-14 14:19:57.000000 heat-1.4.1/heat/datasets/iris.nc
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1800 2023-03-14 14:19:57.000000 heat-1.4.1/heat/datasets/iris_X_test.csv
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1800 2023-03-14 14:19:57.000000 heat-1.4.1/heat/datasets/iris_X_train.csv
+-rw-rw-r--   0 michael   (1000) michael   (1000)      300 2023-03-14 14:19:57.000000 heat-1.4.1/heat/datasets/iris_labels.csv
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5669 2023-03-14 14:19:57.000000 heat-1.4.1/heat/datasets/iris_y_pred_proba.csv
+-rw-rw-r--   0 michael   (1000) michael   (1000)      150 2023-03-14 14:19:57.000000 heat-1.4.1/heat/datasets/iris_y_test.csv
+-rw-rw-r--   0 michael   (1000) michael   (1000)      150 2023-03-14 14:19:57.000000 heat-1.4.1/heat/datasets/iris_y_train.csv
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.340308 heat-1.4.1/heat/fft/
+-rw-rw-r--   0 michael   (1000) michael   (1000)       76 2024-02-20 09:04:42.000000 heat-1.4.1/heat/fft/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    46743 2024-04-29 09:09:08.000000 heat-1.4.1/heat/fft/fft.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.340308 heat-1.4.1/heat/graph/
+-rw-rw-r--   0 michael   (1000) michael   (1000)       86 2023-03-14 14:19:57.000000 heat-1.4.1/heat/graph/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4963 2024-02-20 09:04:42.000000 heat-1.4.1/heat/graph/laplacian.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.344308 heat-1.4.1/heat/naive_bayes/
+-rw-rw-r--   0 michael   (1000) michael   (1000)       88 2023-03-14 14:19:57.000000 heat-1.4.1/heat/naive_bayes/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    22137 2024-04-29 09:09:08.000000 heat-1.4.1/heat/naive_bayes/gaussianNB.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.344308 heat-1.4.1/heat/nn/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2265 2023-07-07 15:01:37.000000 heat-1.4.1/heat/nn/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    16358 2024-02-20 09:04:42.000000 heat-1.4.1/heat/nn/data_parallel.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      630 2023-07-07 15:01:37.000000 heat-1.4.1/heat/nn/functional.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.344308 heat-1.4.1/heat/optim/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2507 2023-07-07 15:01:37.000000 heat-1.4.1/heat/optim/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    39179 2024-02-20 09:04:42.000000 heat-1.4.1/heat/optim/dp_optimizer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      380 2023-07-07 15:01:37.000000 heat-1.4.1/heat/optim/lr_scheduler.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7171 2023-03-14 14:19:57.000000 heat-1.4.1/heat/optim/utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.344308 heat-1.4.1/heat/preprocessing/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      104 2024-02-20 09:04:42.000000 heat-1.4.1/heat/preprocessing/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    22404 2024-04-29 09:09:08.000000 heat-1.4.1/heat/preprocessing/preprocessing.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.348308 heat-1.4.1/heat/regression/
+-rw-rw-r--   0 michael   (1000) michael   (1000)       80 2023-03-14 14:19:57.000000 heat-1.4.1/heat/regression/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5637 2024-02-20 09:04:42.000000 heat-1.4.1/heat/regression/lasso.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.348308 heat-1.4.1/heat/sparse/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      194 2023-07-07 15:01:37.000000 heat-1.4.1/heat/sparse/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5682 2024-02-20 09:04:42.000000 heat-1.4.1/heat/sparse/_operations.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3277 2024-02-20 09:04:42.000000 heat-1.4.1/heat/sparse/arithmetics.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9923 2024-02-20 09:04:42.000000 heat-1.4.1/heat/sparse/dcsr_matrix.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10096 2024-02-20 09:04:42.000000 heat-1.4.1/heat/sparse/factories.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4033 2024-02-20 09:04:42.000000 heat-1.4.1/heat/sparse/manipulations.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.348308 heat-1.4.1/heat/spatial/
+-rw-rw-r--   0 michael   (1000) michael   (1000)       93 2023-03-14 14:19:57.000000 heat-1.4.1/heat/spatial/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    18019 2024-02-20 09:04:42.000000 heat-1.4.1/heat/spatial/distance.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.348308 heat-1.4.1/heat/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      112 2023-03-14 14:19:57.000000 heat-1.4.1/heat/utils/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.352308 heat-1.4.1/heat/utils/data/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      195 2023-07-07 15:01:37.000000 heat-1.4.1/heat/utils/data/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13358 2023-07-07 15:01:37.000000 heat-1.4.1/heat/utils/data/_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    17539 2023-03-14 14:19:57.000000 heat-1.4.1/heat/utils/data/datatools.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8982 2024-04-29 09:09:08.000000 heat-1.4.1/heat/utils/data/matrixgallery.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4849 2023-07-07 15:01:37.000000 heat-1.4.1/heat/utils/data/mnist.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15496 2023-07-07 15:01:37.000000 heat-1.4.1/heat/utils/data/partial_dataset.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7019 2024-04-29 09:09:08.000000 heat-1.4.1/heat/utils/data/spherical.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      606 2023-07-07 15:01:37.000000 heat-1.4.1/heat/utils/vision_transforms.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-13 11:05:43.352308 heat-1.4.1/heat.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)    13303 2024-05-13 11:05:43.000000 heat-1.4.1/heat.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2469 2024-05-13 11:05:43.000000 heat-1.4.1/heat.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2024-05-13 11:05:43.000000 heat-1.4.1/heat.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)      265 2024-05-13 11:05:43.000000 heat-1.4.1/heat.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        5 2024-05-13 11:05:43.000000 heat-1.4.1/heat.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       31 2023-03-14 14:19:57.000000 heat-1.4.1/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      327 2024-05-13 11:05:43.356308 heat-1.4.1/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1756 2024-04-29 09:09:08.000000 heat-1.4.1/setup.py
```

### Comparing `heat-1.4.0/LICENSE` & `heat-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/PKG-INFO` & `heat-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heat
-Version: 1.4.0
+Version: 1.4.1
 Summary: A framework for high-performance data analytics and machine learning.
 Home-page: https://github.com/helmholtz-analytics/heat
 Author: Helmholtz Association
 Author-email: martin.siggel@dlr.de
 Keywords: data,analytics,tensors,distributed,gpu
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -147,15 +147,15 @@
 
 ## Requirements
 
 ### Basics
 - python >= 3.8
 - MPI (OpenMPI, MPICH, Intel MPI, etc.)
 - mpi4py >= 3.0.0
-- pytorch >= 1.8.0
+- pytorch >= 1.11.0
 
 ### Parallel I/O
 - h5py
 - netCDF4
 
 ### GPU support
 In order to do computations on your GPU(s):
@@ -196,15 +196,15 @@
 If you’re unsure where to start or how your skills fit in, reach out! You can ask us here on GitHub, by leaving a comment on a relevant issue that is already open.
 
 **If you are new to contributing to open source, [this guide](https://opensource.guide/how-to-contribute/) helps explain why, what, and how to get involved.**
 
 
 ## Resources
 
-* [Heat Tutorials](https://heat.readthedocs.io/en/latest/tutorials.html)
+* [Heat Tutorials](https://github.com/helmholtz-analytics/heat/tree/main/tutorials)
 * [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html)
 
 ### Parallel Computing and MPI:
 
 * David Henty's [course](https://www.archer2.ac.uk/training/courses/200514-mpi/)
 * Wes Kendall's [Tutorials](https://mpitutorial.com/tutorials/)
 * Rolf Rabenseifner's [MPI course material](https://www.hlrs.de/training/self-study-materials/mpi-course-material) (including C, Fortran **and** Python via `mpi4py`)
```

### Comparing `heat-1.4.0/README.md` & `heat-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 ## Requirements
 
 ### Basics
 - python >= 3.8
 - MPI (OpenMPI, MPICH, Intel MPI, etc.)
 - mpi4py >= 3.0.0
-- pytorch >= 1.8.0
+- pytorch >= 1.11.0
 
 ### Parallel I/O
 - h5py
 - netCDF4
 
 ### GPU support
 In order to do computations on your GPU(s):
@@ -157,15 +157,15 @@
 If you’re unsure where to start or how your skills fit in, reach out! You can ask us here on GitHub, by leaving a comment on a relevant issue that is already open.
 
 **If you are new to contributing to open source, [this guide](https://opensource.guide/how-to-contribute/) helps explain why, what, and how to get involved.**
 
 
 ## Resources
 
-* [Heat Tutorials](https://heat.readthedocs.io/en/latest/tutorials.html)
+* [Heat Tutorials](https://github.com/helmholtz-analytics/heat/tree/main/tutorials)
 * [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html)
 
 ### Parallel Computing and MPI:
 
 * David Henty's [course](https://www.archer2.ac.uk/training/courses/200514-mpi/)
 * Wes Kendall's [Tutorials](https://mpitutorial.com/tutorials/)
 * Rolf Rabenseifner's [MPI course material](https://www.hlrs.de/training/self-study-materials/mpi-course-material) (including C, Fortran **and** Python via `mpi4py`)
```

### Comparing `heat-1.4.0/heat/classification/kneighborsclassifier.py` & `heat-1.4.1/heat/classification/kneighborsclassifier.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/cluster/_kcluster.py` & `heat-1.4.1/heat/cluster/_kcluster.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/cluster/batchparallelclustering.py` & `heat-1.4.1/heat/cluster/batchparallelclustering.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/cluster/kmeans.py` & `heat-1.4.1/heat/cluster/kmeans.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/cluster/kmedians.py` & `heat-1.4.1/heat/cluster/kmedians.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/cluster/kmedoids.py` & `heat-1.4.1/heat/cluster/kmedoids.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/cluster/spectral.py` & `heat-1.4.1/heat/cluster/spectral.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/__init__.py` & `heat-1.4.1/heat/core/__init__.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/_operations.py` & `heat-1.4.1/heat/core/_operations.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/arithmetics.py` & `heat-1.4.1/heat/core/arithmetics.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/base.py` & `heat-1.4.1/heat/core/base.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/communication.py` & `heat-1.4.1/heat/core/communication.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/complex_math.py` & `heat-1.4.1/heat/core/complex_math.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/constants.py` & `heat-1.4.1/heat/core/constants.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/devices.py` & `heat-1.4.1/heat/core/devices.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/dndarray.py` & `heat-1.4.1/heat/core/dndarray.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/exponential.py` & `heat-1.4.1/heat/core/exponential.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/factories.py` & `heat-1.4.1/heat/core/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -594,21 +594,21 @@
     split: Optional[int] = None,
     device: Optional[Device] = None,
     comm: Optional[Communication] = None,
     order: str = "C",
 ) -> DNDarray:
     """
     Returns a new uninitialized :class:`~heat.core.dndarray.DNDarray` with the same type, shape and data distribution
-    of given object. Data type and data distribution strategy can be explicitly overriden.
+    of given object. Data type, data distribution axis, and device can be explicitly overridden.
 
     Parameters
     ----------
     a : DNDarray
-        The shape and data-type of ``a`` define these same attributes of the returned array. Uninitialized array with
-        the same shape, type and split axis as ``a`` unless overriden.
+        The shape, data-type, split axis and device of ``a`` define these same attributes of the returned array. Uninitialized array with
+        the same shape, type, split axis and device as ``a`` unless overriden.
     dtype : datatype, optional
         Overrides the data type of the result.
     split: int or None, optional
         The axis along which the array is split and distributed; ``None`` means no distribution.
     device : str or Device, optional
         Specifies the :class:`~heat.core.devices.Device` the array shall be allocated on, defaults to globally set
         default device.
@@ -790,16 +790,15 @@
     dtype : datatype
         The desired HeAT data type for the array.
     split: int or None, optional
         The axis along which the array is split and distributed, defaults to no distribution).
     factory : function
         Function that creates a DNDarray.
     device : str
-        Specifies the :class:`~heat.core.devices.Device` the array shall be allocated on, defaults to globally set
-        default device.
+        Specifies the :class:`~heat.core.devices.Device` the array shall be allocated on, defaults to the same device as ``a``.
     comm: Communication
         Handle to the nodes holding distributed parts or copies of this array.
     order: str, optional
         Options: ``'C'`` or ``'F'``. Specifies the memory layout of the newly created array. Default is ``order='C'``,
         meaning the array will be stored in row-major order (C-like). If ``order=‘F’``, the array will be stored in
         column-major order (Fortran-like).
 
@@ -830,14 +829,21 @@
     if split is None:
         try:
             split = None if isinstance(a, str) else a.split
         except AttributeError:
             # do not split at all
             pass
 
+    # infer the device, otherwise default to a.device
+    if device is None:
+        try:
+            device = a.device
+        except AttributeError:
+            device = devices.get_device()
+
     # use the default communicator, if not set
     comm = sanitize_comm(comm)
 
     return factory(shape, dtype=dtype, split=split, device=device, comm=comm, order=order, **kwargs)
 
 
 def from_partitioned(x, comm: Optional[Communication] = None) -> DNDarray:
@@ -1053,29 +1059,28 @@
     dtype: Type[datatype] = types.float32,
     split: Optional[int] = None,
     device: Optional[Device] = None,
     comm: Optional[Communication] = None,
     order: str = "C",
 ) -> DNDarray:
     """
-    Return a full :class:`~heat.core.dndarray.DNDarray` with the same shape and type as a given array.
+    Return a full :class:`~heat.core.dndarray.DNDarray` with the same shape and type as a given array. Data type, data distribution axis, and device can be explicitly overridden.
 
     Parameters
     ----------
     a : DNDarray
-        The shape and data-type of ``a`` define these same attributes of the returned array.
+        The shape, data-type, split axis and device of ``a`` define these same attributes of the returned array.
     fill_value : scalar
         Fill value.
     dtype : datatype, optional
-        Overrides the data type of the result.
+        The data type of the result, defaults to `a.dtype`.
     split: int or None, optional
-        The axis along which the array is split and distributed; ``None`` means no distribution.
+        The axis along which the array is split and distributed; defaults to `a.split`.
     device : str or Device, optional
-        Specifies the :class:`~heat.core.devices.Device` the array shall be allocated on, defaults to globally set
-        default device.
+        Specifies the :class:`~heat.core.devices.Device` the array shall be allocated on, defaults to `a.device`.
     comm: Communication, optional
         Handle to the nodes holding distributed parts or copies of this array.
     order: str, optional
         Options: ``'C'`` or ``'F'``. Specifies the memory layout of the newly created array. Default is ``order='C'``,
         meaning the array will be stored in row-major order (C-like). If ``order=‘F’``, the array will be stored in
         column-major order (Fortran-like).
 
@@ -1382,27 +1387,26 @@
     split: Optional[int] = None,
     device: Optional[Device] = None,
     comm: Optional[Communication] = None,
     order: str = "C",
 ) -> DNDarray:
     """
     Returns a new :class:`~heat.core.dndarray.DNDarray` filled with ones with the same type,
-    shape and data distribution of given object. Data type and data distribution strategy can be explicitly overriden.
+    shape, data distribution and device of the input object. Data type, data distribution axis, and device can be explicitly overridden.
 
     Parameters
     ----------
     a : DNDarray
-        The shape and data-type of ``a`` define these same attributes of the returned array.
+        The shape, data-type, split axis and device of ``a`` define these same attributes of the returned array.
     dtype : datatype, optional
         Overrides the data type of the result.
     split: int or None, optional
-        The axis along which the array is split and distributed; ``None`` means no distribution.
+        The axis along which the array is split and distributed; defaults to `a.split`.
     device : str or Device, optional
-        Specifies the :class:`~heat.core.devices.Device` the array shall be allocated on, defaults to globally set
-        default device.
+        Specifies the :class:`~heat.core.devices.Device` the array shall be allocated on, defaults to `a.device`.
     comm: Communication, optional
         Handle to the nodes holding distributed parts or copies of this array.
     order: str, optional
         Options: ``'C'`` or ``'F'``. Specifies the memory layout of the newly created array. Default is ``order='C'``,
         meaning the array will be stored in row-major order (C-like). If ``order=‘F’``, the array will be stored in
         column-major order (Fortran-like).
 
@@ -1478,28 +1482,27 @@
     dtype: Optional[Type[datatype]] = None,
     split: Optional[int] = None,
     device: Optional[Device] = None,
     comm: Optional[Communication] = None,
     order: str = "C",
 ) -> DNDarray:
     """
-    Returns a new :class:`~heat.core.dndarray.DNDarray` filled with zeros with the same type, shape and data
-    distribution of given object. Data type and data distribution strategy can be explicitly overriden.
+    Returns a new :class:`~heat.core.dndarray.DNDarray` filled with zeros with the same type, shape, data
+    distribution, and device of the input object. Data type, data distribution axis, and device can be explicitly overridden.
 
     Parameters
     ----------
     a : DNDarray
-        The shape and data-type of ``a`` define these same attributes of the returned array.
+        The shape, data-type, split axis, and device  of ``a`` define these same attributes of the returned array.
     dtype : datatype, optional
         Overrides the data type of the result.
     split: int or None, optional
-        The axis along which the array is split and distributed; ``None`` means no distribution.
+        The axis along which the array is split and distributed; defaults to `a.split`.
     device : str or Device, optional
-        Specifies the :class:`~heat.core.devices.Device` the array shall be allocated on, defaults to globally set
-        default device.
+        Specifies the :class:`~heat.core.devices.Device` the array shall be allocated on, defaults to `a.device`.
     comm: Communication, optional
         Handle to the nodes holding distributed parts or copies of this array.
     order: str, optional
         Options: ``'C'`` or ``'F'``. Specifies the memory layout of the newly created array. Default is ``order='C'``,
         meaning the array will be stored in row-major order (C-like). If ``order=‘F’``, the array will be stored in
         column-major order (Fortran-like).
```

### Comparing `heat-1.4.0/heat/core/indexing.py` & `heat-1.4.1/heat/core/indexing.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/io.py` & `heat-1.4.1/heat/core/io.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/linalg/basics.py` & `heat-1.4.1/heat/core/linalg/basics.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/linalg/qr.py` & `heat-1.4.1/heat/core/linalg/qr.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/linalg/solver.py` & `heat-1.4.1/heat/core/linalg/solver.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/linalg/svd.py` & `heat-1.4.1/heat/core/linalg/svd.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/linalg/svdtools.py` & `heat-1.4.1/heat/core/linalg/svdtools.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/logical.py` & `heat-1.4.1/heat/core/logical.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/manipulations.py` & `heat-1.4.1/heat/core/manipulations.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/memory.py` & `heat-1.4.1/heat/core/memory.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/printing.py` & `heat-1.4.1/heat/core/printing.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/random.py` & `heat-1.4.1/heat/core/random.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/relational.py` & `heat-1.4.1/heat/core/relational.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/rounding.py` & `heat-1.4.1/heat/core/rounding.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/sanitation.py` & `heat-1.4.1/heat/core/sanitation.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/signal.py` & `heat-1.4.1/heat/core/signal.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/statistics.py` & `heat-1.4.1/heat/core/statistics.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/stride_tricks.py` & `heat-1.4.1/heat/core/stride_tricks.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/tiling.py` & `heat-1.4.1/heat/core/tiling.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/trigonometrics.py` & `heat-1.4.1/heat/core/trigonometrics.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/types.py` & `heat-1.4.1/heat/core/types.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/core/version.py` & `heat-1.4.1/heat/core/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module contains Heat's version information."""
 
 major: int = 1
 """Indicates Heat's main version."""
 minor: int = 4
 """Indicates feature extension."""
-micro: int = 0
+micro: int = 1
 """Indicates revisions for bugfixes."""
 extension: str = None
 """Indicates special builds, e.g. for specific hardware."""
 
 if not extension:
     __version__: str = f"{major}.{minor}.{micro}"
     """The combined version string, consisting out of major, minor, micro and possibly extension."""
```

### Comparing `heat-1.4.0/heat/datasets/diabetes.h5` & `heat-1.4.1/heat/datasets/diabetes.h5`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/datasets/iris.csv` & `heat-1.4.1/heat/datasets/iris.csv`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/datasets/iris.h5` & `heat-1.4.1/heat/datasets/iris.h5`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/datasets/iris.nc` & `heat-1.4.1/heat/datasets/iris.nc`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/datasets/iris_X_test.csv` & `heat-1.4.1/heat/datasets/iris_X_test.csv`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/datasets/iris_X_train.csv` & `heat-1.4.1/heat/datasets/iris_X_train.csv`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/datasets/iris_y_pred_proba.csv` & `heat-1.4.1/heat/datasets/iris_y_pred_proba.csv`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/fft/fft.py` & `heat-1.4.1/heat/fft/fft.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/graph/laplacian.py` & `heat-1.4.1/heat/graph/laplacian.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/naive_bayes/gaussianNB.py` & `heat-1.4.1/heat/naive_bayes/gaussianNB.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/nn/__init__.py` & `heat-1.4.1/heat/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/nn/data_parallel.py` & `heat-1.4.1/heat/nn/data_parallel.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/nn/functional.py` & `heat-1.4.1/heat/nn/functional.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/optim/__init__.py` & `heat-1.4.1/heat/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/optim/dp_optimizer.py` & `heat-1.4.1/heat/optim/dp_optimizer.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/optim/utils.py` & `heat-1.4.1/heat/optim/utils.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/preprocessing/preprocessing.py` & `heat-1.4.1/heat/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/regression/lasso.py` & `heat-1.4.1/heat/regression/lasso.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/sparse/_operations.py` & `heat-1.4.1/heat/sparse/_operations.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/sparse/arithmetics.py` & `heat-1.4.1/heat/sparse/arithmetics.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/sparse/dcsr_matrix.py` & `heat-1.4.1/heat/sparse/dcsr_matrix.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/sparse/factories.py` & `heat-1.4.1/heat/sparse/factories.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/sparse/manipulations.py` & `heat-1.4.1/heat/sparse/manipulations.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/spatial/distance.py` & `heat-1.4.1/heat/spatial/distance.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/utils/data/_utils.py` & `heat-1.4.1/heat/utils/data/_utils.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/utils/data/datatools.py` & `heat-1.4.1/heat/utils/data/datatools.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/utils/data/matrixgallery.py` & `heat-1.4.1/heat/utils/data/matrixgallery.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/utils/data/mnist.py` & `heat-1.4.1/heat/utils/data/mnist.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/utils/data/partial_dataset.py` & `heat-1.4.1/heat/utils/data/partial_dataset.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/utils/data/spherical.py` & `heat-1.4.1/heat/utils/data/spherical.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat/utils/vision_transforms.py` & `heat-1.4.1/heat/utils/vision_transforms.py`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/heat.egg-info/PKG-INFO` & `heat-1.4.1/heat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heat
-Version: 1.4.0
+Version: 1.4.1
 Summary: A framework for high-performance data analytics and machine learning.
 Home-page: https://github.com/helmholtz-analytics/heat
 Author: Helmholtz Association
 Author-email: martin.siggel@dlr.de
 Keywords: data,analytics,tensors,distributed,gpu
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -147,15 +147,15 @@
 
 ## Requirements
 
 ### Basics
 - python >= 3.8
 - MPI (OpenMPI, MPICH, Intel MPI, etc.)
 - mpi4py >= 3.0.0
-- pytorch >= 1.8.0
+- pytorch >= 1.11.0
 
 ### Parallel I/O
 - h5py
 - netCDF4
 
 ### GPU support
 In order to do computations on your GPU(s):
@@ -196,15 +196,15 @@
 If you’re unsure where to start or how your skills fit in, reach out! You can ask us here on GitHub, by leaving a comment on a relevant issue that is already open.
 
 **If you are new to contributing to open source, [this guide](https://opensource.guide/how-to-contribute/) helps explain why, what, and how to get involved.**
 
 
 ## Resources
 
-* [Heat Tutorials](https://heat.readthedocs.io/en/latest/tutorials.html)
+* [Heat Tutorials](https://github.com/helmholtz-analytics/heat/tree/main/tutorials)
 * [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html)
 
 ### Parallel Computing and MPI:
 
 * David Henty's [course](https://www.archer2.ac.uk/training/courses/200514-mpi/)
 * Wes Kendall's [Tutorials](https://mpitutorial.com/tutorials/)
 * Rolf Rabenseifner's [MPI course material](https://www.hlrs.de/training/self-study-materials/mpi-course-material) (including C, Fortran **and** Python via `mpi4py`)
```

### Comparing `heat-1.4.0/heat.egg-info/SOURCES.txt` & `heat-1.4.1/heat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heat-1.4.0/setup.py` & `heat-1.4.1/setup.py`

 * *Files identical despite different names*

