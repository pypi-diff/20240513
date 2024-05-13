# Comparing `tmp/rectools-0.5.0.tar.gz` & `tmp/rectools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rectools-0.5.0.tar", max compression
+gzip compressed data, was "rectools-0.6.0.tar", max compression
```

## Comparing `rectools-0.5.0.tar` & `rectools-0.6.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11419 2024-03-22 13:51:02.775607 rectools-0.5.0/LICENSE
--rw-r--r--   0        0        0     7426 2024-03-22 13:51:02.775607 rectools-0.5.0/README.md
--rw-r--r--   0        0        0     3389 2024-03-22 13:51:02.803607 rectools-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1628 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/__init__.py
--rw-r--r--   0        0        0     1089 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/columns.py
--rw-r--r--   0        0        0     2237 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/compat.py
--rw-r--r--   0        0        0     1386 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/dataset/__init__.py
--rw-r--r--   0        0        0     8460 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/dataset/dataset.py
--rw-r--r--   0        0        0    15029 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/dataset/features.py
--rw-r--r--   0        0        0     6971 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/dataset/identifiers.py
--rw-r--r--   0        0        0     6788 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/dataset/interactions.py
--rw-r--r--   0        0        0     6434 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/dataset/torch_datasets.py
--rw-r--r--   0        0        0      973 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/exceptions.py
--rw-r--r--   0        0        0     2058 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/metrics/__init__.py
--rw-r--r--   0        0        0     3128 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/metrics/base.py
--rw-r--r--   0        0        0    18537 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/metrics/classification.py
--rw-r--r--   0        0        0     8238 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/metrics/distances.py
--rw-r--r--   0        0        0     9223 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/metrics/diversity.py
--rw-r--r--   0        0        0     8355 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/metrics/novelty.py
--rw-r--r--   0        0        0     5781 2024-03-22 13:51:02.803607 rectools-0.5.0/rectools/metrics/popularity.py
--rw-r--r--   0        0        0    19863 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/metrics/ranking.py
--rw-r--r--   0        0        0     6670 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/metrics/scoring.py
--rw-r--r--   0        0        0    11698 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/metrics/serendipity.py
--rw-r--r--   0        0        0     1501 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/model_selection/__init__.py
--rw-r--r--   0        0        0     5768 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/model_selection/cross_validate.py
--rw-r--r--   0        0        0     4325 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/model_selection/last_n_split.py
--rw-r--r--   0        0        0     5573 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/model_selection/random_split.py
--rw-r--r--   0        0        0     6065 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/model_selection/splitter.py
--rw-r--r--   0        0        0     5967 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/model_selection/time_split.py
--rw-r--r--   0        0        0     2840 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/model_selection/utils.py
--rw-r--r--   0        0        0     1913 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/__init__.py
--rw-r--r--   0        0        0    12850 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/base.py
--rw-r--r--   0        0        0    14279 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/dssm.py
--rw-r--r--   0        0        0     4410 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/ease.py
--rw-r--r--   0        0        0    16010 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/implicit_als.py
--rw-r--r--   0        0        0     6283 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/implicit_knn.py
--rw-r--r--   0        0        0     5789 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/lightfm.py
--rw-r--r--   0        0        0     8479 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/popular.py
--rw-r--r--   0        0        0    15740 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/popular_in_category.py
--rw-r--r--   0        0        0     2468 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/pure_svd.py
--rw-r--r--   0        0        0     4217 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/random.py
--rw-r--r--   0        0        0     8882 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/rank.py
--rw-r--r--   0        0        0     4047 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/utils.py
--rw-r--r--   0        0        0     5243 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/models/vector.py
--rw-r--r--   0        0        0     1096 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/tools/__init__.py
--rw-r--r--   0        0        0    19499 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/tools/ann.py
--rw-r--r--   0        0        0      902 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/types.py
--rw-r--r--   0        0        0     1493 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/utils/__init__.py
--rw-r--r--   0        0        0     8198 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/utils/array_set_ops.py
--rw-r--r--   0        0        0     3521 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/utils/indexing.py
--rw-r--r--   0        0        0     3745 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/utils/misc.py
--rw-r--r--   0        0        0       18 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/version.py
--rw-r--r--   0        0        0     1205 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/visuals/__init__.py
--rw-r--r--   0        0        0    35655 2024-03-22 13:51:02.807607 rectools-0.5.0/rectools/visuals/visual_app.py
--rw-r--r--   0        0        0    10114 1970-01-01 00:00:00.000000 rectools-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11419 2024-05-13 16:17:32.538353 rectools-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7830 2024-05-13 16:17:32.538353 rectools-0.6.0/README.md
+-rw-r--r--   0        0        0     3491 2024-05-13 16:17:32.562354 rectools-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1628 2024-05-13 16:17:32.562354 rectools-0.6.0/rectools/__init__.py
+-rw-r--r--   0        0        0     1089 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/columns.py
+-rw-r--r--   0        0        0     2237 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/compat.py
+-rw-r--r--   0        0        0     1386 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/dataset/__init__.py
+-rw-r--r--   0        0        0    10175 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/dataset/dataset.py
+-rw-r--r--   0        0        0    15243 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/dataset/features.py
+-rw-r--r--   0        0        0     9070 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/dataset/identifiers.py
+-rw-r--r--   0        0        0     6788 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/dataset/interactions.py
+-rw-r--r--   0        0        0     8226 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/dataset/torch_datasets.py
+-rw-r--r--   0        0        0      973 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/exceptions.py
+-rw-r--r--   0        0        0     2100 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/metrics/__init__.py
+-rw-r--r--   0        0        0     3128 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/metrics/base.py
+-rw-r--r--   0        0        0    19210 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/metrics/classification.py
+-rw-r--r--   0        0        0     8250 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/metrics/distances.py
+-rw-r--r--   0        0        0     9223 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/metrics/diversity.py
+-rw-r--r--   0        0        0     8355 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/metrics/novelty.py
+-rw-r--r--   0        0        0     5781 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/metrics/popularity.py
+-rw-r--r--   0        0        0    19863 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/metrics/ranking.py
+-rw-r--r--   0        0        0     6670 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/metrics/scoring.py
+-rw-r--r--   0        0        0    11698 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/metrics/serendipity.py
+-rw-r--r--   0        0        0     1501 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/model_selection/__init__.py
+-rw-r--r--   0        0        0     6361 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/model_selection/cross_validate.py
+-rw-r--r--   0        0        0     4497 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/model_selection/last_n_split.py
+-rw-r--r--   0        0        0     5745 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/model_selection/random_split.py
+-rw-r--r--   0        0        0     6065 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/model_selection/splitter.py
+-rw-r--r--   0        0        0     6139 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/model_selection/time_split.py
+-rw-r--r--   0        0        0     2840 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/model_selection/utils.py
+-rw-r--r--   0        0        0     1913 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/__init__.py
+-rw-r--r--   0        0        0    21639 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/base.py
+-rw-r--r--   0        0        0    16691 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/dssm.py
+-rw-r--r--   0        0        0     4513 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/ease.py
+-rw-r--r--   0        0        0    16115 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/implicit_als.py
+-rw-r--r--   0        0        0     6448 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/implicit_knn.py
+-rw-r--r--   0        0        0     7329 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/lightfm.py
+-rw-r--r--   0        0        0     9317 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/popular.py
+-rw-r--r--   0        0        0    18281 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/popular_in_category.py
+-rw-r--r--   0        0        0     2533 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/pure_svd.py
+-rw-r--r--   0        0        0     5413 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/random.py
+-rw-r--r--   0        0        0     8963 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/rank.py
+-rw-r--r--   0        0        0     4181 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/utils.py
+-rw-r--r--   0        0        0     5296 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/models/vector.py
+-rw-r--r--   0        0        0     1096 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/tools/__init__.py
+-rw-r--r--   0        0        0    19502 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/tools/ann.py
+-rw-r--r--   0        0        0     1033 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/types.py
+-rw-r--r--   0        0        0     1493 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/utils/__init__.py
+-rw-r--r--   0        0        0     8198 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/utils/array_set_ops.py
+-rw-r--r--   0        0        0     4368 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/utils/indexing.py
+-rw-r--r--   0        0        0     3762 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/utils/misc.py
+-rw-r--r--   0        0        0       18 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/version.py
+-rw-r--r--   0        0        0     1205 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/visuals/__init__.py
+-rw-r--r--   0        0        0    35655 2024-05-13 16:17:32.566354 rectools-0.6.0/rectools/visuals/visual_app.py
+-rw-r--r--   0        0        0    10526 1970-01-01 00:00:00.000000 rectools-0.6.0/PKG-INFO
```

### Comparing `rectools-0.5.0/LICENSE` & `rectools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/README.md` & `rectools-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 - All of the models follow the same interface. **No exceptions**
 - No need for manual creation of sparse matrixes or mapping ids. Preparing data for models is as simple as `dataset = Dataset.construct(interactions_df)`
 - Fitting any model is as simple as `model.fit(dataset)`
 - For getting recommendations `filter_viewed` and `items_to_recommend` options are available
 - For item-to-item recommendations use `recommend_to_items` method
 - For feeding user/item features to model just specify dataframes when constructing `Dataset`. [Check our tutorial](examples/4_dataset_with_features.ipynb)
