# Comparing `tmp/eo_grow-1.7.8.tar.gz` & `tmp/eo_grow-1.7.9.tar.gz`

## Comparing `eo_grow-1.7.8.tar` & `eo_grow-1.7.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/__init__.py
--rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/py.typed
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/types.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/__init__.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/base.py
--rw-r--r--   0        0        0     7266 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/config.py
--rw-r--r--   0        0        0    17547 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/logging.py
--rw-r--r--   0        0        0    12606 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/pipeline.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/schemas.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/storage.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/area/__init__.py
--rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/area/base.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/area/batch.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/area/custom_grid.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/core/area/utm.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/__init__.py
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/batch_to_eopatch.py
--rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/byoc.py
--rw-r--r--   0        0        0    13959 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/download.py
--rw-r--r--   0        0        0    12883 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/download_batch.py
--rw-r--r--   0        0        0    16559 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/export_maps.py
--rw-r--r--   0        0        0     9911 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/features.py
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/import_tiff.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/import_vector.py
--rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/merge_samples.py
--rw-r--r--   0        0        0     8620 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/prediction.py
--rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/rasterize.py
--rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/sampling.py
--rw-r--r--   0        0        0     9361 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/split_grid.py
--rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/testing.py
--rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/training.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/pipelines/zipmap.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/tasks/__init__.py
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/tasks/batch_to_eopatch.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/tasks/common.py
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/tasks/features.py
--rw-r--r--   0        0        0     7873 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/tasks/prediction.py
--rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/tasks/spatial.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/tasks/testing.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/__init__.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/batch.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/eopatch_list.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/filter.py
--rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/fs.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/general.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/grid.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/logging.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/map.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/meta.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/pipeline_chain.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/ray.py
--rw-r--r--   0        0        0    17120 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/testing.py
--rw-r--r--   0        0        0    10268 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/validators.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/vector.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 eo_grow-1.7.8/eogrow/utils/zipmap.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 eo_grow-1.7.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 eo_grow-1.7.8/LICENSE
--rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 eo_grow-1.7.8/README.md
--rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 eo_grow-1.7.8/pyproject.toml
--rw-r--r--   0        0        0    10222 2020-02-02 00:00:00.000000 eo_grow-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/__init__.py
+-rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/py.typed
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/types.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/__init__.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/base.py
+-rw-r--r--   0        0        0     7266 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/config.py
+-rw-r--r--   0        0        0    17547 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/logging.py
+-rw-r--r--   0        0        0    12606 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/pipeline.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/schemas.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/storage.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/area/__init__.py
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/area/base.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/area/batch.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/area/custom_grid.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/core/area/utm.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/__init__.py
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/batch_to_eopatch.py
+-rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/byoc.py
+-rw-r--r--   0        0        0    13959 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/download.py
+-rw-r--r--   0        0        0    12883 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/download_batch.py
+-rw-r--r--   0        0        0    16559 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/export_maps.py
+-rw-r--r--   0        0        0     9911 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/features.py
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/import_tiff.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/import_vector.py
+-rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/merge_samples.py
+-rw-r--r--   0        0        0     8620 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/prediction.py
+-rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/rasterize.py
+-rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/sampling.py
+-rw-r--r--   0        0        0     9361 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/split_grid.py
+-rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/testing.py
+-rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/training.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/pipelines/zipmap.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/tasks/__init__.py
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/tasks/batch_to_eopatch.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/tasks/common.py
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/tasks/features.py
+-rw-r--r--   0        0        0     7873 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/tasks/prediction.py
+-rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/tasks/spatial.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/tasks/testing.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/__init__.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/batch.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/eopatch_list.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/filter.py
+-rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/fs.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/general.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/grid.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/logging.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/map.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/meta.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/pipeline_chain.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/ray.py
+-rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/testing.py
+-rw-r--r--   0        0        0    10268 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/validators.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/vector.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 eo_grow-1.7.9/eogrow/utils/zipmap.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 eo_grow-1.7.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 eo_grow-1.7.9/LICENSE
+-rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 eo_grow-1.7.9/README.md
+-rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 eo_grow-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0    10222 2020-02-02 00:00:00.000000 eo_grow-1.7.9/PKG-INFO
```

### Comparing `eo_grow-1.7.8/eogrow/cli.py` & `eo_grow-1.7.9/eogrow/cli.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/types.py` & `eo_grow-1.7.9/eogrow/types.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/core/base.py` & `eo_grow-1.7.9/eogrow/core/base.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/core/config.py` & `eo_grow-1.7.9/eogrow/core/config.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/core/logging.py` & `eo_grow-1.7.9/eogrow/core/logging.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/core/pipeline.py` & `eo_grow-1.7.9/eogrow/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/core/schemas.py` & `eo_grow-1.7.9/eogrow/core/schemas.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/core/storage.py` & `eo_grow-1.7.9/eogrow/core/storage.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/core/area/base.py` & `eo_grow-1.7.9/eogrow/core/area/base.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/core/area/batch.py` & `eo_grow-1.7.9/eogrow/core/area/batch.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/core/area/custom_grid.py` & `eo_grow-1.7.9/eogrow/core/area/custom_grid.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/core/area/utm.py` & `eo_grow-1.7.9/eogrow/core/area/utm.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/batch_to_eopatch.py` & `eo_grow-1.7.9/eogrow/pipelines/batch_to_eopatch.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/byoc.py` & `eo_grow-1.7.9/eogrow/pipelines/byoc.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/download.py` & `eo_grow-1.7.9/eogrow/pipelines/download.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/download_batch.py` & `eo_grow-1.7.9/eogrow/pipelines/download_batch.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/export_maps.py` & `eo_grow-1.7.9/eogrow/pipelines/export_maps.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/features.py` & `eo_grow-1.7.9/eogrow/pipelines/features.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/import_tiff.py` & `eo_grow-1.7.9/eogrow/pipelines/import_tiff.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/import_vector.py` & `eo_grow-1.7.9/eogrow/pipelines/import_vector.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/merge_samples.py` & `eo_grow-1.7.9/eogrow/pipelines/merge_samples.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/prediction.py` & `eo_grow-1.7.9/eogrow/pipelines/prediction.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/rasterize.py` & `eo_grow-1.7.9/eogrow/pipelines/rasterize.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/sampling.py` & `eo_grow-1.7.9/eogrow/pipelines/sampling.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/split_grid.py` & `eo_grow-1.7.9/eogrow/pipelines/split_grid.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/testing.py` & `eo_grow-1.7.9/eogrow/pipelines/testing.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/training.py` & `eo_grow-1.7.9/eogrow/pipelines/training.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/pipelines/zipmap.py` & `eo_grow-1.7.9/eogrow/pipelines/zipmap.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/tasks/batch_to_eopatch.py` & `eo_grow-1.7.9/eogrow/tasks/batch_to_eopatch.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/tasks/common.py` & `eo_grow-1.7.9/eogrow/tasks/common.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/tasks/features.py` & `eo_grow-1.7.9/eogrow/tasks/features.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/tasks/prediction.py` & `eo_grow-1.7.9/eogrow/tasks/prediction.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/tasks/spatial.py` & `eo_grow-1.7.9/eogrow/tasks/spatial.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/tasks/testing.py` & `eo_grow-1.7.9/eogrow/tasks/testing.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/batch.py` & `eo_grow-1.7.9/eogrow/utils/batch.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/eopatch_list.py` & `eo_grow-1.7.9/eogrow/utils/eopatch_list.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/filter.py` & `eo_grow-1.7.9/eogrow/utils/filter.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/fs.py` & `eo_grow-1.7.9/eogrow/utils/fs.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/general.py` & `eo_grow-1.7.9/eogrow/utils/general.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/grid.py` & `eo_grow-1.7.9/eogrow/utils/grid.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/logging.py` & `eo_grow-1.7.9/eogrow/utils/logging.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/map.py` & `eo_grow-1.7.9/eogrow/utils/map.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/meta.py` & `eo_grow-1.7.9/eogrow/utils/meta.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/pipeline_chain.py` & `eo_grow-1.7.9/eogrow/utils/pipeline_chain.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/ray.py` & `eo_grow-1.7.9/eogrow/utils/ray.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/testing.py` & `eo_grow-1.7.9/eogrow/utils/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         "row_count": len(gdf),
         "crs": str(gdf.crs),
         "mean_area": _prepare_value(gdf.area.mean(), np.float64),
         "total_bounds": [_prepare_value(x, dtype=np.float64) for x in gdf.total_bounds],
         "agg_stats": _extract_dataframe_stats(gdf),
     }
 
