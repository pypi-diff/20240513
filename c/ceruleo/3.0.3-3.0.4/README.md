# Comparing `tmp/ceruleo-3.0.3.tar.gz` & `tmp/ceruleo-3.0.4.tar.gz`

## Comparing `ceruleo-3.0.3.tar` & `ceruleo-3.0.4.tar`

### file list

```diff
@@ -1,189 +1,190 @@
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ceruleo-3.0.3/.bumpversion.cfg
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ceruleo-3.0.3/.coveragerc
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 ceruleo-3.0.3/.zenodo.json
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 ceruleo-3.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ceruleo-3.0.3/RELEASING.md
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 ceruleo-3.0.3/mkdocs.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ceruleo-3.0.3/requirements.txt
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 ceruleo-3.0.3/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ceruleo-3.0.3/.github/workflows/joss.yml
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 ceruleo-3.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 ceruleo-3.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/transformed.py
--rw-r--r--   0        0        0    13758 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/ts_dataset.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/utils.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/analysis/__init__.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/analysis/correlation.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/analysis/distribution.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/analysis/numerical_features.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/analysis/sample_rate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/builder/__init__.py
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/builder/builder.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/builder/cycles_splitter.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/builder/output.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/builder/rul_column.py
--rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/catalog/CMAPSS.py
--rw-r--r--   0        0        0     5846 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/catalog/CMAPSS2.py
--rw-r--r--   0        0        0     7059 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/catalog/PHMDataset2018.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/dataset/catalog/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/graphics/__init__.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/graphics/analysis.py
--rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/graphics/duration.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/graphics/explanations.py
--rw-r--r--   0        0        0    21499 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/graphics/results.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/graphics/utils/__init__.py
--rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/graphics/utils/curly_brace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/iterators/__init__.py
--rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/iterators/batcher.py
--rw-r--r--   0        0        0    12800 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/iterators/iterators.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/iterators/sample_weight.py
--rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/iterators/shufflers.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/iterators/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/__init__.py
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/baseline.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/pytorch.py
--rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/sklearn.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/inspection/feature_importance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/callbacks.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/dataset.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/layers.py
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/losses.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/weibull.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/catalog/CNLSTM.py
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/catalog/InceptionTime.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/catalog/MSWRLRCN.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/catalog/MVCNN.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/catalog/MultiScaleConvolutional.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/catalog/MultiTaskRUL.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/catalog/XCM.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/catalog/XiangQiangJianQiao.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/keras/catalog/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/torch/__init__.py
--rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/torch/dsanet.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/models/torch/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/results/__init__.py
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/results/picewise_regression.py
--rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/results/results.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/target.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/__init__.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/cast.py
--rw-r--r--   0        0        0     7655 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/denoising.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/entropy.py
--rw-r--r--   0        0        0    36221 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/extraction.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/extraction_frequency.py
--rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/hurst.py
--rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/imputers.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/operations.py
--rw-r--r--   0        0        0    14712 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/outliers.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/resamplers.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/rolling_windows.py
--rw-r--r--   0        0        0    14446 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/scalers.py
--rw-r--r--   0        0        0    12171 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/selection.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/slicing.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/split.py
--rw-r--r--   0        0        0    10869 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/tdigest.py
--rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/features/transformation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/__init__.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/common.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/concatenate.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/graph_utils.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/mixin.py
--rw-r--r--   0        0        0     8446 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/transformers.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/transformerstep.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/pipeline/__init__.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/pipeline/cache_store.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/pipeline/pipeline.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/pipeline/runner.py
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/pipeline/traversal.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/transformation/functional/pipeline/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/utils/__init__.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/utils/download.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ceruleo-3.0.3/ceruleo/utils/lrucache.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/index.md
--rw-r--r--   0        0        0    13289 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/refs.bib
--rw-r--r--   0        0        0   289838 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/dataset/Example.ipynb
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/dataset/builder.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/dataset/catalog.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/dataset/dataset.md
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/dataset/visualization.md
--rw-r--r--   0        0        0   527614 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/dataset/analysis/Sensor Validation.ipynb
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/dataset/analysis/correlation.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/dataset/analysis/distribution.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/dataset/analysis/sample_rate.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/dataset/analysis/sensor_validation.md
--rw-r--r--   0        0        0    17517 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/images/cerulean.png
--rw-r--r--   0        0        0    67664 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/images/unipd_logo.png
--rw-r--r--   0        0        0    50083 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/img/duration_histogram.png
--rw-r--r--   0        0        0     7770 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/iterators/Iterators.ipynb
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/iterators/batcher.md
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/iterators/iterators.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/iterators/shufflers.md
--rw-r--r--   0        0        0   631762 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/models/Models.ipynb
--rw-r--r--   0        0        0   486920 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/models/Models_sklearn.ipynb
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/models/baseline.md
--rw-r--r--   0        0        0   139463 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/models/models_tf.ipynb
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/models/sklearn.md
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/models/keras/index.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/models/keras/catalog/models.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/results/results.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/results/visualization.md
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/pipeline.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/transformers.md
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/cast.md
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/denoising.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/entropy.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/extraction.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/extraction_frequency.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/hurst.md
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/imputers.md
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/operations.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/outliers.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/resamplers.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/rolling_windows.md
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/scalers.md
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/selection.md
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/slicing.md
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/split.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ceruleo-3.0.3/docs/transformation/features/transformation.md
--rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 ceruleo-3.0.3/paper/paper.bib
--rw-r--r--   0        0        0     7364 2020-02-02 00:00:00.000000 ceruleo-3.0.3/paper/paper.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/manual_features.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_analysis.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_batcher.py
--rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_dataset.py
--rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_dataset_builder.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_denoising.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_graph.py
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_graphics.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_imputers.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_iterators.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_lrucache.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_models.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_operations.py
--rw-r--r--   0        0        0     9491 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_pipeline.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_results.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_scalers.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_shufflers.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_transformation.py
--rw-r--r--   0        0        0    25329 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_transformers.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_utils.py
--rw-r--r--   0        0        0    48809 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_images/test_XCM_explanation-expected.png
--rw-r--r--   0        0        0    14744 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_images/test_barplot_errors_wrt_RUL-expected.png
--rw-r--r--   0        0        0    22355 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_images/test_boxplot_errors_wrt_RUL-expected.png
--rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_images/test_correlation_plot-expected.png
--rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_images/test_durations_boxplot-expected.png
--rw-r--r--   0        0        0    23670 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_images/test_durations_histogram-expected.png
--rw-r--r--   0        0        0    26658 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_images/test_plot_predictions_grid_1-expected.png
--rw-r--r--   0        0        0    38027 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_images/test_plot_predictions_grid_2-expected.png
--rw-r--r--   0        0        0    53987 2020-02-02 00:00:00.000000 ceruleo-3.0.3/tests/test_images/test_shadedline_plot_errors_wrt_RUL-expected.png
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 ceruleo-3.0.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ceruleo-3.0.3/LICENSE
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 ceruleo-3.0.3/README.md
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 ceruleo-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 ceruleo-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ceruleo-3.0.4/.bumpversion.cfg
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ceruleo-3.0.4/.coveragerc
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 ceruleo-3.0.4/.zenodo.json
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 ceruleo-3.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ceruleo-3.0.4/RELEASING.md
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 ceruleo-3.0.4/mkdocs.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ceruleo-3.0.4/requirements.txt
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 ceruleo-3.0.4/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ceruleo-3.0.4/.github/workflows/joss.yml
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 ceruleo-3.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 ceruleo-3.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/transformed.py
+-rw-r--r--   0        0        0    13758 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/ts_dataset.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/utils.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/analysis/__init__.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/analysis/correlation.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/analysis/distribution.py
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/analysis/numerical_features.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/analysis/sample_rate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/builder/__init__.py
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/builder/builder.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/builder/cycles_splitter.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/builder/output.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/builder/rul_column.py
+-rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/catalog/CMAPSS.py
+-rw-r--r--   0        0        0     5846 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/catalog/CMAPSS2.py
+-rw-r--r--   0        0        0     7059 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/catalog/PHMDataset2018.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/dataset/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/graphics/__init__.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/graphics/analysis.py
+-rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/graphics/duration.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/graphics/explanations.py
+-rw-r--r--   0        0        0    21499 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/graphics/results.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/graphics/utils/__init__.py
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/graphics/utils/curly_brace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/iterators/__init__.py
+-rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/iterators/batcher.py
+-rw-r--r--   0        0        0    12800 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/iterators/iterators.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/iterators/sample_weight.py
+-rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/iterators/shufflers.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/iterators/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/__init__.py
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/baseline.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/pytorch.py
+-rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/sklearn.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/inspection/feature_importance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/callbacks.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/dataset.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/layers.py
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/losses.py
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/weibull.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/catalog/CNLSTM.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/catalog/InceptionTime.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/catalog/MSWRLRCN.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/catalog/MVCNN.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/catalog/MultiScaleConvolutional.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/catalog/MultiTaskRUL.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/catalog/XCM.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/catalog/XiangQiangJianQiao.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/keras/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/torch/__init__.py
+-rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/torch/dsanet.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/models/torch/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/results/__init__.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/results/picewise_regression.py
+-rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/results/results.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/target.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/__init__.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/cast.py
+-rw-r--r--   0        0        0     7655 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/denoising.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/entropy.py
+-rw-r--r--   0        0        0    36221 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/extraction.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/extraction_frequency.py
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/hurst.py
+-rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/imputers.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/operations.py
+-rw-r--r--   0        0        0    14712 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/outliers.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/resamplers.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/rolling_windows.py
+-rw-r--r--   0        0        0    14446 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/scalers.py
+-rw-r--r--   0        0        0    12171 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/selection.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/slicing.py
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/split.py
+-rw-r--r--   0        0        0    10869 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/tdigest.py
+-rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/features/transformation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/__init__.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/common.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/concatenate.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/graph_utils.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/mixin.py
+-rw-r--r--   0        0        0     8446 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/transformers.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/transformerstep.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/pipeline/__init__.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/pipeline/cache_store.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/pipeline/pipeline.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/pipeline/runner.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/pipeline/traversal.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/transformation/functional/pipeline/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/utils/__init__.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/utils/download.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ceruleo-3.0.4/ceruleo/utils/lrucache.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/index.md
+-rw-r--r--   0        0        0    13289 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/refs.bib
+-rw-r--r--   0        0        0   289838 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/dataset/Example.ipynb
+-rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/dataset/builder.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/dataset/catalog.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/dataset/dataset.md
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/dataset/visualization.md
+-rw-r--r--   0        0        0   527614 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/dataset/analysis/Sensor Validation.ipynb
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/dataset/analysis/correlation.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/dataset/analysis/distribution.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/dataset/analysis/sample_rate.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/dataset/analysis/sensor_validation.md
+-rw-r--r--   0        0        0    17517 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/images/cerulean.png
+-rw-r--r--   0        0        0    67664 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/images/unipd_logo.png
+-rw-r--r--   0        0        0    50083 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/img/duration_histogram.png
+-rw-r--r--   0        0        0     7770 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/iterators/Iterators.ipynb
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/iterators/batcher.md
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/iterators/iterators.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/iterators/shufflers.md
+-rw-r--r--   0        0        0   631762 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/models/Models.ipynb
+-rw-r--r--   0        0        0   486920 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/models/Models_sklearn.ipynb
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/models/baseline.md
+-rw-r--r--   0        0        0   139463 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/models/models_tf.ipynb
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/models/sklearn.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/models/keras/index.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/models/keras/catalog/models.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/results/results.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/results/visualization.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/pipeline.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/transformers.md
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/cast.md
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/denoising.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/entropy.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/extraction.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/extraction_frequency.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/hurst.md
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/imputers.md
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/operations.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/outliers.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/resamplers.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/rolling_windows.md
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/scalers.md
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/selection.md
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/slicing.md
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/split.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ceruleo-3.0.4/docs/transformation/features/transformation.md
+-rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 ceruleo-3.0.4/paper/paper.bib
+-rw-r--r--   0        0        0     7364 2020-02-02 00:00:00.000000 ceruleo-3.0.4/paper/paper.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/manual_features.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_analysis.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_batcher.py
+-rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_dataset.py
+-rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_dataset_builder.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_denoising.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_graph.py
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_graphics.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_imputers.py
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_iterators.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_lrucache.py
+-rw-r--r--   0        0        0    14411 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_models.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_operations.py
+-rw-r--r--   0        0        0     9491 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_pipeline.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_results.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_scalers.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_shufflers.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_sklearn.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_transformation.py
+-rw-r--r--   0        0        0    25329 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_transformers.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_utils.py
+-rw-r--r--   0        0        0    48809 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_images/test_XCM_explanation-expected.png
+-rw-r--r--   0        0        0    14744 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_images/test_barplot_errors_wrt_RUL-expected.png
+-rw-r--r--   0        0        0    22355 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_images/test_boxplot_errors_wrt_RUL-expected.png
+-rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_images/test_correlation_plot-expected.png
+-rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_images/test_durations_boxplot-expected.png
+-rw-r--r--   0        0        0    23670 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_images/test_durations_histogram-expected.png
+-rw-r--r--   0        0        0    26658 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_images/test_plot_predictions_grid_1-expected.png
+-rw-r--r--   0        0        0    38027 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_images/test_plot_predictions_grid_2-expected.png
+-rw-r--r--   0        0        0    53987 2020-02-02 00:00:00.000000 ceruleo-3.0.4/tests/test_images/test_shadedline_plot_errors_wrt_RUL-expected.png
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 ceruleo-3.0.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ceruleo-3.0.4/LICENSE
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 ceruleo-3.0.4/README.md
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 ceruleo-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 ceruleo-3.0.4/PKG-INFO
```