-
+- For warm / cold inference just provide all required ids in `users` or `target_items` parameters of `recommend` or `recommend_to_items` methods and make sure you have features in the dataset for warm users/items. **Nothing else is needed, everything works out of the box.** Check [documentation](https://rectools.readthedocs.io/en/stable/features.html#models) to see which models support this scenarios.
 
 ## Contribution
 [Contributing guide](CONTRIBUTING.rst)
 
 To install all requirements
 - you must have `python3` and `poetry==1.4.0` installed
 - make sure you have no active virtual environments (deactivate conda `base` if applicable)
```

### Comparing `rectools-0.5.0/pyproject.toml` & `rectools-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "RecTools"
-version = "0.5.0"
+version = "0.6.0"
 description = "An easy-to-use Python library for building recommendation systems"
 license = "Apache-2.0"
 authors = [
     "Emiliy Feldman <feldlime@yandex.ru>",
     "Daria Tikhonovich <daria.m.tikhonovich@gmail.com>",
     "Daniil Potapov <sharth23@gmail.com>",
     "Ildar Safilo <irsafilo@gmail.com>",
@@ -29,57 +29,56 @@
     "machine learning",
     "AI",
     "personalization",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Education",
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 packages = [
     { include = "rectools", from = "." },
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.7.2, <3.11"
-numpy = ">=1.19.5, <2.0.0"
-pandas = [
-    {version = ">=0.25.3, <2.0.0", python = "<3.8"},
-    {version = ">=1.0.0, <3.0.0", python = ">=3.8"}
+python = ">=3.8.1, <3.13"
+numpy = [
+    {version = ">=1.19.5, <2.0.0", python = "3.8"},  # for compatibility with scipy
+    {version = ">=1.22, <2.0.0", python = ">=3.9, <3.12"},
+    {version = ">=1.26, <2.0.0", python = ">=3.12"}  # numpy <1.26 fails to install on Python 3.12
+]
+pandas = ">=1.5.0, <3.0.0"
+scipy = [
+    {version = "^1.9.1, <1.11", python = "3.8"},  # since 1.11 scipy doesn't support python 3.8
+    {version = "^1.10.1, <1.13", python = ">=3.9"},  # in 1.13 were introduced significant changes breaking our logic
 ]
-scipy = "^1.5.4"
 tqdm = "^4.27.0"
 implicit = "^0.7.1"
 attrs = ">=19.1.0,<24.0.0"
-typeguard = "^2.0.1"
+typeguard = "^4.1.0"
 
 
-lightfm = {version = ">=1.16,<=1.17", optional = true}
+lightfm = {version = ">=1.16,<=1.17", python = "<3.12", optional = true}
 
-nmslib = {version = "^2.0.4", optional = true}
+nmslib = {version = "^2.0.4", python = "<3.11", optional = true}
 
-torch = [
-    {version = ">=1.6.0, <2.0.0", python = "<3.8", optional = true},
-    {version = ">=1.6.0, <3.0.0", python = ">=3.8", optional = true}
-]
-pytorch-lightning = [
-    {version = ">=1.6.0, <2.0.0", python = "<3.8", optional = true},
-    {version = ">=1.6.0, <3.0.0", python = ">=3.8", optional = true}
-]
+torch = {version = ">=1.6.0, <3.0.0", optional = true}
+pytorch-lightning = {version = ">=1.6.0, <3.0.0", optional = true}
 
 ipywidgets = {version = ">=7.7,<8.2", optional = true}
 
 
 [tool.poetry.extras]
 lightfm = ["lightfm"]
 nmslib = ["nmslib"]
@@ -88,36 +87,35 @@
 all = [
     "lightfm",
     "nmslib", 
     "torch", "pytorch-lightning",
     "ipywidgets"
 ]
 
+
 [tool.poetry.group.dev.dependencies]
-black = "22.3.0"
-isort = "5.10.1"
-pylint = "2.17.6"
-mypy = [
-    {version = "0.931", python = "<3.8"},  # not compatible with torch >= 2
-    {version = "1.6.1", python = ">=3.8"}  # not compatible with python 3.7
-]
-flake8 = "4.0.1"
-bandit = "1.7.4"
-pytest = "7.1.2"
-radon = "5.1.0"
-coverage = "6.4.2"
-autopep8 = "1.6.0"
-codespell = "2.1.0"
-pytest-subtests = "0.8.0"
-flake8-docstrings = "1.6.0"
-pep8-naming = "0.12.1"
-pytest-cov = "2.12.1"
-pytest-mock = "3.11.1"
+black = "24.4.2"
+isort = "5.13.2"
+pylint = "3.1.0"
+mypy = "1.10.0"
+flake8 = "7.0.0"
+bandit = "1.7.8"
+pytest = "8.1.1"
+radon = "6.0.1"
+coverage = "7.5.0"
+autopep8 = "2.1.0"
+codespell = "2.2.6"
+pytest-subtests = "0.12.1"
+flake8-docstrings = "1.7.0"
+pep8-naming = "0.13.3"
+pytest-cov = "5.0.0"
+pytest-mock = "3.14.0"
 
 
 [tool.black]
 line-length = 120
-target-version = ["py37", "py38", "py39", "py310"]
+target-version = ["py38", "py39", "py310", "py311", "py312"]
+
 
 [build-system]
 requires = ["poetry>=1.0.5"]
 build-backend = "poetry.masonry.api"
```

### Comparing `rectools-0.5.0/rectools/__init__.py` & `rectools-0.6.0/rectools/__init__.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/columns.py` & `rectools-0.6.0/rectools/columns.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/compat.py` & `rectools-0.6.0/rectools/compat.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/dataset/__init__.py` & `rectools-0.6.0/rectools/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/dataset/dataset.py` & `rectools-0.6.0/rectools/dataset/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 
 import attr
 import pandas as pd
 from scipy import sparse
 
 from rectools import Columns
 
-from .features import AbsentIdError, DenseFeatures, Features, SparseFeatures, UnknownIdError
+from .features import AbsentIdError, DenseFeatures, Features, SparseFeatures
 from .identifiers import IdMap
 from .interactions import Interactions
 
 
 @attr.s(slots=True, frozen=True)
 class Dataset:
     """
     Container class for all data for a recommendation model.
 
     It stores data about internal-external id mapping,
     user-item interactions, user and item features
     in special `rectools` structures for convenient future usage.
 
-    This is data class, so you can create it explicitly, but
-    it's recommended to use `construct` method.
+    WARNING: It's highly not recommended to create `Dataset` object directly.
+    Use `construct` class method instead.
 
     Parameters
     ----------
     user_id_map : IdMap
         User identifiers mapping.
     item_id_map : IdMap
         Item identifiers mapping.
@@ -55,14 +55,46 @@
 
     user_id_map: IdMap = attr.ib()
     item_id_map: IdMap = attr.ib()
     interactions: Interactions = attr.ib()
     user_features: tp.Optional[Features] = attr.ib(default=None)
     item_features: tp.Optional[Features] = attr.ib(default=None)
 
+    @property
+    def n_hot_users(self) -> int:
+        """
+        Return number of hot users in dataset.
+        Users with internal ids from `0` to `n_hot_users - 1` are hot (they are present in interactions).
+        Users with internal ids from `n_hot_users` to `dataset.user_id_map.size - 1` are warm
+        (they aren't present in interactions, but they have features).
+        """
+        return self.interactions.df[Columns.User].max() + 1
+
+    @property
+    def n_hot_items(self) -> int:
+        """
+        Return number of hot items in dataset.
+        Items with internal ids from `0` to `n_hot_items - 1` are hot (they are present in interactions).
+        Items with internal ids from `n_hot_items` to `dataset.item_id_map.size - 1` are warm
+        (they aren't present in interactions, but they have features).
+        """
+        return self.interactions.df[Columns.Item].max() + 1
+
+    def get_hot_user_features(self) -> tp.Optional[Features]:
+        """User features for hot users."""
+        if self.user_features is None:
+            return None
+        return self.user_features.take(range(self.n_hot_users))
+
+    def get_hot_item_features(self) -> tp.Optional[Features]:
+        """Item features for hot items."""
+        if self.item_features is None:
+            return None
+        return self.item_features.take(range(self.n_hot_items))
+
     @classmethod
     def construct(
         cls,
         interactions_df: pd.DataFrame,
         user_features_df: tp.Optional[pd.DataFrame] = None,
         cat_user_features: tp.Iterable[str] = (),
         make_dense_user_features: bool = False,
@@ -108,23 +140,24 @@
         """
         for col in (Columns.User, Columns.Item):
             if col not in interactions_df:
                 raise KeyError(f"Column '{col}' must be present in `interactions_df`")
         user_id_map = IdMap.from_values(interactions_df[Columns.User].values)
         item_id_map = IdMap.from_values(interactions_df[Columns.Item].values)
         interactions = Interactions.from_raw(interactions_df, user_id_map, item_id_map)
-        user_features = cls._make_features(
+
+        user_features, user_id_map = cls._make_features(
             user_features_df,
             cat_user_features,
             make_dense_user_features,
             user_id_map,
             Columns.User,
             "user",
         )
-        item_features = cls._make_features(
+        item_features, item_id_map = cls._make_features(
             item_features_df,
             cat_item_features,
             make_dense_item_features,
             item_id_map,
             Columns.Item,
             "item",
         )
@@ -134,66 +167,75 @@
     def _make_features(
         df: tp.Optional[pd.DataFrame],
         cat_features: tp.Iterable[str],
         make_dense: bool,
         id_map: IdMap,
         possible_id_col: str,
         feature_type: str,
-    ) -> tp.Optional[Features]:
+    ) -> tp.Tuple[tp.Optional[Features], IdMap]:
         if df is None:
-            return None
+            return None, id_map
 
         id_col = possible_id_col if possible_id_col in df else "id"
+        id_map = id_map.add_ids(df[id_col].values, raise_if_already_present=False)
 
         if make_dense:
             try:
-                return DenseFeatures.from_dataframe(df, id_map, id_col=id_col)
-            except UnknownIdError:
-                raise ValueError(f"Some ids from {feature_type} features table not present in interactions")
+                return DenseFeatures.from_dataframe(df, id_map, id_col=id_col), id_map
             except AbsentIdError:
                 raise ValueError(
                     f"An error has occurred while constructing {feature_type} features: "
-                    "When using dense features all ids from interactions must present in features table"
+                    "When using dense features all ids from interactions must be present in features table"
                 )
             except Exception as e:  # pragma: no cover
                 raise RuntimeError(f"An error has occurred while constructing {feature_type} features: {e!r}")
+
         try:
-            return SparseFeatures.from_flatten(df, id_map, cat_features, id_col=id_col)
-        except UnknownIdError:
-            raise ValueError(f"Some ids from {feature_type} features table not present in interactions")
+            return SparseFeatures.from_flatten(df, id_map, cat_features, id_col=id_col), id_map
         except Exception as e:  # pragma: no cover
             raise RuntimeError(f"An error has occurred while constructing {feature_type} features: {e!r}")
 
-    def get_user_item_matrix(self, include_weights: bool = True) -> sparse.csr_matrix:
+    def get_user_item_matrix(
+        self,
+        include_weights: bool = True,
+        include_warm_users: bool = False,
+        include_warm_items: bool = False,
+    ) -> sparse.csr_matrix:
         """
         Construct user-item CSR matrix based on `interactions` attribute.
 
         Return a resized user-item matrix.
         Resizing is done using `user_id_map` and `item_id_map`,
         hence if either a user or an item is not presented in interactions,
         but presented in id map, then it's going to be in the returned matrix.
 
         Parameters
         ----------
         include_weights : bool, default ``True``
              Whether include interaction weights in matrix or not.
              If False, all values in returned matrix will be equal to ``1``.
+        include_warm : bool, default ``False``
+            Whether to include warm users and items into the matrix or not.
+            Rows and columns for warm users and items will be added to the end of matrix,
+            they will contain only zeros.
 
         Returns
         -------
         csr_matrix
             Resized user-item CSR matrix
         """
         matrix = self.interactions.get_user_item_matrix(include_weights)
-        matrix.resize(self.user_id_map.internal_ids.size, self.item_id_map.internal_ids.size)
+        n_rows = self.user_id_map.size if include_warm_users else matrix.shape[0]
+        n_columns = self.item_id_map.size if include_warm_items else matrix.shape[1]
+        matrix.resize(n_rows, n_columns)
         return matrix
 
     def get_raw_interactions(self, include_weight: bool = True, include_datetime: bool = True) -> pd.DataFrame:
         """
-        Return iteractions as a `pd.DataFrame` object with replacing internal user and item ids to external ones.
+        Return interactions as a `pd.DataFrame` object with replacing internal user and item ids to external ones.
 
         Parameters
         ----------
         include_weight : bool, default ``True``
             Whether to include weight column into resulting table or not.
         include_datetime : bool, default ``True``
             Whether to include datetime column into resulting table or not.
```

### Comparing `rectools-0.5.0/rectools/dataset/features.py` & `rectools-0.6.0/rectools/dataset/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,18 @@
 
         """
         return DenseFeatures(
             values=self.values[ids],
             names=self.names,
         )
 
+    def __len__(self) -> int:
+        """Return number of objects."""
+        return self.values.shape[0]
+
 
 SparseFeatureName = tp.Tuple[str, tp.Any]
 
 
 @attr.s(slots=True, frozen=True)
 class SparseFeatures:
     """
@@ -438,9 +442,13 @@
         SparseFeatures
         """
         return SparseFeatures(
             values=self.values[ids],
             names=self.names,
         )
 
+    def __len__(self) -> int:
+        """Return number of objects."""
+        return self.values.shape[0]
+
 
 Features = tp.Union[DenseFeatures, SparseFeatures]
```

### Comparing `rectools-0.5.0/rectools/dataset/identifiers.py` & `rectools-0.6.0/rectools/dataset/identifiers.py`

 * *Files 17% similar despite different names*

```diff
@@ -94,14 +94,19 @@
 
     @property
     def size(self) -> int:
         """Return number of ids in map."""
         return self.external_ids.size
 
     @property
+    def external_dtype(self) -> tp.Type:
+        """Return dtype of external ids."""
+        return self.external_ids.dtype
+
+    @property
     def to_internal(self) -> pd.Series:
         """Map internal->external."""
         return pd.Series(np.arange(self.size), index=self.external_ids)
 
     @property
     def to_external(self) -> pd.Series:
         """Map internal->external."""
@@ -116,65 +121,109 @@
         """Return array of sorted internal ids."""
         return self.internal_ids
 
     def get_external_sorted_by_internal(self) -> np.ndarray:
         """Return array of external ids sorted by internal ids."""
         return self.external_ids
 
-    def convert_to_internal(self, external: ExternalIds, strict: bool = True) -> np.ndarray:
+    @tp.overload
+    def convert_to_internal(  # noqa: D102
+        self, external: ExternalIds, strict: bool = ..., return_missing: tp.Literal[False] = False
+    ) -> np.ndarray:  # pragma: no cover
+        ...
+
+    @tp.overload
+    def convert_to_internal(  # noqa: D102
+        self, external: ExternalIds, strict: bool = ..., *, return_missing: tp.Literal[True]
+    ) -> tp.Tuple[np.ndarray, np.ndarray]:  # pragma: no cover
+        ...
+
+    def convert_to_internal(
+        self, external: ExternalIds, strict: bool = True, return_missing: bool = False
+    ) -> tp.Union[np.ndarray, tp.Tuple[np.ndarray, np.ndarray]]:
         """
         Convert any sequence of external ids to array of internal ids (map external -> internal).
 
         Parameters
         ----------
         external : sequence(hashable)
             Sequence of external ids to convert.
         strict : bool, default ``True``
              Defines behaviour when some of given external ids do not exist in mapping.
                 - If ``True``, `KeyError` will be raised;
                 - If ``False``, nonexistent ids will be skipped.
+        return_missing : bool, default ``False``
+            If True, return a tuple of 2 arrays: internal ids and missing ids (that are not in map).
+            Works only if `strict` is False.
 
         Returns
         -------
         np.ndarray
             Array of internal ids.
+        np.ndarray, np.ndarray
+            Tuple of 2 arrays: internal ids and missing ids.
+            Only if `strict` is False and `return_missing` is True.
 
         Raises
         ------
         KeyError
             If some of given external ids do not exist in mapping and `strict` flag is ``True``.
+        ValueError
+            If `strict` and `return_missing` are both ``True``.
         """
-        internal = get_from_series_by_index(self.to_internal, external, strict)
-        return internal
+        result = get_from_series_by_index(self.to_internal, external, strict, return_missing)
+        return result
 
-    def convert_to_external(self, internal: InternalIds, strict: bool = True) -> np.ndarray:
+    @tp.overload
+    def convert_to_external(  # noqa: D102
+        self, internal: InternalIds, strict: bool = ..., return_missing: tp.Literal[False] = False
+    ) -> np.ndarray:  # pragma: no cover
+        ...
+
+    @tp.overload
+    def convert_to_external(  # noqa: D102
+        self, internal: InternalIds, strict: bool = ..., *, return_missing: tp.Literal[True]
+    ) -> tp.Tuple[np.ndarray, np.ndarray]:  # pragma: no cover
+        ...
+
+    def convert_to_external(
+        self, internal: InternalIds, strict: bool = True, return_missing: bool = False
+    ) -> tp.Union[np.ndarray, tp.Tuple[np.ndarray, np.ndarray]]:
         """
         Convert any sequence of internal ids to array of external ids (map internal -> external).
 
         Parameters
         ----------
         internal : sequence(int)
             Sequence of internal ids to convert.
         strict : bool, default ``True``
              Defines behaviour when some of given internal ids do not exist in mapping.
                 - If ``True``, `KeyError` will be raised;
                 - If ``False``, nonexistent ids will be skipped.
+        return_missing : bool, default ``False``
+            If True, return a tuple of 2 arrays: external ids and missing ids (that are not in map).
+            Works only if `strict` is False.
 
         Returns
         -------
         np.ndarray
             Array of external ids.
+        np.ndarray, np.ndarray
+            Tuple of 2 arrays: external ids and missing ids.
+            Only if `strict` is False and `return_missing` is True.
 
         Raises
         ------
         KeyError
             If some of given internal ids do not exist in mapping and `strict` flag is True.
+        ValueError
+            If `strict` and `return_missing` are both ``True``.
         """
-        external = get_from_series_by_index(self.to_external, internal, strict)
-        return external
+        result = get_from_series_by_index(self.to_external, internal, strict, return_missing)
+        return result
 
     def add_ids(self, values: ExternalIds, raise_if_already_present: bool = False) -> "IdMap":
         """
         Add new external ids to current IdMap and return new IdMap.
         Mapping for old ids does not change.
         New ids are added to the end of list of external ids.
```

### Comparing `rectools-0.5.0/rectools/dataset/interactions.py` & `rectools-0.6.0/rectools/dataset/interactions.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/dataset/torch_datasets.py` & `rectools-0.6.0/rectools/dataset/torch_datasets.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,20 +21,31 @@
 import numpy as np
 import torch
 from scipy import sparse
 from torch.utils.data import Dataset as TorchDataset
 
 from .dataset import Dataset
 
-DD = tp.TypeVar("DD", bound="DSSMDataset")
-ID = tp.TypeVar("ID", bound="ItemFeaturesDataset")
-UD = tp.TypeVar("UD", bound="UserFeaturesDataset")
+DSSMTrainDatasetT = tp.TypeVar("DSSMTrainDatasetT", bound="DSSMTrainDatasetBase")
+DSSMItemDatasetT = tp.TypeVar("DSSMItemDatasetT", bound="DSSMItemDatasetBase")
+DSSMUserDatasetT = tp.TypeVar("DSSMUserDatasetT", bound="DSSMUserDatasetBase")
 
 
-class DSSMDataset(TorchDataset[tp.Any]):
+class DSSMTrainDatasetBase(TorchDataset[tp.Any]):
+    """Base class for DSSM training datasets. Used only for type hinting."""
+
+    def __init__(self, *args: tp.Any, **kwargs: tp.Any) -> None:
+        raise NotImplementedError()
+
+    @classmethod
+    def from_dataset(cls: tp.Type[DSSMTrainDatasetT], dataset: Dataset) -> DSSMTrainDatasetT:
+        raise NotImplementedError()
+
+
+class DSSMTrainDataset(DSSMTrainDatasetBase):
     """
     Torch dataset wrapper for `rectools.dataset.dataset.Dataset`.
     Implements `torch.utils.data.Dataset` for subsequent usage with
     `torch.utils.data.DataLoader`. Does the following: for a given index
     takes a row of user interactions, a row of user features and samples
     one positive and one negative items and then returns them as tensors.
 
@@ -64,25 +75,25 @@
             raise ValueError(
                 "Impossible to sample from a row that either contains only negative items"
                 " or contains any negatively signed integers."
                 "Make sure that all rows from interactions have at least 1 positive item"
             )
 
     @classmethod
-    def from_dataset(cls: tp.Type[DD], dataset: Dataset) -> DD:
+    def from_dataset(cls: tp.Type[DSSMTrainDatasetT], dataset: Dataset) -> DSSMTrainDatasetT:
         ui_matrix = dataset.get_user_item_matrix()
-        if dataset.item_features is not None:
-            item_features = dataset.item_features.get_sparse()
-        else:
+
+        # We take hot here since this dataset is used for fit only
+        item_features = dataset.get_hot_item_features()
+        user_features = dataset.get_hot_user_features()
+        if item_features is None:
             raise AttributeError("Item features attribute of dataset could not be None")
-        if dataset.user_features is not None:
-            user_features = dataset.user_features.get_sparse()
-        else:
+        if user_features is None:
             raise AttributeError("User features attribute of dataset could not be None")
-        return cls(items=item_features, users=user_features, interactions=ui_matrix)
+        return cls(items=item_features.get_sparse(), users=user_features.get_sparse(), interactions=ui_matrix)
 
     def __len__(self) -> int:
         return self.interactions.shape[0]
 
     def __getitem__(
         self, idx: int
     ) -> tp.Tuple[torch.FloatTensor, torch.FloatTensor, torch.FloatTensor, torch.FloatTensor]:
@@ -95,41 +106,68 @@
         interactions = torch.FloatTensor(interactions_vec)
         pos = torch.FloatTensor(self.items[pos_i].toarray().flatten())
         neg = torch.FloatTensor(self.items[neg_i].toarray().flatten())
 
         return user_features, interactions, pos, neg
 
 
-class ItemFeaturesDataset(TorchDataset[tp.Any]):
+class DSSMItemDatasetBase(TorchDataset[tp.Any]):
+    """Base class for DSSM item datasets. Used only for type hinting."""
+
+    def __init__(self, *args: tp.Any, **kwargs: tp.Any) -> None:
+        raise NotImplementedError()
+
+    @classmethod
+    def from_dataset(cls: tp.Type[DSSMItemDatasetT], dataset: Dataset) -> DSSMItemDatasetT:
+        raise NotImplementedError()
+
+
+class DSSMItemDataset(DSSMItemDatasetBase):
     """
     Torch dataset wrapper for `rectools.dataset.dataset.Dataset`.
     Implements `torch.utils.data.Dataset` for subsequent usage with
     `torch.utils.data.DataLoader`. Does the following: for a given index
     takes a row of item features and then returns them as tensors.
 
     This class is intended for internal usage or advanced users.
     """
 
     def __init__(self, items: sparse.csr_matrix):
         self.items = items
 
     @classmethod
-    def from_dataset(cls: tp.Type[ID], dataset: Dataset) -> ID:
+    def from_dataset(cls: tp.Type[DSSMItemDatasetT], dataset: Dataset) -> DSSMItemDatasetT:
+        # We take all features here since this dataset is used for recommend only, not for fit
         if dataset.item_features is not None:
             return cls(dataset.item_features.get_sparse())
         raise AttributeError("Item features attribute of dataset could not be None")
 
     def __len__(self) -> int:
         return self.items.shape[0]
 
     def __getitem__(self, idx: int) -> torch.FloatTensor:
         return torch.FloatTensor(self.items[idx].toarray().flatten())
 
 
-class UserFeaturesDataset(TorchDataset[tp.Any]):
+class DSSMUserDatasetBase(TorchDataset[tp.Any]):
+    """Base class for DSSM training datasets. Used only for type hinting."""
+
+    def __init__(self, *args: tp.Any, **kwargs: tp.Any) -> None:
+        raise NotImplementedError()
+
+    @classmethod
+    def from_dataset(
+        cls: tp.Type[DSSMUserDatasetT],
+        dataset: Dataset,
+        keep_users: tp.Optional[tp.Sequence[int]] = None,
+    ) -> DSSMUserDatasetT:
+        raise NotImplementedError()
+
+
+class DSSMUserDataset(DSSMUserDatasetBase):
     """
     Torch dataset wrapper for `rectools.dataset.dataset.Dataset`.
     Implements `torch.utils.data.Dataset` for subsequent usage with
     `torch.utils.data.DataLoader`. Does the following: for a given index
     takes a row of user interactions, a row of user features and then
     returns them as tensors.
 
@@ -138,31 +176,34 @@
 
     def __init__(
         self,
         users: sparse.csr_matrix,
         interactions: sparse.csr_matrix,
         keep_users: tp.Optional[tp.Sequence[int]] = None,
     ):
+        if users.shape[0] != interactions.shape[0]:
+            raise ValueError("Number of rows in user features matrix and in interactions matrix must be the same")
         if keep_users is not None:
             self.users = users[keep_users]
             self.interactions = interactions[keep_users]
         else:
             self.users = users
             self.interactions = interactions
 
     @classmethod
     def from_dataset(
-        cls: tp.Type[UD],
+        cls: tp.Type[DSSMUserDatasetT],
         dataset: Dataset,
         keep_users: tp.Optional[tp.Sequence[int]] = None,
-    ) -> UD:
+    ) -> DSSMUserDatasetT:
+        # We take all features here since this dataset is used for recommend only, not for fit
         if dataset.user_features is not None:
             return cls(
                 dataset.user_features.get_sparse(),
-                dataset.get_user_item_matrix(),
+                dataset.get_user_item_matrix(include_warm_users=True),
                 keep_users,
             )
         raise AttributeError("User features attribute of dataset could not be None")
 
     def __len__(self) -> int:
         return self.users.shape[0]
```

### Comparing `rectools-0.5.0/rectools/exceptions.py` & `rectools-0.6.0/rectools/exceptions.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/metrics/__init__.py` & `rectools-0.6.0/rectools/metrics/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,24 +29,25 @@
 `metrics.MAP`
 `metrics.NDCG`
 `metrics.MRR`
 `metrics.MeanInvUserFreq`
 `metrics.IntraListDiversity`
 `metrics.AvgRecPopularity`
 `metrics.Serendipity`
+`metrics.HitRate`
 
 Tools
 -----
 `metrics.calc_metrics` - calculate a set of metrics efficiently
 `metrics.PairwiseDistanceCalculator`
 `metrics.PairwiseHammingDistanceCalculator`
 `metrics.SparsePairwiseHammingDistanceCalculator`
 """
 
-from .classification import MCC, Accuracy, F1Beta, Precision, Recall
+from .classification import MCC, Accuracy, F1Beta, HitRate, Precision, Recall
 from .distances import (
     PairwiseDistanceCalculator,
     PairwiseHammingDistanceCalculator,
     SparsePairwiseHammingDistanceCalculator,
 )
 from .diversity import IntraListDiversity
 from .novelty import MeanInvUserFreq
@@ -57,14 +58,15 @@
 
 __all__ = (
     "Precision",
     "Recall",
     "F1Beta",
     "Accuracy",
     "MCC",
+    "HitRate",
     "MAP",
     "NDCG",
     "MRR",
     "MeanInvUserFreq",
     "IntraListDiversity",
     "AvgRecPopularity",
     "Serendipity",
```

### Comparing `rectools-0.5.0/rectools/metrics/base.py` & `rectools-0.6.0/rectools/metrics/base.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/metrics/classification.py` & `rectools-0.6.0/rectools/metrics/classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -367,14 +367,34 @@
         mcc_numerator = tp_ * tn_ - fp_ * fn_
         mcc_denominator = np.sqrt((tp_ + fp_) * (tp_ + fn_) * (tn_ + fp_) * (tn_ + fn_))
         mcc = mcc_numerator / mcc_denominator
         mcc.loc[mcc_denominator == 0.0] = 0.0  # if denominator == 0 than numerator is also equals 0
         return mcc
 
 
+@attr.s
+class HitRate(SimpleClassificationMetric):
+    """
+    HitRate calculates the fraction of users for which the correct answer is included in the recommendation list.
+
+    The HitRate equals to ``1 if tp > 0, otherwise 0`` where
+        - ``tp`` is the number of relevant recommendations
+          among the first ``k`` items in recommendation list.
+
+    Parameters
+    ----------
+    k : int
+        Number of items in top of recommendations list that will be used to calculate metric.
+    """
+
+    def _calc_per_user_from_confusion_df(self, confusion_df: pd.DataFrame) -> pd.Series:
+        hit_rate = (confusion_df[TP] > 0).astype(float)
+        return hit_rate
+
+
 def calc_classification_metrics(
     metrics: tp.Dict[str, tp.Union[ClassificationMetric, SimpleClassificationMetric]],
     merged: pd.DataFrame,
     catalog: tp.Optional[Catalog] = None,
 ) -> tp.Dict[str, float]:
     """
     Calculate any classification metrics.
```

### Comparing `rectools-0.5.0/rectools/metrics/distances.py` & `rectools-0.6.0/rectools/metrics/distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
     def __init__(self, features: SparseFeatures, id_map: IdMap) -> None:
         self.features = features.values.copy()
         self.mapper = deepcopy(id_map)
 
     def _get_distances_for_item_pairs(self, items_0: ExternalIds, items_1: ExternalIds) -> Distances:
         # Create accumulator for result
-        result = np.empty(len(items_0), dtype=np.float32)
+        result: np.ndarray = np.empty(len(items_0), dtype=np.float32)
         # Find mask external ids that are not contained in the mapper
         existing_external_0 = fast_isin(np.asarray(items_0), self.mapper.external_ids)
         existing_external_1 = fast_isin(np.asarray(items_1), self.mapper.external_ids)
         existing_mask = np.logical_and(existing_external_0, existing_external_1)
         # Check absence items ids in mapper
         if not existing_mask.all():
             warnings.warn("Some items absent in mapper. Corresponding pair distances are set to NaN.")
```

### Comparing `rectools-0.5.0/rectools/metrics/diversity.py` & `rectools-0.6.0/rectools/metrics/diversity.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/metrics/novelty.py` & `rectools-0.6.0/rectools/metrics/novelty.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/metrics/popularity.py` & `rectools-0.6.0/rectools/metrics/popularity.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/metrics/ranking.py` & `rectools-0.6.0/rectools/metrics/ranking.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/metrics/scoring.py` & `rectools-0.6.0/rectools/metrics/scoring.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/metrics/serendipity.py` & `rectools-0.6.0/rectools/metrics/serendipity.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/model_selection/__init__.py` & `rectools-0.6.0/rectools/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/model_selection/cross_validate.py` & `rectools-0.6.0/rectools/model_selection/cross_validate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as tp
-import warnings
 
+import numpy as np
 import pandas as pd
 
 from rectools.columns import Columns
 from rectools.dataset import Dataset, Features, IdMap, Interactions
 from rectools.metrics import calc_metrics
 from rectools.metrics.base import MetricAtK
 from rectools.models.base import ModelBase
@@ -13,28 +13,39 @@
 from .splitter import Splitter
 
 
 def _gen_2x_internal_ids_dataset(
     interactions_internal_df: pd.DataFrame,
     user_features: tp.Optional[Features],
     item_features: tp.Optional[Features],
+    prefer_warm_inference_over_cold: bool,
 ) -> Dataset:
     """
     Make new dataset based on given interactions and features from base dataset.
     Assume that interactions dataframe contains internal ids.
     Returned dataset contains 2nd level of internal ids.
     """
     user_id_map = IdMap.from_values(interactions_internal_df[Columns.User].values)  # 1x internal -> 2x internal
     item_id_map = IdMap.from_values(interactions_internal_df[Columns.Item].values)  # 1x internal -> 2x internal
     interactions_train = Interactions.from_raw(interactions_internal_df, user_id_map, item_id_map)  # 2x internal
-    user_features_new = item_features_new = None
-    if user_features is not None:
-        user_features_new = user_features.take(user_id_map.get_external_sorted_by_internal())  # 2x internal
-    if item_features is not None:
-        item_features_new = item_features.take(item_id_map.get_external_sorted_by_internal())  # 2x internal
+
+    def _handle_features(features: tp.Optional[Features], id_map: IdMap) -> tp.Tuple[tp.Optional[Features], IdMap]:
+        if features is None:
+            return None, id_map
+
+        if prefer_warm_inference_over_cold:
+            all_features_ids = np.arange(len(features))  # 1x internal
+            id_map = id_map.add_ids(all_features_ids, raise_if_already_present=False)
+
+        features = features.take(id_map.get_external_sorted_by_internal())  # 2x internal
+        return features, id_map
+
+    user_features_new, user_id_map = _handle_features(user_features, user_id_map)
+    item_features_new, item_id_map = _handle_features(item_features, item_id_map)
+
     dataset = Dataset(
         user_id_map=user_id_map,
         item_id_map=item_id_map,
         interactions=interactions_train,
         user_features=user_features_new,
         item_features=item_features_new,
     )
@@ -45,14 +56,15 @@
     dataset: Dataset,
     splitter: Splitter,
     metrics: tp.Dict[str, MetricAtK],
     models: tp.Dict[str, ModelBase],
     k: int,
     filter_viewed: bool,
     items_to_recommend: tp.Optional[ExternalIds] = None,
+    prefer_warm_inference_over_cold: bool = True,
 ) -> tp.Dict[str, tp.Any]:
     """
     Run cross validation on multiple models with multiple metrics.
 
     Parameters
     ----------
     dataset : Dataset
@@ -69,14 +81,19 @@
         Derived number of recommendations for every user.
         For some models actual number of recommendations may be less than `k`.
     filter_viewed : bool
         Whether to filter from recommendations items that user has already interacted with.
     items_to_recommend : array-like, optional, default None
         Whitelist of external item ids.
         If given, only these items will be used for recommendations.
+    prefer_warm_inference_over_cold : bool, default True
+        Whether to keep features for test users and items that were not present in train.
+        Set to `True` to enable "warm" recommendations for all applicable models.
+        Set to `False` to treat all new users and items as "cold" and not to provide features for them.
+        If new users and items are filtered from test in splitter, this argument has no effect.
 
     Returns
     -------
     dict
         Dictionary with structure
         {
             "splits": [
@@ -88,35 +105,30 @@
                 {"model": "model_1", "i_split": 0, <metrics>},
                 {"model": "model_2", "i_split": 0, <metrics>},
                 {"model": "model_1", "i_split": 1, <metrics>},
                 ...
             ]
         }
     """
-    if not splitter.filter_cold_users:  # TODO: remove when cold users support added
-        warnings.warn(
-            "Currently models do not support recommendations for cold users. "
-            "Set `filter_cold_users` to `False` only for custom models. "
-            "Otherwise you will get `KeyError`."
-        )
-
     interactions = dataset.interactions
 
     split_iterator = splitter.split(interactions, collect_fold_stats=True)
 
     split_infos = []
     metrics_all = []
 
     for train_ids, test_ids, split_info in split_iterator:
         split_infos.append(split_info)
 
         interactions_df_train = interactions.df.iloc[train_ids]  # 1x internal
         # We need to avoid fitting models on sparse matrices with all zero rows/columns =>
         # => we need to create a fold dataset which contains only hot users and items for current training
-        fold_dataset = _gen_2x_internal_ids_dataset(interactions_df_train, dataset.user_features, dataset.item_features)
+        fold_dataset = _gen_2x_internal_ids_dataset(
+            interactions_df_train, dataset.user_features, dataset.item_features, prefer_warm_inference_over_cold
+        )
 
         interactions_df_test = interactions.df.iloc[test_ids]  # 1x internal
         test_users = interactions_df_test[Columns.User].unique()  # 1x internal
         catalog = interactions_df_train[Columns.Item].unique()  # 1x internal
 
         if items_to_recommend is not None:
             item_ids_to_recommend = dataset.item_id_map.convert_to_internal(
```

### Comparing `rectools-0.5.0/rectools/model_selection/last_n_split.py` & `rectools-0.6.0/rectools/model_selection/last_n_split.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,19 +40,21 @@
     Parameters
     ----------
     n : int
         Number of interactions for each user that will be included in test.
     n_splits : int, default 1
         Number of test folds.
     filter_cold_users : bool, default ``True``
-        If `True`, users that not in train will be excluded from test.
+        If `True`, users that are not present in train will be excluded from test.
+        WARNING: both cold and warm users will be excluded from test.
     filter_cold_items : bool, default ``True``
-        If `True`, items that not in train will be excluded from test.
+        If `True`, items that are not present in train will be excluded from test.
+        WARNING: both cold and warm items will be excluded from test.
     filter_already_seen : bool, default ``True``
-        If ``True``, pairs (user, item) that are in train will be excluded from test.
+        If ``True``, pairs (user, item) that are present in train will be excluded from test.
 
     Examples
     --------
     >>> from rectools import Columns
     >>> df = pd.DataFrame(
     ...     [
     ...         [1, 1, 1, "2021-09-01"], # 0
```

### Comparing `rectools-0.5.0/rectools/model_selection/random_split.py` & `rectools-0.6.0/rectools/model_selection/random_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,19 +40,21 @@
     test_fold_frac : float
         Relative size of test part, must be between 0. and 1.
     n_splits : int, default 1
         Number of test folds.
     random_state : int, default  None,
         Controls randomness of each fold. Pass an int to get reproducible result across multiple `split` calls.
     filter_cold_users : bool, default ``True``
-        If `True`, users that not in train will be excluded from test.
+        If `True`, users that are not present in train will be excluded from test.
+        WARNING: both cold and warm users will be excluded from test.
     filter_cold_items : bool, default ``True``
-        If `True`, items that not in train will be excluded from test.
+        If `True`, items that are not present in train will be excluded from test.
+        WARNING: both cold and warm items will be excluded from test.
     filter_already_seen : bool, default ``True``
-        If `True`, pairs (user, item) that are in train will be excluded from test.
+        If `True`, pairs (user, item) that are present in train will be excluded from test.
 
     Examples
     --------
     >>> from rectools import Columns
     >>> df = pd.DataFrame(
     ...     [
     ...         [1, 2, 1, "2021-09-01"],  # 0
```

### Comparing `rectools-0.5.0/rectools/model_selection/splitter.py` & `rectools-0.6.0/rectools/model_selection/splitter.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/model_selection/time_split.py` & `rectools-0.6.0/rectools/model_selection/time_split.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,19 +52,21 @@
         The last fold includes the whole time unit with the last interaction.
         E.g. if the last interaction was at 01:25 a.m. of Monday, then
         with `test_size = "1D"` the last fold will be the full Monday,
         and with `test_size = "1H"` the last fold will be between 01:00 a.m. and 02:00 a.m on Monday.
     n_splits : int
         Number of test folds.
     filter_cold_users : bool, default ``True``
-        If `True`, users that not in train will be excluded from test.
+        If `True`, users that are not present in train will be excluded from test.
+        WARNING: both cold and warm users will be excluded from test.
     filter_cold_items : bool, default ``True``
-        If `True`, items that not in train will be excluded from test.
+        If `True`, items that are not present in train will be excluded from test.
+        WARNING: both cold and warm items will be excluded from test.
     filter_already_seen : bool, default ``True``
-        If ``True``, pairs (user, item) that are in train will be excluded from test.
+        If ``True``, pairs (user, item) that are present in train will be excluded from test.
 
     Examples
     --------
     >>> from datetime import date
     >>> df = pd.DataFrame(
     ...     [
     ...         [1, 2, 1, "2021-09-01"],  # 0
```

### Comparing `rectools-0.5.0/rectools/model_selection/utils.py` & `rectools-0.6.0/rectools/model_selection/utils.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/models/__init__.py` & `rectools-0.6.0/rectools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/models/dssm.py` & `rectools-0.6.0/rectools/models/dssm.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,19 +29,28 @@
 with warnings.catch_warnings():
     warnings.simplefilter("ignore", DeprecationWarning)
     from pytorch_lightning import Callback, LightningModule, Trainer
     from pytorch_lightning.loggers import Logger
 
 from torch import nn
 from torch.utils.data import DataLoader
-from torch.utils.data import Dataset as TorchDataset
 
-from ..dataset.dataset import Dataset
-from ..dataset.torch_datasets import ItemFeaturesDataset, UserFeaturesDataset
-from ..exceptions import NotFittedError
+from rectools.dataset import Dataset
+from rectools.dataset.torch_datasets import (
+    DSSMItemDataset,
+    DSSMItemDatasetBase,
+    DSSMTrainDataset,
+    DSSMTrainDatasetBase,
+    DSSMUserDataset,
+    DSSMUserDatasetBase,
+)
+from rectools.exceptions import NotFittedError
+from rectools.types import InternalIdsArray
+
+from .base import InternalRecoTriplet
 from .rank import Distance
 from .vector import Factors, VectorModel
 
 
 class ItemNet(nn.Module):
     def __init__(
         self,
@@ -208,20 +217,32 @@
 
 class DSSMModel(VectorModel):
     """
     Wrapper for `rectools.models.dssm.DSSM`
 
     Parameters
     ----------
-    dataset_type : torch.utils.data.Dataset
+    train_dataset_type : Type(DSSMTrainDatasetBase), default `DSSMTrainDataset`
+        Type of dataset used for training.
+        A child of `torch.utils.data.Dataset` that implements `from_dataset` classmethod.
+        Used to construct `torch.utils.data.Dataset` from a given `rectools.dataset.dataset.Dataset`.
+    user_dataset_type : Type(DSSMUserDatasetBase), default `DSSMUserDataset`
+        Type of dataset used for user inference.
+        A child of `torch.utils.data.Dataset` that implements `from_dataset` classmethod.
+        Used to construct `torch.utils.data.Dataset` from a given `rectools.dataset.dataset.Dataset`.
+    item_dataset_type : Type(DSSMItemDatasetBase), default `DSSMItemDataset`
+        Type of dataset used for item inference.
         A child of `torch.utils.data.Dataset` that implements `from_dataset` classmethod.
         Used to construct `torch.utils.data.Dataset` from a given `rectools.dataset.dataset.Dataset`.
     model : Optional(DSSM), default None
         Which model to wrap.
         If model is None, an instance of default DSSM is created during fit.
+    n_factors: int, default 128
+        How many hidden units to use in user and item networks.
+        Used only if `model` is None.
     max_epochs : int, default 5
         Stop training if this number of epochs is reached.
         Keep in mind that if any kind of early stopping callback is passed
         as one of the callbacks along with a validation dataset,
         then hitting exactly max_epochs is not guaranteed.
     batch_size : int, default 128
         How many samples per batch to load.
@@ -239,104 +260,140 @@
         The "auto" option recognizes the machine you are on, and selects the respective.
     callbacks : Optional(Sequence(Callback)), default None
         Which callbacks to use. For instance, `pytorch_lightning.callbacks.TQDMProgressBar`, etc.
     loggers : LightningLoggerBase | iterable(LightningLoggerBase) | bool, default True
         Which loggers to use. For instance, `pytorch_lightning.loggers.TensorboardLogger`, etc.
     verbose : int, default 0
         Verbosity level (applies only to recommend loop).
+    deterministic : bool, default ``False``
+        If ``True``, sets whether PyTorch operations must use deterministic algorithms.
+        Use `pytorch_lightning.seed_everything` together with this param to fix the random state.
     """
 
+    recommends_for_warm = True
+    recommends_for_cold = False
+
     u2i_dist = Distance.EUCLIDEAN
     i2i_dist = Distance.EUCLIDEAN
 
     def __init__(
         self,
-        dataset_type: TorchDataset[tp.Any],
+        train_dataset_type: tp.Type[DSSMTrainDatasetBase] = DSSMTrainDataset,
+        user_dataset_type: tp.Type[DSSMUserDatasetBase] = DSSMUserDataset,
+        item_dataset_type: tp.Type[DSSMItemDatasetBase] = DSSMItemDataset,
         model: tp.Optional[DSSM] = None,
+        n_factors: int = 128,
         max_epochs: int = 5,
         batch_size: int = 128,
         dataloader_num_workers: int = 0,
         trainer_sanity_steps: int = 2,
         trainer_devices: tp.Union[str, int] = 1,
         trainer_accelerator: str = "auto",
         callbacks: tp.Optional[tp.Union[tp.List[Callback], Callback]] = None,
         loggers: tp.Union[Logger, tp.Iterable[Logger], bool] = True,
         verbose: int = 0,
+        deterministic: bool = False,
     ) -> None:
         super().__init__(verbose=verbose)
-        self.model: tp.Optional[DSSM]
+        self.model: DSSM
         self._model = model
+        self.n_factors = n_factors
         self.max_epochs = max_epochs
         self.batch_size = batch_size
         self.trainer: Trainer
         self._trainer = Trainer(
             devices=trainer_devices,
             accelerator=trainer_accelerator,
             max_epochs=self.max_epochs,
             num_sanity_val_steps=trainer_sanity_steps,
             callbacks=callbacks,
             logger=loggers,
+            deterministic=deterministic,
         )
         self.dataloader_num_workers = dataloader_num_workers
-        self.dataset_type = dataset_type
+        self.train_dataset_type = train_dataset_type
+        self.user_dataset_type = user_dataset_type
+        self.item_dataset_type = item_dataset_type
 
     def _fit(self, dataset: Dataset, dataset_valid: tp.Optional[Dataset] = None) -> None:  # type: ignore
         self.trainer = deepcopy(self._trainer)
-        self.model = deepcopy(self._model)
 
-        if self.model is None:
+        if self._model is None:
+            if dataset.user_features is None or dataset.item_features is None:
+                raise ValueError("DSSM model requires user and item features to be present in the dataset.")
             self.model = DSSM(
-                n_factors_user=128,
-                n_factors_item=128,
-                dim_input_user=dataset.user_features.get_sparse().shape[1],  # type: ignore
-                dim_input_item=dataset.item_features.get_sparse().shape[1],  # type: ignore
+                n_factors_user=self.n_factors,
+                n_factors_item=self.n_factors,
+                dim_input_user=dataset.user_features.get_sparse().shape[1],
+                dim_input_item=dataset.item_features.get_sparse().shape[1],
                 dim_interactions=dataset.get_user_item_matrix().shape[1],
             )
-        train_dataset = self.dataset_type.from_dataset(dataset)  # type: ignore
+        else:
+            self.model = deepcopy(self._model)
+
+        train_dataset = self.train_dataset_type.from_dataset(dataset)
         train_dataloader = DataLoader(
             train_dataset,
             batch_size=self.batch_size,
             num_workers=self.dataloader_num_workers,
             shuffle=True,
         )
+        valid_dataloader = None
         if dataset_valid is not None:
-            valid_dataset = self.dataset_type.from_dataset(dataset_valid)  # type: ignore
+            valid_dataset = self.train_dataset_type.from_dataset(dataset_valid)
             valid_dataloader = DataLoader(
                 valid_dataset,
                 batch_size=self.batch_size,
                 num_workers=self.dataloader_num_workers,
                 shuffle=False,
             )
-            self.trainer.fit(
-                model=self.model,
-                train_dataloaders=train_dataloader,
-                val_dataloaders=valid_dataloader,
-            )
-        else:
-            self.trainer.fit(model=self.model, train_dataloaders=train_dataloader)
+
+        self.trainer.fit(
+            model=self.model,
+            train_dataloaders=train_dataloader,
+            val_dataloaders=valid_dataloader,
+        )
 
     def get_vectors(self, dataset: Dataset) -> tp.Tuple[np.ndarray, np.ndarray]:
         if not self.is_fitted:
             raise NotFittedError(self.__class__.__name__)
         user_factors = self._get_users_factors(dataset)
         item_factors = self._get_items_factors(dataset)
         return user_factors.embeddings, item_factors.embeddings
 
     def _get_users_factors(self, dataset: Dataset) -> Factors:
         dataloader = DataLoader(
-            UserFeaturesDataset.from_dataset(dataset),
+            self.user_dataset_type.from_dataset(dataset),
             batch_size=self.batch_size,
             num_workers=self.dataloader_num_workers,
             shuffle=False,
         )
-        vectors = self.model.inference_users(dataloader)  # type: ignore
+        vectors = self.model.inference_users(dataloader)
         return Factors(vectors)
 
     def _get_items_factors(self, dataset: Dataset) -> Factors:
         dataloader = DataLoader(
-            ItemFeaturesDataset.from_dataset(dataset),
+            self.item_dataset_type.from_dataset(dataset),
             batch_size=self.batch_size,
             num_workers=self.dataloader_num_workers,
             shuffle=False,
         )
-        vectors = self.model.inference_items(dataloader)  # type: ignore
+        vectors = self.model.inference_items(dataloader)
         return Factors(vectors)
+
+    def _recommend_u2i_warm(
+        self,
+        user_ids: InternalIdsArray,
+        dataset: Dataset,
+        k: int,
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
+    ) -> InternalRecoTriplet:
+        return self._recommend_u2i(user_ids, dataset, k, False, sorted_item_ids_to_recommend)
+
+    def _recommend_i2i_warm(
+        self,
+        target_ids: InternalIdsArray,
+        dataset: Dataset,
+        k: int,
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
+    ) -> InternalRecoTriplet:
+        return self._recommend_i2i(target_ids, dataset, k, sorted_item_ids_to_recommend)
```

### Comparing `rectools-0.5.0/rectools/models/ease.py` & `rectools-0.6.0/rectools/models/ease.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import typing as tp
 
 import numpy as np
 from scipy import sparse
 
 from rectools import InternalIds
 from rectools.dataset import Dataset
+from rectools.types import InternalIdsArray
 
 from .base import ModelBase, Scores
 from .rank import Distance, ImplicitRanker
 
 
 class EASEModel(ModelBase):
     """
@@ -43,15 +44,16 @@
         The regularization factor of the weights.
     verbose : int, default 0
         Degree of verbose output. If 0, no output will be provided.
     num_threads: int, default 1
         Number of threads used for `recommend` method.
     """
 
-    u2i_dist = Distance.DOT
+    recommends_for_warm = False
+    recommends_for_cold = False
 
     def __init__(
         self,
         regularization: float = 500.0,
         num_threads: int = 1,
         verbose: int = 0,
     ):
@@ -70,24 +72,24 @@
         gram_matrix_inv = np.linalg.inv(gram_matrix)
 
         self.weight = np.array(gram_matrix_inv / (-np.diag(gram_matrix_inv)))
         np.fill_diagonal(self.weight, 0.0)
 
     def _recommend_u2i(
         self,
-        user_ids: np.ndarray,
+        user_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
         filter_viewed: bool,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
         user_items = dataset.get_user_item_matrix(include_weights=True)
 
         ranker = ImplicitRanker(
-            distance=self.u2i_dist,
+            distance=Distance.DOT,
             subjects_factors=user_items,
             objects_factors=self.weight,
         )
         ui_csr_for_filter = user_items[user_ids] if filter_viewed else None
 
         all_user_ids, all_reco_ids, all_scores = ranker.rank(
             subject_ids=user_ids,
@@ -97,18 +99,18 @@
             num_threads=self.num_threads,
         )
 
         return all_user_ids, all_reco_ids, all_scores
 
     def _recommend_i2i(
         self,
-        target_ids: np.ndarray,
+        target_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
         similarity = self.weight[target_ids]
         if sorted_item_ids_to_recommend is not None:
             similarity = similarity[:, sorted_item_ids_to_recommend]
 
         n_reco = min(k, similarity.shape[1])
         unsorted_reco_positions = similarity.argpartition(-n_reco, axis=1)[:, -n_reco:]
```

### Comparing `rectools-0.5.0/rectools/models/implicit_als.py` & `rectools-0.6.0/rectools/models/implicit_als.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         Degree of verbose output. If 0, no output will be provided.
     fit_features_together: bool, default False
         Whether fit explicit features together with latent features or not.
         Used only if explicit features are present in dataset.
         See documentations linked above for details.
     """
 
+    recommends_for_warm = False
+    recommends_for_cold = False
+
     u2i_dist = Distance.DOT
     i2i_dist = Distance.COSINE
 
     def __init__(self, model: AnyAlternatingLeastSquares, verbose: int = 0, fit_features_together: bool = False):
         super().__init__(verbose=verbose)
 
         self.model: AnyAlternatingLeastSquares
@@ -70,24 +73,24 @@
         self.model = deepcopy(self._model)
         ui_csr = dataset.get_user_item_matrix(include_weights=True).astype(np.float32)
 
         if self.fit_features_together:
             fit_als_with_features_together_inplace(
                 self.model,
                 ui_csr,
-                dataset.user_features,
-                dataset.item_features,
+                dataset.get_hot_user_features(),
+                dataset.get_hot_item_features(),
                 self.verbose,
             )
         else:
             fit_als_with_features_separately_inplace(
                 self.model,
                 ui_csr,
-                dataset.user_features,
-                dataset.item_features,
+                dataset.get_hot_user_features(),
+                dataset.get_hot_item_features(),
                 self.verbose,
             )
 
     def _get_users_factors(self, dataset: Dataset) -> Factors:
         return Factors(get_users_vectors(self.model))
 
     def _get_items_factors(self, dataset: Dataset) -> Factors:
```

### Comparing `rectools-0.5.0/rectools/models/implicit_knn.py` & `rectools-0.6.0/rectools/models/implicit_knn.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from implicit.nearest_neighbours import ItemItemRecommender
 from implicit.utils import ParameterWarning
 from scipy import sparse
 from tqdm.auto import tqdm
 
 from rectools import InternalIds
 from rectools.dataset import Dataset
+from rectools.types import InternalId, InternalIdsArray
 from rectools.utils import fast_isin_for_sorted_test_elements
 
 from .base import ModelBase, Scores
 from .utils import get_viewed_item_ids, recommend_from_scores
 
 
 class ImplicitItemKNNWrapperModel(ModelBase):
@@ -40,14 +41,17 @@
     ----------
     model : ItemItemRecommender
         Base model that will be used.
     verbose : int, default 0
         Degree of verbose output. If 0, no output will be provided.
     """
 
+    recommends_for_warm = False
+    recommends_for_cold = False
+
     def __init__(self, model: ItemItemRecommender, verbose: int = 0):
         super().__init__(verbose=verbose)
         self.model: ItemItemRecommender
         self._model = model
 
     def _fit(self, dataset: Dataset) -> None:  # type: ignore
         self.model = deepcopy(self._model)
@@ -55,19 +59,19 @@
         # implicit library processes weights in coo_matrix format and then warns about converting it to csr
         with warnings.catch_warnings():
             warnings.filterwarnings(action="ignore", category=ParameterWarning, message="Method expects CSR input")
             self.model.fit(ui_csr, show_progress=self.verbose > 0)
 
     def _recommend_u2i(
         self,
-        user_ids: np.ndarray,
+        user_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
         filter_viewed: bool,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
         user_items = dataset.get_user_item_matrix(include_weights=True)
 
         all_user_ids = []
         all_reco_ids: tp.List[int] = []
         all_scores: tp.List[float] = []
         for user_id in tqdm(user_ids, disable=self.verbose == 0):
@@ -82,19 +86,19 @@
             all_reco_ids.extend(reco_ids)
             all_scores.extend(reco_scores)
 
         return all_user_ids, all_reco_ids, all_scores
 
     def _recommend_for_user(
         self,
-        user_id: int,
+        user_id: InternalId,
         user_items: sparse.csr_matrix,
         k: int,
         filter_viewed: bool,
-        sorted_item_ids: tp.Optional[np.ndarray],
+        sorted_item_ids: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, Scores]:
         if filter_viewed:
             viewed_ids = get_viewed_item_ids(user_items, user_id)  # sorted
         else:
             viewed_ids = np.array([], dtype=int)
 
         # Set filter_already_liked_items=False because if there are not enough reco it uses already liked
@@ -116,18 +120,18 @@
 
         reco = reco[valid_items_mask][:k]
         scores = scores[valid_items_mask][:k]
         return reco, scores
 
     def _recommend_i2i(
         self,
-        target_ids: np.ndarray,
+        target_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
         similarity = self.model.similarity
         if sorted_item_ids_to_recommend is not None:
             similarity = similarity[:, sorted_item_ids_to_recommend]
 
         all_target_ids = []
         all_reco_ids: tp.List[np.ndarray] = []
@@ -148,15 +152,15 @@
             all_reco_ids_arr = sorted_item_ids_to_recommend[all_reco_ids_arr]
 
         return all_target_ids, all_reco_ids_arr, np.concatenate(all_scores)
 
     @staticmethod
     def _recommend_for_item(
         similarity: sparse.csr_matrix,
-        target_id: int,
+        target_id: InternalId,
         k: int,
     ) -> tp.Tuple[np.ndarray, np.ndarray]:
         slice_ = slice(similarity.indptr[target_id], similarity.indptr[target_id + 1])
         similar_item_ids = similarity.indices[slice_]
         similar_item_scores = similarity.data[slice_]
         reco_similar_ids, reco_scores = recommend_from_scores(similar_item_scores, k=k)
         reco_ids = similar_item_ids[reco_similar_ids]
```

### Comparing `rectools-0.5.0/rectools/models/popular.py` & `rectools-0.6.0/rectools/models/popular.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,30 +20,31 @@
 
 import numpy as np
 import pandas as pd
 from tqdm.auto import tqdm
 
 from rectools import Columns, InternalIds
 from rectools.dataset import Dataset
+from rectools.types import InternalIdsArray
 from rectools.utils import fast_isin_for_sorted_test_elements
 
-from .base import ModelBase, Scores
+from .base import FixedColdRecoModelMixin, ModelBase, Scores, ScoresArray
 from .utils import get_viewed_item_ids
 
 
 class Popularity(Enum):
     """Types of popularity"""
 
     N_USERS = "n_users"
     N_INTERACTIONS = "n_interactions"
     MEAN_WEIGHT = "mean_weight"
     SUM_WEIGHT = "sum_weight"
 
 
-class PopularModel(ModelBase):
+class PopularModel(FixedColdRecoModelMixin, ModelBase):
     """
     Model generating recommendations based on popularity of items.
 
     Parameters
     ----------
     popularity : {"n_users", "n_interactions", "mean_weight", "sum_weight"}, default `"n_users"`
         Method of calculating item popularity.
@@ -68,14 +69,17 @@
         Cold items score will be equal to ``0``.
     inverse : bool, default ``False``
         If ``True`` least popular items will be selected.
     verbose : int, default ``0``
         Degree of verbose output. If ``0``, no output will be provided.
     """
 
+    recommends_for_warm = False
+    recommends_for_cold = True
+
     def __init__(
         self,
         popularity: str = "n_users",
         period: tp.Optional[timedelta] = None,
         begin_from: tp.Optional[datetime] = None,
         add_cold: bool = False,
         inverse: bool = False,
@@ -93,15 +97,15 @@
             raise ValueError("Only one of `period` and `begin_from` can be set")
         self.period = period
         self.begin_from = begin_from
 
         self.add_cold = add_cold
         self.inverse = inverse
 
-        self.popularity_list: tp.Tuple[np.ndarray, np.ndarray]
+        self.popularity_list: tp.Tuple[InternalIdsArray, ScoresArray]
 
     def _filter_interactions(self, interactions: pd.DataFrame) -> pd.DataFrame:
         if self.begin_from is not None:
             interactions = interactions.loc[interactions[Columns.Datetime] >= self.begin_from]
         elif self.period is not None:
             begin_from = interactions[Columns.Datetime].max() - self.period
             interactions = interactions.loc[interactions[Columns.Datetime] >= begin_from]
@@ -136,25 +140,21 @@
             return Columns.Weight, "mean"
         if popularity == Popularity.SUM_WEIGHT:
             return Columns.Weight, "sum"
         raise ValueError(f"Unexpected popularity {popularity}")
 
     def _recommend_u2i(
         self,
-        user_ids: np.ndarray,
+        user_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
         filter_viewed: bool,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
-        if sorted_item_ids_to_recommend is not None:
-            valid_items_mask = fast_isin_for_sorted_test_elements(self.popularity_list[0], sorted_item_ids_to_recommend)
-            popularity_list = (self.popularity_list[0][valid_items_mask], self.popularity_list[1][valid_items_mask])
-        else:
-            popularity_list = self.popularity_list
+        popularity_list = self._get_filtered_popularity_list(sorted_item_ids_to_recommend)
 
         if filter_viewed:
             user_items = dataset.get_user_item_matrix(include_weights=False)
 
         all_user_ids = []
         all_reco_ids: tp.List[int] = []
         all_scores: tp.List[float] = []
@@ -170,16 +170,16 @@
 
         return all_user_ids, all_reco_ids, all_scores
 
     @classmethod
     def _recommend_for_user(
         cls,
         k: int,
-        popularity_list: tp.Tuple[np.ndarray, np.ndarray],
-        sorted_blacklist: tp.Optional[np.ndarray],
+        popularity_list: tp.Tuple[InternalIdsArray, ScoresArray],
+        sorted_blacklist: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, Scores]:
         if sorted_blacklist is not None:
             n_items = k + sorted_blacklist.size
         else:
             n_items = k
 
         reco = popularity_list[0][:n_items]
@@ -190,18 +190,18 @@
             reco = reco[valid_mask][:k]
             scores = scores[valid_mask][:k]
 
         return reco, scores
 
     def _recommend_i2i(
         self,
-        target_ids: np.ndarray,
+        target_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
         _, single_reco, single_scores = self._recommend_u2i(
             user_ids=dataset.user_id_map.internal_ids[:1],
             dataset=dataset,
             k=k,
             filter_viewed=False,
             sorted_item_ids_to_recommend=sorted_item_ids_to_recommend,
@@ -210,7 +210,24 @@
         n_targets = len(target_ids)
         n_reco_per_target = len(single_reco)
 
         all_target_ids = np.repeat(target_ids, n_reco_per_target)
         all_reco_ids = np.tile(single_reco, n_targets)
         all_scores = np.tile(single_scores, n_targets)
         return all_target_ids, all_reco_ids, all_scores
+
+    def _get_filtered_popularity_list(
+        self, sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray]
+    ) -> tp.Tuple[InternalIdsArray, ScoresArray]:
+        popularity_list = self.popularity_list
+        if sorted_item_ids_to_recommend is not None:
+            valid_items_mask = fast_isin_for_sorted_test_elements(popularity_list[0], sorted_item_ids_to_recommend)
+            popularity_list = (popularity_list[0][valid_items_mask], popularity_list[1][valid_items_mask])
+        return popularity_list
+
+    def _get_cold_reco(
+        self, dataset: Dataset, k: int, sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray]
+    ) -> tp.Tuple[InternalIds, Scores]:
+        popularity_list = self._get_filtered_popularity_list(sorted_item_ids_to_recommend)
+        reco_ids = popularity_list[0][:k]
+        scores = popularity_list[1][:k]
+        return reco_ids, scores
```

### Comparing `rectools-0.5.0/rectools/models/popular_in_category.py` & `rectools-0.6.0/rectools/models/popular_in_category.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from enum import Enum
 
 import numpy as np
 import pandas as pd
 
 from rectools import Columns, InternalIds
 from rectools.dataset import Dataset, Interactions, features
+from rectools.types import InternalIdsArray
 
 from .base import Scores
 from .popular import PopularModel
 
 
 class MixingStrategy(Enum):
     """Types of mixing strategy"""
@@ -90,14 +91,17 @@
         Cold items score will be equal to ``0``.
     inverse : bool, default ``False``
         If ``True`` least popular items will be selected.
     verbose : int, default ``0``
         Degree of verbose output. If ``0``, no output will be provided.
     """
 
+    recommends_for_warm = False
+    recommends_for_cold = True
+
     def __init__(
         self,
         category_feature: str,
         n_categories: tp.Optional[int] = None,
         mixing_strategy: tp.Optional[str] = "rotate",
         ratio_strategy: tp.Optional[str] = "proportional",
         popularity: str = "n_users",
@@ -226,15 +230,15 @@
         return num_recs
 
     def _get_full_recs_from_main_and_fallback(
         self,
         main_recs: tp.List[pd.DataFrame],
         fallback_recs: tp.List[pd.DataFrame],
         k: int,
-        user_ids: np.ndarray,
+        user_ids: InternalIdsArray,
     ) -> pd.DataFrame:
         cat_recs = pd.concat(main_recs, sort=False)
         cat_recs.drop_duplicates(subset=[Columns.User, Columns.Item], inplace=True)
 
         num_recs_per_user = cat_recs[Columns.User].value_counts()
         user_w_insufficient_recs = num_recs_per_user[num_recs_per_user < k].index
 
@@ -267,19 +271,19 @@
         )
         insufficient_recs = insufficient_recs.groupby(Columns.User).head(k)
         full_recs = pd.concat([sufficient_recs, insufficient_recs], sort=False)
         return full_recs
 
     def _recommend_u2i(
         self,
-        user_ids: np.ndarray,
+        user_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
         filter_viewed: bool,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
         num_recs = self._get_num_recs_for_each_category(k)
         main_recs = []
         fallback_recs = []
         for priority, num_col in enumerate(num_recs.index):
             model = self.models[num_col]
             all_user_ids, all_reco_ids, all_scores = model._recommend_u2i(  # pylint: disable=protected-access
@@ -309,27 +313,71 @@
         elif self.mixing_strategy == MixingStrategy.ROTATE:
             full_recs["category_rank"] = full_recs.groupby([Columns.User, "category_priority"], sort=False).cumcount()
             full_recs.sort_values(by=[Columns.User, "category_rank", "category_priority"], inplace=True)
         return full_recs[Columns.User].values, full_recs[Columns.Item].values, full_recs[Columns.Score].values
 
     def _recommend_i2i(
         self,
-        target_ids: np.ndarray,
+        target_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
-        _, single_reco, single_scores = self._recommend_u2i(
-            user_ids=dataset.user_id_map.internal_ids[:1],
-            dataset=dataset,
-            k=k,
-            filter_viewed=False,
-            sorted_item_ids_to_recommend=sorted_item_ids_to_recommend,
-        )
-
+        single_reco, single_scores = self._get_cold_reco(dataset, k, sorted_item_ids_to_recommend)
         n_targets = len(target_ids)
         n_reco_per_target = len(single_reco)
 
         all_target_ids = np.repeat(target_ids, n_reco_per_target)
         all_reco_ids = np.tile(single_reco, n_targets)
         all_scores = np.tile(single_scores, n_targets)
         return all_target_ids, all_reco_ids, all_scores
+
+    def _get_cold_reco(
+        self, dataset: Dataset, k: int, sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray]
+    ) -> tp.Tuple[InternalIds, Scores]:
+        num_recs = self._get_num_recs_for_each_category(k)
+        main_recs = []
+        fallback_recs = []
+        for priority, num_col in enumerate(num_recs.index):
+            model = self.models[num_col]
+            reco_ids, reco_scores = model._get_cold_reco(  # pylint: disable=protected-access
+                dataset, k, sorted_item_ids_to_recommend
+            )
+            reco_df = pd.DataFrame(
+                {
+                    Columns.Item: reco_ids,
+                    Columns.Score: reco_scores,
+                    "category_priority": priority,
+                }
+            )
+            reco_df["category_rank"] = range(len(reco_df))
+            main_mask = reco_df["category_rank"] < num_recs.loc[num_col]
+            main_recs.append(reco_df[main_mask])
+            fallback_recs.append(reco_df[~main_mask])
+        cat_recs = pd.concat(main_recs, sort=False)
+        cat_recs.drop_duplicates(subset=[Columns.Item], inplace=True)
+        if len(cat_recs) < k:
+            cat_recs["is_main_rec"] = True
+            extra_recs = pd.concat(fallback_recs, sort=False)
+            extra_recs["is_main_rec"] = False
+            full_recs = pd.concat([cat_recs, extra_recs], sort=False)
+            full_recs.drop_duplicates(subset=[Columns.Item], inplace=True)
+
+            # Extra recommendations are given in a specific logic to guarantee that fallback recommendations
+            # never replace main recommendations in final result. And popular category doesn't dominate
+            # over other categories in fallback recs. Thus `rotate` mixing strategy is applied before getting
+            # k recs for each user.
+            full_recs.sort_values(
+                by=["is_main_rec", "category_rank", "category_priority"],
+                ascending=[False, True, True],
+                inplace=True,
+            )
+            full_recs = full_recs.head(k)
+        else:
+            full_recs = cat_recs
+
+        if self.mixing_strategy == MixingStrategy.GROUP:
+            full_recs.sort_values(by=["category_priority", "category_rank"], inplace=True)
+        elif self.mixing_strategy == MixingStrategy.ROTATE:
+            full_recs["category_rank"] = full_recs.groupby(["category_priority"], sort=False).cumcount()
+            full_recs.sort_values(by=["category_rank", "category_priority"], inplace=True)
+        return full_recs[Columns.Item].values, full_recs[Columns.Score].values
```

### Comparing `rectools-0.5.0/rectools/models/pure_svd.py` & `rectools-0.6.0/rectools/models/pure_svd.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     ----------
     factors : int, default ``10``
         The number of latent factors to compute.
     verbose : int, default ``0``
         Degree of verbose output. If ``0``, no output will be provided.
     """
 
+    recommends_for_warm = False
+    recommends_for_cold = False
+
     u2i_dist = Distance.DOT
     i2i_dist = Distance.COSINE
 
     def __init__(self, factors: int = 10, verbose: int = 0):
         super().__init__(verbose=verbose)
 
         self.factors = factors
```

### Comparing `rectools-0.5.0/rectools/models/random.py` & `rectools-0.6.0/rectools/models/random.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,24 +18,40 @@
 import typing as tp
 
 import numpy as np
 from tqdm.auto import tqdm
 
 from rectools import InternalIds
 from rectools.dataset import Dataset
+from rectools.types import AnyIdsArray, InternalId, InternalIdsArray
 from rectools.utils import fast_isin_for_sorted_test_elements
 
-from .base import ModelBase, Scores
+from .base import ModelBase, Scores, SemiInternalRecoTriplet
 from .utils import get_viewed_item_ids
 
-# Experiments have shown that for random sampling without replacement if k / n > 0.025
-# where n - size of population, k - required number of samples
-# it's faster to use `np.random.choice(population, k, replace=False)
-# otherwise it's better to use `random.sample(population, k)
-K_TO_N_MIN_NUMPY_RATIO = 0.025
+
+class _RandomGen:
+    def __init__(self, random_state: tp.Optional[int] = None) -> None:
+        self.python_gen = random.Random(random_state)  # nosec
+        self.np_gen = np.random.default_rng(random_state)
+
+
+class _RandomSampler:
+    def __init__(self, values: np.ndarray, random_gen: _RandomGen) -> None:
+        self.python_gen = random_gen.python_gen
+        self.np_gen = random_gen.np_gen
+        self.values = values
+        self.values_list = list(values)  # for random.sample
+
+    def sample(self, n: int) -> np.ndarray:
+        if n < 25:  # Empiric value, for optimization
+            sampled = np.asarray(self.python_gen.sample(self.values_list, n))
+        else:
+            sampled = self.np_gen.choice(self.values, n, replace=False)
+        return sampled
 
 
 class RandomModel(ModelBase):
     """
     Model generating random recommendations.
 
     By default all items that are present
@@ -47,73 +63,87 @@
     ----------
     random_state : int, optional, default ``None``
         Pseudorandom number generator state to control the sampling.
     verbose : int, default ``0``
         Degree of verbose output. If ``0``, no output will be provided.
     """
 
+    recommends_for_warm = False
+    recommends_for_cold = True
+
     def __init__(self, random_state: tp.Optional[int] = None, verbose: int = 0):
         super().__init__(verbose=verbose)
         self.random_state = random_state
+        self.random_gen = _RandomGen(random_state)
+
         self.all_item_ids: np.ndarray
 
     def _fit(self, dataset: Dataset) -> None:  # type: ignore
         self.all_item_ids = dataset.item_id_map.internal_ids
 
     def _recommend_u2i(
         self,
-        user_ids: np.ndarray,
+        user_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
         filter_viewed: bool,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
         if filter_viewed:
             user_items = dataset.get_user_item_matrix(include_weights=False)
 
-        if sorted_item_ids_to_recommend is not None:
-            item_ids = np.unique(sorted_item_ids_to_recommend)
-        else:
-            item_ids = self.all_item_ids
-
-        item_indices = list(range(item_ids.size))  # for random.sample
-
-        np.random.seed(self.random_state)
-        random.seed(self.random_state, version=2)
+        item_ids = sorted_item_ids_to_recommend if sorted_item_ids_to_recommend is not None else self.all_item_ids
+        sampler = _RandomSampler(item_ids, self.random_gen)
 
         all_user_ids = []
-        all_reco_ids = []
+        all_reco_ids: tp.List[InternalId] = []
         all_scores: tp.List[float] = []
         for user_id in tqdm(user_ids, disable=self.verbose == 0):
             if filter_viewed:
                 viewed_ids = get_viewed_item_ids(user_items, user_id)  # sorted
                 n_reco = k + viewed_ids.size
             else:
                 n_reco = k
 
             n_reco = min(n_reco, item_ids.size)
-
-            if n_reco / item_ids.size < K_TO_N_MIN_NUMPY_RATIO:
-                reco_indices = random.sample(item_indices, n_reco)
-                reco_ids = item_ids[reco_indices]
-            else:
-                reco_ids = np.random.choice(item_ids, n_reco, replace=False)
+            reco_ids = sampler.sample(n_reco)
 
             if filter_viewed:
                 reco_ids = reco_ids[fast_isin_for_sorted_test_elements(reco_ids, viewed_ids, invert=True)][:k]
 
             reco_scores = np.arange(reco_ids.size, 0, -1)
 
             all_user_ids.extend([user_id] * len(reco_ids))
-            all_reco_ids.extend(reco_ids)
-            all_scores.extend(reco_scores)
+            all_reco_ids.extend(reco_ids.tolist())
+            all_scores.extend(reco_scores.tolist())
 
         return all_user_ids, all_reco_ids, all_scores
 
     def _recommend_i2i(
         self,
-        target_ids: np.ndarray,
+        target_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
         return self._recommend_u2i(target_ids, dataset, k, False, sorted_item_ids_to_recommend)
+
+    def _recommend_cold(
+        self,
+        target_ids: AnyIdsArray,
+        dataset: Dataset,
+        k: int,
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
+    ) -> SemiInternalRecoTriplet:
+        item_ids = sorted_item_ids_to_recommend if sorted_item_ids_to_recommend is not None else self.all_item_ids
+        sampler = _RandomSampler(item_ids, self.random_gen)
+        n_reco = min(k, item_ids.size)
+
+        reco_ids_lst = []
+        for _ in tqdm(target_ids, disable=self.verbose == 0):
+            reco_ids = sampler.sample(n_reco)
+            reco_ids_lst.append(reco_ids)
+
+        reco_item_ids = np.concatenate(reco_ids_lst)
+        reco_target_ids = np.repeat(target_ids, n_reco)
+        reco_scores = np.tile(np.arange(n_reco, 0, -1), len(target_ids))
+        return reco_target_ids, reco_item_ids, reco_scores
```

### Comparing `rectools-0.5.0/rectools/models/rank.py` & `rectools-0.6.0/rectools/models/rank.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import implicit.cpu
 import numpy as np
 from implicit.cpu.matrix_factorization_base import _filter_items_from_sparse_matrix as filter_items_from_sparse_matrix
 from scipy import sparse
 
 from rectools import InternalIds
 from rectools.models.base import Scores
+from rectools.types import InternalIdsArray
 
 
 class Distance(Enum):
     """Distance metric"""
 
     DOT = 1  # Bigger value means closer vectors
     COSINE = 2  # Bigger value means closer vectors
@@ -57,28 +58,28 @@
     def __init__(
         self, distance: Distance, subjects_factors: tp.Union[np.ndarray, sparse.csr_matrix], objects_factors: np.ndarray
     ) -> None:
         if isinstance(subjects_factors, sparse.csr_matrix) and distance != Distance.DOT:
             raise ValueError("To use `sparse.csr_matrix` distance must be `Distance.DOT`")
 
         self.distance = distance
-        self.subjects_factors = subjects_factors.astype(np.float32)
-        self.objects_factors = objects_factors.astype(np.float32)
+        self.subjects_factors: np.ndarray = subjects_factors.astype(np.float32)
+        self.objects_factors: np.ndarray = objects_factors.astype(np.float32)
 
         self.subjects_norms: np.ndarray
         if distance == Distance.COSINE:
             self.subjects_norms = self._calc_norms(self.subjects_factors, avoid_zeros=True)
 
         self.subjects_dots: np.ndarray
         if distance == Distance.EUCLIDEAN:
             self.subjects_dots = self._calc_dots(self.subjects_factors)
 
     def _get_neginf_score(self) -> float:
         # Adding 1 to avoid float calculation errors (we're comparing `scores <= neginf_score`)
-        return -np.finfo(np.float32).max + 1
+        return float(-np.finfo(np.float32).max + 1)
 
     @staticmethod
     def _calc_dots(factors: np.ndarray) -> np.ndarray:
         return (factors**2).sum(axis=1)
 
     @staticmethod
     def _calc_norms(factors: np.ndarray, avoid_zeros: bool = False) -> np.ndarray:
@@ -132,15 +133,15 @@
         return all_target_ids, np.concatenate(all_reco_ids), np.concatenate(all_scores)
 
     def rank(
         self,
         subject_ids: InternalIds,
         k: int,
         filter_pairs_csr: tp.Optional[sparse.csr_matrix] = None,
-        sorted_object_whitelist: tp.Optional[np.ndarray] = None,
+        sorted_object_whitelist: tp.Optional[InternalIdsArray] = None,
         num_threads: int = 0,
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
         """Rank objects to proceed inference using implicit library topk cpu method.
 
         Parameters
         ----------
         subject_ids : csr_matrix
```

### Comparing `rectools-0.5.0/rectools/models/utils.py` & `rectools-0.6.0/rectools/models/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 """Useful functions."""
 
 import typing as tp
 
 import numpy as np
 from scipy import sparse
 
+from rectools.models.base import ScoresArray
+from rectools.types import InternalId, InternalIdsArray
 from rectools.utils import fast_isin_for_sorted_test_elements
 
 
-def get_viewed_item_ids(user_items: sparse.csr_matrix, user_id: int) -> np.ndarray:
+def get_viewed_item_ids(user_items: sparse.csr_matrix, user_id: InternalId) -> InternalIdsArray:
     """
     Return indices of items that user has interacted with.
 
     Parameters
     ----------
     user_items : csr_matrix
         Matrix of interactions.
@@ -38,20 +40,20 @@
     np.ndarray
         Internal item indices that user has interacted with.
     """
     return user_items.indices[user_items.indptr[user_id] : user_items.indptr[user_id + 1]]
 
 
 def recommend_from_scores(
-    scores: np.ndarray,
+    scores: ScoresArray,
     k: int,
-    sorted_blacklist: tp.Optional[np.ndarray] = None,
-    sorted_whitelist: tp.Optional[np.ndarray] = None,
+    sorted_blacklist: tp.Optional[InternalIdsArray] = None,
+    sorted_whitelist: tp.Optional[InternalIdsArray] = None,
     ascending: bool = False,
-) -> tp.Tuple[np.ndarray, np.ndarray]:
+) -> tp.Tuple[InternalIdsArray, ScoresArray]:
     """
     Prepare top-k recommendations for a user.
 
     Recommendations are sorted by item scores for this particular user.
     Recommendations can be filtered according to whitelist and blacklist.
 
     If `I` - set of all items, `B` - set of blacklist items, `W` - set of whitelist items, then:
```

### Comparing `rectools-0.5.0/rectools/models/vector.py` & `rectools-0.6.0/rectools/models/vector.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import attr
 import numpy as np
 
 from rectools import InternalIds
 from rectools.dataset import Dataset
 from rectools.models.base import ModelBase, Scores
+from rectools.types import InternalIdsArray
 
 from .rank import Distance, ImplicitRanker
 
 
 @attr.s(auto_attribs=True)
 class Factors:
     """Embeddings and biases"""
@@ -39,43 +40,44 @@
 
     u2i_dist: Distance = NotImplemented
     i2i_dist: Distance = NotImplemented
     n_threads: int = 0  # TODO: decide how to pass it correctly for all models
 
     def _recommend_u2i(
         self,
-        user_ids: np.ndarray,
+        user_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
         filter_viewed: bool,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
         if filter_viewed:
             user_items = dataset.get_user_item_matrix(include_weights=False)
+            ui_csr_for_filter = user_items[user_ids]
         else:
-            user_items = None
+            ui_csr_for_filter = None
 
         user_vectors, item_vectors = self._get_u2i_vectors(dataset)
 
         ranker = ImplicitRanker(self.u2i_dist, user_vectors, item_vectors)
-        ui_csr_for_filter = user_items[user_ids] if filter_viewed else None
+
         return ranker.rank(
             subject_ids=user_ids,
             k=k,
             filter_pairs_csr=ui_csr_for_filter,
             sorted_object_whitelist=sorted_item_ids_to_recommend,
             num_threads=self.n_threads,
         )
 
     def _recommend_i2i(
         self,
-        target_ids: np.ndarray,
+        target_ids: InternalIdsArray,
         dataset: Dataset,
         k: int,
-        sorted_item_ids_to_recommend: tp.Optional[np.ndarray],
+        sorted_item_ids_to_recommend: tp.Optional[InternalIdsArray],
     ) -> tp.Tuple[InternalIds, InternalIds, Scores]:
         item_vectors_1, item_vectors_2 = self._get_i2i_vectors(dataset)
 
         ranker = ImplicitRanker(self.i2i_dist, item_vectors_1, item_vectors_2)
 
         return ranker.rank(
             subject_ids=target_ids,
```

### Comparing `rectools-0.5.0/rectools/tools/__init__.py` & `rectools-0.6.0/rectools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/tools/ann.py` & `rectools-0.6.0/rectools/tools/ann.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     index_query_time_params: optional(dict(str, str)), default None
         NMSLIB query time parameters. See nmslib documentation.
         In case of None defaults to reasonable parameters.
     create_index_params: optional(dict(str, str)), default None
         NMSLIB index creation parameters. See nmslib documentation.
         In case of None defaults to reasonable parameters.
     index : FloatIndex, optional
-        Optonal instance of FloatIndex. Exists for outside initialization.
+        Optional instance of FloatIndex. Exists for outside initialization.
 
     See Also
     --------
     UserToItemAnnRecommender
     ItemToItemAnnRecommender
     """
 
@@ -229,15 +229,15 @@
     index_query_time_params: optional(dict(str, int)), default None
         NMSLIB query time parameters. See nmslib documentation.
         In case of None defaults to reasonable parameters.
     create_index_params: optional(dict(str, int)), default None
         NMSLIB index creation parameters. See nmslib documentation.
         In case of None defaults to reasonable parameters.
     index : FloatIndex, optional
-        Optonal instance of `FloatIndex`. Exists for outside initialization.
+        Optional instance of `FloatIndex`. Exists for outside initialization.
 
     Methods
     -------
     get_item_list_for_user
         Part of public API. Given user id and item ids, calculates
         recommendations via index query.
     get_item_list_for_user_batch
@@ -379,15 +379,15 @@
     index_query_time_params : optional(dict(str, int)) | rectools.dataset.IdMap
         NMSLIB query time parameters. See nmslib documentation.
         In case of None defaults to reasonable parameters.
     create_index_params : optional(dict(str, int)) | rectools.dataset.IdMap
         NMSLIB index creation parameters. See nmslib documentation.
         In case of None defaults to reasonable parameters.
     index : FloatIndex, optional
-        Optonal instance of FloatIndex. Exists for outside initialization.
+        Optional instance of FloatIndex. Exists for outside initialization.
 
     Methods
     -------
     get_item_list_for_item
         Part of public API. Given item id and available item ids, calculates
         recommendations via index query.
     get_item_list_for_item_batch
```

### Comparing `rectools-0.5.0/rectools/types.py` & `rectools-0.6.0/rectools/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,12 +13,15 @@
 #  limitations under the License.
 
 import typing as tp
 
 import numpy as np
 
 ExternalId = tp.Hashable
-ExternalIds = tp.Union[tp.Sequence[ExternalId], np.ndarray]
+ExternalIdsArray = np.ndarray
+ExternalIds = tp.Union[tp.Sequence[ExternalId], ExternalIdsArray]
 InternalId = int
-InternalIds = tp.Union[tp.Sequence[InternalId], np.ndarray]
+InternalIdsArray = np.ndarray
+InternalIds = tp.Union[tp.Sequence[InternalId], InternalIdsArray]
+AnyIdsArray = tp.Union[ExternalIdsArray, InternalIdsArray]
 AnyIds = tp.Union[ExternalIds, InternalIds]
 AnySequence = tp.Union[tp.Sequence[tp.Any], np.ndarray]
```

### Comparing `rectools-0.5.0/rectools/utils/__init__.py` & `rectools-0.6.0/rectools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/utils/array_set_ops.py` & `rectools-0.6.0/rectools/utils/array_set_ops.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/utils/misc.py` & `rectools-0.6.0/rectools/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import typing as tp
 from itertools import tee
 
 import numpy as np
-from typeguard import check_type
+from typeguard import TypeCheckError, check_type
 
 T = tp.TypeVar("T")
 
 
 def pairwise(iterable: tp.Iterable[T]) -> tp.Iterable[tp.Tuple[T, T]]:
     """
     Make iterator of pairs of neighbours in sequence.
@@ -89,17 +89,17 @@
 
     Returns
     -------
     bool
         Whether `type_` is type of `obj`.
     """
     try:
-        check_type("", obj, type_)
+        check_type(obj, type_)
         return True
-    except TypeError:
+    except TypeCheckError:
         return False
 
 
 def is_instance(obj: tp.Any, types: tp.Union[AnyType, tp.Tuple[AnyType, ...]]) -> bool:
     """
     Analogue of `isinstance(obj, types)` but also works for generics.
```

### Comparing `rectools-0.5.0/rectools/visuals/__init__.py` & `rectools-0.6.0/rectools/visuals/__init__.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/rectools/visuals/visual_app.py` & `rectools-0.6.0/rectools/visuals/visual_app.py`

 * *Files identical despite different names*

### Comparing `rectools-0.5.0/PKG-INFO` & `rectools-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 Metadata-Version: 2.1
 Name: rectools
-Version: 0.5.0
+Version: 0.6.0
 Summary: An easy-to-use Python library for building recommendation systems
 Home-page: https://github.com/MobileTeleSystems/RecTools
 License: Apache-2.0
 Keywords: recsys,recommendation systems,machine learning,AI,personalization
 Author: Emiliy Feldman
 Author-email: feldlime@yandex.ru
 Maintainer: Emiliy Feldman
 Maintainer-email: feldlime@yandex.ru
-Requires-Python: >=3.7.2,<3.11
+Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: lightfm
 Provides-Extra: nmslib
 Provides-Extra: torch
 Provides-Extra: visuals
 Requires-Dist: attrs (>=19.1.0,<24.0.0)
 Requires-Dist: implicit (>=0.7.1,<0.8.0)
 Requires-Dist: ipywidgets (>=7.7,<8.2) ; extra == "visuals" or extra == "all"
-Requires-Dist: lightfm (>=1.16,<=1.17) ; extra == "lightfm" or extra == "all"
-Requires-Dist: nmslib (>=2.0.4,<3.0.0) ; extra == "nmslib" or extra == "all"
-Requires-Dist: numpy (>=1.19.5,<2.0.0)
-Requires-Dist: pandas (>=0.25.3,<2.0.0) ; python_version < "3.8"
-Requires-Dist: pandas (>=1.0.0,<3.0.0) ; python_version >= "3.8"
-Requires-Dist: pytorch-lightning (>=1.6.0,<2.0.0) ; (python_version < "3.8") and (extra == "torch" or extra == "all")
-Requires-Dist: pytorch-lightning (>=1.6.0,<3.0.0) ; (python_version >= "3.8") and (extra == "torch" or extra == "all")
-Requires-Dist: scipy (>=1.5.4,<2.0.0)
-Requires-Dist: torch (>=1.6.0,<2.0.0) ; (python_version < "3.8") and (extra == "torch" or extra == "all")
-Requires-Dist: torch (>=1.6.0,<3.0.0) ; (python_version >= "3.8") and (extra == "torch" or extra == "all")
+Requires-Dist: lightfm (>=1.16,<=1.17) ; (python_version < "3.12") and (extra == "lightfm" or extra == "all")
+Requires-Dist: nmslib (>=2.0.4,<3.0.0) ; (python_version < "3.11") and (extra == "nmslib" or extra == "all")
+Requires-Dist: numpy (>=1.19.5,<2.0.0) ; python_version == "3.8"
+Requires-Dist: numpy (>=1.22,<2.0.0) ; python_version >= "3.9" and python_version < "3.12"
+Requires-Dist: numpy (>=1.26,<2.0.0) ; python_version >= "3.12"
+Requires-Dist: pandas (>=1.5.0,<3.0.0)
+Requires-Dist: pytorch-lightning (>=1.6.0,<3.0.0) ; extra == "torch" or extra == "all"
+Requires-Dist: scipy (>=1.10.1,<1.13) ; python_version >= "3.9"
+Requires-Dist: scipy (>=1.9.1,<1.11) ; python_version == "3.8"
+Requires-Dist: torch (>=1.6.0,<3.0.0) ; extra == "torch" or extra == "all"
 Requires-Dist: tqdm (>=4.27.0,<5.0.0)
-Requires-Dist: typeguard (>=2.0.1,<3.0.0)
+Requires-Dist: typeguard (>=4.1.0,<5.0.0)
 Project-URL: Documentation, https://rectools.readthedocs.io
 Project-URL: Repository, https://github.com/MobileTeleSystems/RecTools
 Description-Content-Type: text/markdown
 
 # RecTools
 
 [![Python versions](https://img.shields.io/pypi/pyversions/rectools.svg)](https://pypi.org/project/rectools)
@@ -164,15 +165,15 @@
 
 - All of the models follow the same interface. **No exceptions**
 - No need for manual creation of sparse matrixes or mapping ids. Preparing data for models is as simple as `dataset = Dataset.construct(interactions_df)`
 - Fitting any model is as simple as `model.fit(dataset)`
 - For getting recommendations `filter_viewed` and `items_to_recommend` options are available
 - For item-to-item recommendations use `recommend_to_items` method
 - For feeding user/item features to model just specify dataframes when constructing `Dataset`. [Check our tutorial](examples/4_dataset_with_features.ipynb)
-
+- For warm / cold inference just provide all required ids in `users` or `target_items` parameters of `recommend` or `recommend_to_items` methods and make sure you have features in the dataset for warm users/items. **Nothing else is needed, everything works out of the box.** Check [documentation](https://rectools.readthedocs.io/en/stable/features.html#models) to see which models support this scenarios.
 
 ## Contribution
 [Contributing guide](CONTRIBUTING.rst)
 
 To install all requirements
 - you must have `python3` and `poetry==1.4.0` installed
 - make sure you have no active virtual environments (deactivate conda `base` if applicable)
```