-    if len(gdf):
+    if len(gdf) and config.num_random_values > 0:
         subsample: gpd.GeoDataFrame = gdf.sample(min(len(gdf), config.num_random_values), random_state=42)
         subsample["centroid"] = subsample.centroid.apply(_rounder)
         subsample["area"] = subsample.area
         subsample["geometry_type"] = subsample.geometry.geom_type
         subsample["some_coords"] = subsample.geometry.apply(_get_coords_sample)
 
         for col in subsample.select_dtypes(include="number").columns.values:
```

### Comparing `eo_grow-1.7.8/eogrow/utils/validators.py` & `eo_grow-1.7.9/eogrow/utils/validators.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/vector.py` & `eo_grow-1.7.9/eogrow/utils/vector.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/eogrow/utils/zipmap.py` & `eo_grow-1.7.9/eogrow/utils/zipmap.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/.gitignore` & `eo_grow-1.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/LICENSE` & `eo_grow-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/README.md` & `eo_grow-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/pyproject.toml` & `eo_grow-1.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eo_grow-1.7.8/PKG-INFO` & `eo_grow-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: eo-grow
-Version: 1.7.8
+Version: 1.7.9
 Summary: Earth observation framework for scaled-up processing in Python
 Project-URL: Homepage, https://github.com/sentinel-hub/eo-grow
 Project-URL: Documentation, https://eo-grow.readthedocs.io
 Project-URL: Issues, https://github.com/sentinel-hub/eo-grow/issues
 Project-URL: Source, https://github.com/sentinel-hub/eo-grow
 Project-URL: Forum, https://forum.sentinel-hub.com
 Author-email: Sinergise EO research team <eoresearch@sinergise.com>
```