### Comparing `ceruleo-3.0.3/.zenodo.json` & `ceruleo-3.0.4/.zenodo.json`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/CONTRIBUTING.md` & `ceruleo-3.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/mkdocs.yml` & `ceruleo-3.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/.github/workflows/documentation.yml` & `ceruleo-3.0.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/.github/workflows/joss.yml` & `ceruleo-3.0.4/.github/workflows/joss.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/.github/workflows/publish.yml` & `ceruleo-3.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/.github/workflows/test.yml` & `ceruleo-3.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/transformed.py` & `ceruleo-3.0.4/ceruleo/dataset/transformed.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/ts_dataset.py` & `ceruleo-3.0.4/ceruleo/dataset/ts_dataset.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/utils.py` & `ceruleo-3.0.4/ceruleo/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/analysis/correlation.py` & `ceruleo-3.0.4/ceruleo/dataset/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/analysis/distribution.py` & `ceruleo-3.0.4/ceruleo/dataset/analysis/distribution.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/analysis/numerical_features.py` & `ceruleo-3.0.4/ceruleo/dataset/analysis/numerical_features.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/analysis/sample_rate.py` & `ceruleo-3.0.4/ceruleo/dataset/analysis/sample_rate.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/builder/builder.py` & `ceruleo-3.0.4/ceruleo/dataset/builder/builder.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/builder/cycles_splitter.py` & `ceruleo-3.0.4/ceruleo/dataset/builder/cycles_splitter.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/builder/output.py` & `ceruleo-3.0.4/ceruleo/dataset/builder/output.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/builder/rul_column.py` & `ceruleo-3.0.4/ceruleo/dataset/builder/rul_column.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/catalog/CMAPSS.py` & `ceruleo-3.0.4/ceruleo/dataset/catalog/CMAPSS.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/catalog/CMAPSS2.py` & `ceruleo-3.0.4/ceruleo/dataset/catalog/CMAPSS2.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/dataset/catalog/PHMDataset2018.py` & `ceruleo-3.0.4/ceruleo/dataset/catalog/PHMDataset2018.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/graphics/analysis.py` & `ceruleo-3.0.4/ceruleo/graphics/analysis.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/graphics/duration.py` & `ceruleo-3.0.4/ceruleo/graphics/duration.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/graphics/explanations.py` & `ceruleo-3.0.4/ceruleo/graphics/explanations.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/graphics/results.py` & `ceruleo-3.0.4/ceruleo/graphics/results.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/graphics/utils/curly_brace.py` & `ceruleo-3.0.4/ceruleo/graphics/utils/curly_brace.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/iterators/batcher.py` & `ceruleo-3.0.4/ceruleo/iterators/batcher.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/iterators/iterators.py` & `ceruleo-3.0.4/ceruleo/iterators/iterators.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/iterators/sample_weight.py` & `ceruleo-3.0.4/ceruleo/iterators/sample_weight.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,47 @@
-from abc import abstractmethod
 
-from signal import signal
 from typing import Any, Callable, Union
 
 import numpy as np
+import pandas as pd
 
 
 class AbstractSampleWeights:
     """
     The base class for the sample weight provider
     """
 
-    def __call__(self, y, i: int, metadata):
+    def __call__(self, y: Union[np.ndarray, pd.DataFrame], i: int, metadata):
         raise NotImplementedError
 
 
+
+def get_value(y: Union[np.ndarray, pd.DataFrame], i:int) -> float:
+    if isinstance(y, np.ndarray):
+        if len(y.shape) > 1:
+            return y[i, 0]
+        else:
+            return  y[i]
+    elif isinstance(y, pd.DataFrame):
+        return y.iloc[i, 0] 
+    elif isinstance(y, pd.Series):
+        return y.iloc[i]
+    else:
+        raise ValueError(f"Unsupported type {type(y)}")
+   
+
+
 class NotWeighted(AbstractSampleWeights):
     """
     Simplest sample weight provider
 
     Provide 1 as a sample weight for every sample
     """
 
-    def __call__(self, y, i: int, metadata):
+    def __call__(self, y: Union[np.ndarray, pd.DataFrame], i: int, metadata):
         return 1
 
 
 """
 The Sample Weight type is a callable with the following signature
 
     fun(y, i:int, metadata)
@@ -37,35 +52,38 @@
 
 
 class RULInverseWeighted(AbstractSampleWeights):
     """
     Weight each sample by the inverse of the RUL
     """
 
-    def __call__(self, y, i: int, metadata):
-        return 1 / (y[i, 0] + 1)
+    def __call__(self, y : Union[np.ndarray, pd.DataFrame], i: int, metadata):
+        return 1 / (get_value(y, i) + 1)
+
+        
 
 
 class InverseToLengthWeighted(AbstractSampleWeights):
     """
     Weights samples according to the duration of the run-to-failure cycle they belong to.
 
     All points in the run-to-cycle are weighted equally inverse to the cycle duration
 
     """
 
-    def __call__(self, y, i: int, metadata):
-        return 1 / y[0]
+    def __call__(self, y:Union[np.ndarray, pd.DataFrame], i: int, metadata):
+        return 1 / get_value(y, 0)
 
 
 class ExponentialDecay(AbstractSampleWeights):
     """
     Weight samples with an exponential decay function based on the RUL.
 
     """
 
     def __init__(self, *, near_0_at: float):
+        
         super().__init__()
         self.alpha = -((near_0_at) ** 2) / np.log(0.000001)
 
-    def __call__(self, y, i: int, metadata):
-        return (1 + np.exp(-(y[i, 0] ** 2) / self.alpha)) ** 2
+    def __call__(self, y:Union[np.ndarray, pd.DataFrame], i: int, metadata):
+        return ( np.exp(-(get_value(y,i) ** 2) / self.alpha))
```

### Comparing `ceruleo-3.0.3/ceruleo/iterators/shufflers.py` & `ceruleo-3.0.4/ceruleo/iterators/shufflers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/iterators/utils.py` & `ceruleo-3.0.4/ceruleo/iterators/utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/baseline.py` & `ceruleo-3.0.4/ceruleo/models/baseline.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/pytorch.py` & `ceruleo-3.0.4/ceruleo/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/sklearn.py` & `ceruleo-3.0.4/ceruleo/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/inspection/feature_importance.py` & `ceruleo-3.0.4/ceruleo/models/inspection/feature_importance.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/callbacks.py` & `ceruleo-3.0.4/ceruleo/models/keras/callbacks.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/dataset.py` & `ceruleo-3.0.4/ceruleo/models/keras/dataset.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/layers.py` & `ceruleo-3.0.4/ceruleo/models/keras/layers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,46 @@
-import typing
-import warnings
-from typing import Tuple
+
 
 import numpy as np
 import tensorflow as tf
-from tensorflow.keras import Sequential
-from tensorflow.keras import backend as K
-from tensorflow.keras import regularizers
-from tensorflow.keras.layers import (Activation, BatchNormalization, Conv2D,
-                                     Dense, Flatten, Lambda, Layer, Permute,
-                                     Reshape)
+import keras
+from keras import Sequential
+from keras import backend as K
+from keras import regularizers
+from keras.layers import (
+    Activation,
+    BatchNormalization,
+    Conv2D,
+    GlobalAveragePooling1D,
+    Dense,
+    Flatten,
+    Lambda,
+    Layer,
+    Permute,
+    maximum,
+    Reshape,
+)
 from tensorflow.python.framework import tensor_shape
-from tensorflow.python.keras.layers.pooling import GlobalAveragePooling1D
+import keras
+if keras.__version__.startswith("3"):
+    import keras.ops as ops 
+else:
+    import tensorflow.keras.backend as ops
+
 
 
 def ExpandDimension(dim: int = -1):
-    return Lambda(lambda x: K.expand_dims(x, dim))
+    return Lambda(lambda x: ops.expand_dims(x, dim))
 
 
 def RemoveDimension(axis=0):
-    return Lambda(lambda x: K.squeeze(x, axis=axis))
+    return Lambda(lambda x: ops.squeeze(x, axis=axis))
 
 
-class ConcreteDropout(tf.keras.layers.Layer):
+class ConcreteDropout(Layer):
     """
     Concrete Dropout layer class from https://arxiv.org/abs/1705.07832.
     Dropout Feature Ranking for Deep Learning Models
     Chun-Hao Chang
     Ladislav Rampasek
     Anna Goldenberg
 
@@ -46,17 +60,16 @@
     def __init__(
         self,
         dropout_regularizer=1e-5,
         init_min=0.1,
         init_max=0.9,
         name=None,
         training=True,
-        **kwargs
+        **kwargs,
     ):
-
         super(ConcreteDropout, self).__init__(name=name, **kwargs)
         assert init_min <= init_max, "init_min must be lower or equal to init_max."
 
         self.dropout_regularizer = dropout_regularizer
 
         self.p_logit = None
         self.p = None
@@ -92,33 +105,33 @@
 
         retain_prob = 1.0 - p
         x *= random_tensor
         x /= retain_prob
         return x
 
     def call(self, inputs, training=True):
-
         p = K.sigmoid(self.p_logit)
 
         dropout_regularizer = p * K.log(p)
         dropout_regularizer += (1.0 - p) * K.log(1.0 - p)
         dropout_regularizer *= self.dropout_regularizer * self.number_of_features
         regularizer = K.sum(dropout_regularizer)
         self.add_loss(regularizer)
 
         x = self.concrete_dropout(p, inputs)
 
         return x
 
 
-class ResidualShrinkageBlock(tf.keras.layers.Layer):
+class ResidualShrinkageBlock(Layer):
     """
     ResidualShrinkageBlock
 
     """
+
     def build(self, input_shape):
         self.blocks = []
         for i in range(2):
             self.blocks.append(
                 Sequential(
                     [
                         BatchNormalization(),
@@ -167,67 +180,61 @@
         scales = self.shrinkage(abs_mean)
         thres = abs_mean * scales
         thres = Permute((2, 1, 3))(thres)
         sub = (residual_abs) - thres
 
         zeros = sub - sub
 
-        n_sub = tf.keras.layers.maximum([sub, zeros])
+        n_sub = maximum([sub, zeros])
 
-        residual = tf.keras.backend.sign(residual) * n_sub
+        residual = ops.sign(residual) * n_sub
         residual = RemoveDimension(3)(residual)
         return residual + inputs
 
 
-
-
 class ZeroWeights(tf.keras.constraints.Constraint):
-  
-
-  def __init__(self, l1:float):
-    self.l1 = l1
+    def __init__(self, l1: float):
+        self.l1 = l1
 
-  def __call__(self, w):
-    
-    return (tf.math.multiply(w, tf.cast(tf.abs(w) > self.l1, tf.float32)) )
+    def __call__(self, w):
+        return tf.math.multiply(w, tf.cast(tf.abs(w) > self.l1, tf.float32))
 
-  def get_config(self):
-    return {'l1': self.l1}
+    def get_config(self):
+        return {"l1": self.l1}
 
 
 class LASSOLayer(Layer):
-    """ 
+    """
     LASSO Layer
 
     Parameters:
         l1: L1 regularization parameter
     """
-    def __init__(self, l1:float):
+
+    def __init__(self, l1: float):
         super(LASSOLayer, self).__init__()
         self.l1 = l1
         self.kernel_regularizer = regularizers.L1(l1)
 
-
     def build(self, input_shape):
         W_size = np.prod(input_shape[1:])
         self.w = self.add_weight(
-            shape=(W_size, ),
+            shape=(W_size,),
             initializer="random_normal",
             trainable=True,
             regularizer=self.kernel_regularizer,
-            constraint=ZeroWeights(self.l1)
+            constraint=ZeroWeights(self.l1),
         )
-        
-        
+
         self.input_reshape = Reshape((W_size,))
         self.output_reshape = Reshape(input_shape[1:])
-        
-
 
     def call(self, inputs):
         x = self.input_reshape(inputs)
-        
-        
-        x = tf.math.multiply(self.w, x) 
-        
-        self.add_metric(tf.math.reduce_sum(tf.cast(tf.abs(self.w) > 0, tf.float32)), name="Number of features")
+
+        x = tf.math.multiply(self.w, x)
+
+        self.add_metric(
+            tf.math.reduce_sum(tf.cast(tf.abs(self.w) > 0, tf.float32)),
+            name="Number of features",
+        )
         return self.output_reshape(x)
```

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/losses.py` & `ceruleo-3.0.4/ceruleo/models/keras/losses.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/weibull.py` & `ceruleo-3.0.4/ceruleo/models/keras/weibull.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/catalog/CNLSTM.py` & `ceruleo-3.0.4/ceruleo/models/keras/catalog/CNLSTM.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/catalog/InceptionTime.py` & `ceruleo-3.0.4/ceruleo/models/keras/catalog/InceptionTime.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/catalog/MSWRLRCN.py` & `ceruleo-3.0.4/ceruleo/models/keras/catalog/MSWRLRCN.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Tuple
 import tensorflow as tf
-from tensorflow.python.keras.layers.pooling import GlobalAveragePooling1D, MaxPool1D
 from ceruleo.models.keras.layers import ExpandDimension, ResidualShrinkageBlock
-from tensorflow.keras import Input, Model, Sequential
-from tensorflow.keras.layers import (
+from keras import Input, Model, Sequential
+from keras.layers import (
 
     BatchNormalization,
 
     Dense,
 
     Conv1D,
     ReLU,
     LSTM,
     Bidirectional,
     Concatenate,
+    GlobalAveragePooling1D, 
+    MaxPooling1D
 
 )
 from typing import Tuple
 
 
 def MSWRLRCN(input_shape: Tuple[int, int]):
     """MSWR-LRCN: A new deep learning approach to remaining useful life estimation of bearings
@@ -28,15 +29,15 @@
 
     def ConvBlock(n_filters: int, kernel_size: int):
         return Sequential(
             [
                 Conv1D(n_filters, kernel_size, padding='same'),
                 BatchNormalization(),
                 ReLU(),
-                MaxPool1D(2),
+                MaxPooling1D(2),
             ]
         )
 
     input = Input(input_shape)
     x = input
     x1 = ConvBlock(input_shape[-1], 16)(x)
     x = ConvBlock(input_shape[-1], 32)(x1)
```

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/catalog/MVCNN.py` & `ceruleo-3.0.4/ceruleo/models/keras/catalog/MVCNN.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/catalog/MultiScaleConvolutional.py` & `ceruleo-3.0.4/ceruleo/models/keras/catalog/MultiScaleConvolutional.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/catalog/MultiTaskRUL.py` & `ceruleo-3.0.4/ceruleo/models/keras/catalog/MultiTaskRUL.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/catalog/XCM.py` & `ceruleo-3.0.4/ceruleo/models/keras/catalog/XCM.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple
 import numpy as np
 import tensorflow as tf
 
 from ceruleo.models.keras.layers import ExpandDimension, RemoveDimension
-from tensorflow.keras import Input, Model
-from tensorflow.keras.layers import (
+from keras import Input, Model
+from keras.layers import (
     Activation,
     BatchNormalization,
     Concatenate,
     Conv1D,
     Conv2D,
     Dense,
     GlobalAveragePooling1D,
@@ -92,15 +92,15 @@
     model_input = Input(shape=(input_shape[0], input_shape[1]))
     conv2d = model_fisrt_conv2d(model_input)
     conv1d = model_fisrt_conv1d(model_input)
     output = model_regression([conv2d, conv1d])
 
     model = Model(
         inputs=[model_input],
-        outputs=[output],
+        outputs=output,
     )
     return model,  (model_fisrt_conv1d, model_fisrt_conv2d, model_regression)
 
 
 def explain( model_extras, input):
     model_fisrt_conv1d, model_fisrt_conv2d, model_regression = model_extras
     data_input = np.expand_dims(input, axis=0)
```

### Comparing `ceruleo-3.0.3/ceruleo/models/keras/catalog/XiangQiangJianQiao.py` & `ceruleo-3.0.4/ceruleo/models/keras/catalog/XiangQiangJianQiao.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/torch/dsanet.py` & `ceruleo-3.0.4/ceruleo/models/torch/dsanet.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/models/torch/model.py` & `ceruleo-3.0.4/ceruleo/models/torch/model.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/results/picewise_regression.py` & `ceruleo-3.0.4/ceruleo/results/picewise_regression.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/results/results.py` & `ceruleo-3.0.4/ceruleo/results/results.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/target.py` & `ceruleo-3.0.4/ceruleo/transformation/target.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/utils.py` & `ceruleo-3.0.4/ceruleo/transformation/utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/cast.py` & `ceruleo-3.0.4/ceruleo/transformation/features/cast.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/denoising.py` & `ceruleo-3.0.4/ceruleo/transformation/features/denoising.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/entropy.py` & `ceruleo-3.0.4/ceruleo/transformation/features/entropy.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/extraction.py` & `ceruleo-3.0.4/ceruleo/transformation/features/extraction.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/extraction_frequency.py` & `ceruleo-3.0.4/ceruleo/transformation/features/extraction_frequency.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/hurst.py` & `ceruleo-3.0.4/ceruleo/transformation/features/hurst.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/imputers.py` & `ceruleo-3.0.4/ceruleo/transformation/features/imputers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/operations.py` & `ceruleo-3.0.4/ceruleo/transformation/features/operations.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/outliers.py` & `ceruleo-3.0.4/ceruleo/transformation/features/outliers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/resamplers.py` & `ceruleo-3.0.4/ceruleo/transformation/features/resamplers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/rolling_windows.py` & `ceruleo-3.0.4/ceruleo/transformation/features/rolling_windows.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/scalers.py` & `ceruleo-3.0.4/ceruleo/transformation/features/scalers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/selection.py` & `ceruleo-3.0.4/ceruleo/transformation/features/selection.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/slicing.py` & `ceruleo-3.0.4/ceruleo/transformation/features/slicing.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/split.py` & `ceruleo-3.0.4/ceruleo/transformation/features/split.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/tdigest.py` & `ceruleo-3.0.4/ceruleo/transformation/features/tdigest.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/features/transformation.py` & `ceruleo-3.0.4/ceruleo/transformation/features/transformation.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/functional/concatenate.py` & `ceruleo-3.0.4/ceruleo/transformation/functional/concatenate.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/functional/graph_utils.py` & `ceruleo-3.0.4/ceruleo/transformation/functional/graph_utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/functional/mixin.py` & `ceruleo-3.0.4/ceruleo/transformation/functional/mixin.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/functional/transformers.py` & `ceruleo-3.0.4/ceruleo/transformation/functional/transformers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/functional/transformerstep.py` & `ceruleo-3.0.4/ceruleo/transformation/functional/transformerstep.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/functional/pipeline/cache_store.py` & `ceruleo-3.0.4/ceruleo/transformation/functional/pipeline/cache_store.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/functional/pipeline/pipeline.py` & `ceruleo-3.0.4/ceruleo/transformation/functional/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/functional/pipeline/runner.py` & `ceruleo-3.0.4/ceruleo/transformation/functional/pipeline/runner.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/functional/pipeline/traversal.py` & `ceruleo-3.0.4/ceruleo/transformation/functional/pipeline/traversal.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/transformation/functional/pipeline/utils.py` & `ceruleo-3.0.4/ceruleo/transformation/functional/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/utils/download.py` & `ceruleo-3.0.4/ceruleo/utils/download.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/ceruleo/utils/lrucache.py` & `ceruleo-3.0.4/ceruleo/utils/lrucache.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/index.md` & `ceruleo-3.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/refs.bib` & `ceruleo-3.0.4/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/dataset/Example.ipynb` & `ceruleo-3.0.4/docs/dataset/Example.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/dataset/builder.md` & `ceruleo-3.0.4/docs/dataset/builder.md`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/dataset/catalog.md` & `ceruleo-3.0.4/docs/dataset/catalog.md`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/dataset/analysis/Sensor Validation.ipynb` & `ceruleo-3.0.4/docs/dataset/analysis/Sensor Validation.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.11.9'}}"}*

```diff
@@ -1127,13 +1127,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.7"
+            "version": "3.11.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `ceruleo-3.0.3/docs/dataset/analysis/sensor_validation.md` & `ceruleo-3.0.4/docs/dataset/analysis/sensor_validation.md`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/images/cerulean.png` & `ceruleo-3.0.4/docs/images/cerulean.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/images/unipd_logo.png` & `ceruleo-3.0.4/docs/images/unipd_logo.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/img/duration_histogram.png` & `ceruleo-3.0.4/docs/img/duration_histogram.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/iterators/Iterators.ipynb` & `ceruleo-3.0.4/docs/iterators/Iterators.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/iterators/iterators.md` & `ceruleo-3.0.4/docs/iterators/iterators.md`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/models/Models.ipynb` & `ceruleo-3.0.4/docs/models/Models.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/models/Models_sklearn.ipynb` & `ceruleo-3.0.4/docs/models/Models_sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/docs/models/models_tf.ipynb` & `ceruleo-3.0.4/docs/models/models_tf.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/paper/paper.bib` & `ceruleo-3.0.4/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/paper/paper.md` & `ceruleo-3.0.4/paper/paper.md`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/manual_features.py` & `ceruleo-3.0.4/tests/manual_features.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_analysis.py` & `ceruleo-3.0.4/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_batcher.py` & `ceruleo-3.0.4/tests/test_batcher.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_dataset.py` & `ceruleo-3.0.4/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_dataset_builder.py` & `ceruleo-3.0.4/tests/test_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_denoising.py` & `ceruleo-3.0.4/tests/test_denoising.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_graph.py` & `ceruleo-3.0.4/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_graphics.py` & `ceruleo-3.0.4/tests/test_graphics.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_imputers.py` & `ceruleo-3.0.4/tests/test_imputers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_lrucache.py` & `ceruleo-3.0.4/tests/test_lrucache.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_models.py` & `ceruleo-3.0.4/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
+from numpy.random import seed
+from sklearn.linear_model import LinearRegression
+from sklearn.pipeline import make_pipeline
+from tensorflow.keras import Input, Model
+from tensorflow.keras.layers import Dense, Flatten
+from xgboost import XGBRegressor
+
 from ceruleo.dataset.ts_dataset import AbstractPDMDataset
 from ceruleo.iterators.iterators import WindowedDatasetIterator
+from ceruleo.iterators.sample_weight import RULInverseWeighted
 from ceruleo.iterators.shufflers import AllShuffled
 from ceruleo.iterators.utils import true_values
 from ceruleo.models.baseline import BaselineModel, FixedValueBaselineModel
 from ceruleo.models.keras.callbacks import PredictionCallback
 from ceruleo.models.keras.catalog.CNLSTM import CNLSTM
 from ceruleo.models.keras.catalog.InceptionTime import InceptionTime
 from ceruleo.models.keras.catalog.MSWRLRCN import MSWRLRCN
-from ceruleo.models.keras.catalog.MVCNN import MVCNN
 from ceruleo.models.keras.catalog.MultiScaleConvolutional import (
     MultiScaleConvolutionalModel,
 )
 from ceruleo.models.keras.catalog.XCM import XCM, explain
 from ceruleo.models.keras.catalog.XiangQiangJianQiao import XiangQiangJianQiaoModel
 from ceruleo.models.keras.dataset import tf_regression_dataset
 from ceruleo.models.keras.losses import (
@@ -32,20 +39,14 @@
     TimeSeriesWindowTransformer,
     predict,
     train_model,
 )
 from ceruleo.transformation import Transformer
 from ceruleo.transformation.features.scalers import MinMaxScaler
 from ceruleo.transformation.features.selection import ByNameFeatureSelector
-from numpy.random import seed
-from sklearn.linear_model import LinearRegression
-from sklearn.pipeline import make_pipeline
-from tensorflow.keras import Input, Model
-from tensorflow.keras.layers import Dense, Flatten
-from xgboost import XGBRegressor
 
 seed(1)
 
 
 tf.random.set_seed(2)
 
 
@@ -207,14 +208,40 @@
         )
         y_pred = model.predict(tf_regression_dataset(val_iterator).batch(64))
 
         mae = np.mean(np.abs(y_pred.ravel() - y_true.ravel()))
 
         assert mae < mae_before_fit
 
+        train_iterator = WindowedDatasetIterator(
+            train_dataset.map(transformer),
+            window_size=window_size,
+            step=1,
+            shuffler=AllShuffled(),
+            sample_weight=RULInverseWeighted(),
+        )
+
+        val_iterator = WindowedDatasetIterator(
+            val_dataset.map(transformer), window_size=window_size, step=1
+        )
+        model.compile(loss="mae", optimizer=tf.keras.optimizers.SGD(0.01))
+        y_true = true_values(val_iterator)
+        y_pred_before_fit = model.predict(tf_regression_dataset(val_iterator).batch(64))
+        mae_before_fit = np.mean(np.abs(y_pred_before_fit.ravel() - y_true.ravel()))
+        model.fit(
+            tf_regression_dataset(train_iterator).batch(4),
+            validation_data=tf_regression_dataset(val_iterator).batch(64),
+            epochs=15,
+        )
+        y_pred = model.predict(tf_regression_dataset(val_iterator).batch(64))
+
+        mae = np.mean(np.abs(y_pred.ravel() - y_true.ravel()))
+
+        assert mae < mae_before_fit
+        
     def test_xgboost(self):
         features = ["feature1", "feature2"]
 
         x = ByNameFeatureSelector(features=features)
         x = MinMaxScaler(range=(-1, 1))(x)
 
         y = ByNameFeatureSelector(features=["RUL"])
```

### Comparing `ceruleo-3.0.3/tests/test_operations.py` & `ceruleo-3.0.4/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_pipeline.py` & `ceruleo-3.0.4/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_results.py` & `ceruleo-3.0.4/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_scalers.py` & `ceruleo-3.0.4/tests/test_scalers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_shufflers.py` & `ceruleo-3.0.4/tests/test_shufflers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_transformation.py` & `ceruleo-3.0.4/tests/test_transformation.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_transformers.py` & `ceruleo-3.0.4/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_utils.py` & `ceruleo-3.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_images/test_XCM_explanation-expected.png` & `ceruleo-3.0.4/tests/test_images/test_XCM_explanation-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_images/test_barplot_errors_wrt_RUL-expected.png` & `ceruleo-3.0.4/tests/test_images/test_barplot_errors_wrt_RUL-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_images/test_boxplot_errors_wrt_RUL-expected.png` & `ceruleo-3.0.4/tests/test_images/test_boxplot_errors_wrt_RUL-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_images/test_correlation_plot-expected.png` & `ceruleo-3.0.4/tests/test_images/test_correlation_plot-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_images/test_durations_boxplot-expected.png` & `ceruleo-3.0.4/tests/test_images/test_durations_boxplot-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_images/test_durations_histogram-expected.png` & `ceruleo-3.0.4/tests/test_images/test_durations_histogram-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_images/test_plot_predictions_grid_1-expected.png` & `ceruleo-3.0.4/tests/test_images/test_plot_predictions_grid_1-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_images/test_plot_predictions_grid_2-expected.png` & `ceruleo-3.0.4/tests/test_images/test_plot_predictions_grid_2-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/tests/test_images/test_shadedline_plot_errors_wrt_RUL-expected.png` & `ceruleo-3.0.4/tests/test_images/test_shadedline_plot_errors_wrt_RUL-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/.gitignore` & `ceruleo-3.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/LICENSE` & `ceruleo-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/README.md` & `ceruleo-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ceruleo-3.0.3/pyproject.toml` & `ceruleo-3.0.4/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,8 @@
     "notebook<=6.5",
     "jupyter_contrib_nbextensions",
     "mkdocstrings",
     "mkdocs-bibtex",
     "sphinxcontrib.bibtex",
     "mkdocs-matplotlib",
     
-]
+]
```

### Comparing `ceruleo-3.0.3/PKG-INFO` & `ceruleo-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ceruleo
-Version: 3.0.3
+Version: 3.0.4
 Summary: Remaining useful life estimation utilities
 Project-URL: Homepage, https://github.com/lucianolorenti/ceruleo
 Project-URL: Documentation, https://lucianolorenti.github.io/ceruleo/
 License: MIT
 License-File: LICENSE
 Keywords: predictive maintenance,remaining useful life
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ceruleo Version: 3.0.3 Summary: Remaining useful
+Metadata-Version: 2.3 Name: ceruleo Version: 3.0.4 Summary: Remaining useful
 life estimation utilities Project-URL: Homepage, https://github.com/
 lucianolorenti/ceruleo Project-URL: Documentation, https://
 lucianolorenti.github.io/ceruleo/ License: MIT License-File: LICENSE Keywords:
 predictive maintenance,remaining useful life Classifier: Programming Language
 :: Python :: 3 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.7 Requires-Dist: antropy>=0.1.5 Requires-
 Dist: emd>=0.4 Requires-Dist: gdown>=4.2 Requires-Dist: mmh3>=2.0 Requires-
```

