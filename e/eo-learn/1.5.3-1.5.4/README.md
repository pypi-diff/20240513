# Comparing `tmp/eo_learn-1.5.3.tar.gz` & `tmp/eo_learn-1.5.4.tar.gz`

## Comparing `eo_learn-1.5.3.tar` & `eo_learn-1.5.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/py.typed
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/__init__.py
--rw-r--r--   0        0        0    11589 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/constants.py
--rw-r--r--   0        0        0    27348 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/core_tasks.py
--rw-r--r--   0        0        0    39952 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/eodata.py
--rw-r--r--   0        0        0    33101 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/eodata_io.py
--rw-r--r--   0        0        0    13307 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/eodata_merge.py
--rw-r--r--   0        0        0    17615 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/eoexecution.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/eonode.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/eotask.py
--rw-r--r--   0        0        0    16816 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/eoworkflow.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/eoworkflow_tasks.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/exceptions.py
--rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/graph.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/types.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/extra/__init__.py
--rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/extra/ray.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/utils/__init__.py
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/utils/common.py
--rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/utils/fs.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/utils/logging.py
--rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/utils/parallelize.py
--rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/utils/parsing.py
--rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/utils/raster.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/utils/testing.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/core/utils/types.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/coregistration/__init__.py
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/coregistration/coregistration.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/features/__init__.py
--rw-r--r--   0        0        0     7569 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/features/feature_manipulation.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/features/ndi.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/features/utils.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/features/extra/__init__.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/features/extra/clustering.py
--rw-r--r--   0        0        0    29488 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/features/extra/interpolation.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/geometry/__init__.py
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/geometry/morphology.py
--rw-r--r--   0        0        0    22324 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/geometry/transformations.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/io/__init__.py
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/io/geometry_io.py
--rw-r--r--   0        0        0    26551 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/io/raster_io.py
--rw-r--r--   0        0        0    27642 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/io/sentinelhub_process.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/mask/__init__.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/mask/masking.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/mask/snow_mask.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/mask/extra/__init__.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/mask/extra/cloud_mask.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/ml_tools/__init__.py
--rw-r--r--   0        0        0    17865 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/ml_tools/sampling.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/visualization/__init__.py
--rw-r--r--   0        0        0     9751 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/visualization/eoexecutor.py
--rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/visualization/eopatch.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/visualization/eoworkflow.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/visualization/utils.py
--rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 eo_learn-1.5.3/eolearn/visualization/report_templates/report.html
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 eo_learn-1.5.3/.gitignore
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 eo_learn-1.5.3/LICENSE
--rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 eo_learn-1.5.3/README.md
--rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 eo_learn-1.5.3/pyproject.toml
--rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 eo_learn-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/py.typed
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/__init__.py
+-rw-r--r--   0        0        0    11589 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/constants.py
+-rw-r--r--   0        0        0    27348 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/core_tasks.py
+-rw-r--r--   0        0        0    39952 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/eodata.py
+-rw-r--r--   0        0        0    33101 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/eodata_io.py
+-rw-r--r--   0        0        0    13307 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/eodata_merge.py
+-rw-r--r--   0        0        0    17616 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/eoexecution.py
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/eonode.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/eotask.py
+-rw-r--r--   0        0        0    16816 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/eoworkflow.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/eoworkflow_tasks.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/exceptions.py
+-rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/graph.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/types.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/extra/__init__.py
+-rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/extra/ray.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/utils/__init__.py
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/utils/common.py
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/utils/fs.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/utils/logging.py
+-rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/utils/parallelize.py
+-rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/utils/parsing.py
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/utils/raster.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/utils/testing.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/core/utils/types.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/coregistration/__init__.py
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/coregistration/coregistration.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/features/__init__.py
+-rw-r--r--   0        0        0     7569 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/features/feature_manipulation.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/features/ndi.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/features/utils.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/features/extra/__init__.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/features/extra/clustering.py
+-rw-r--r--   0        0        0    29522 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/features/extra/interpolation.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/geometry/__init__.py
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/geometry/morphology.py
+-rw-r--r--   0        0        0    22324 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/geometry/transformations.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/io/__init__.py
+-rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/io/geometry_io.py
+-rw-r--r--   0        0        0    26551 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/io/raster_io.py
+-rw-r--r--   0        0        0    27641 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/io/sentinelhub_process.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/mask/__init__.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/mask/masking.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/mask/snow_mask.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/mask/extra/__init__.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/mask/extra/cloud_mask.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/ml_tools/__init__.py
+-rw-r--r--   0        0        0    17865 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/ml_tools/sampling.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/visualization/__init__.py
+-rw-r--r--   0        0        0     9813 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/visualization/eoexecutor.py
+-rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/visualization/eopatch.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/visualization/eoworkflow.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/visualization/utils.py
+-rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 eo_learn-1.5.4/eolearn/visualization/report_templates/report.html
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 eo_learn-1.5.4/.gitignore
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 eo_learn-1.5.4/LICENSE
+-rw-r--r--   0        0        0    13454 2020-02-02 00:00:00.000000 eo_learn-1.5.4/README.md
+-rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 eo_learn-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0    19969 2020-02-02 00:00:00.000000 eo_learn-1.5.4/PKG-INFO
```

### Comparing `eo_learn-1.5.3/eolearn/__init__.py` & `eo_learn-1.5.4/eolearn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Main module of the `eolearn` package."""
 
-__version__ = "1.5.3"
+__version__ = "1.5.4"
 
 import importlib.util
 import warnings
 
 SUBPACKAGES = ["core", "coregistration", "features", "geometry", "io", "mask", "ml_tools", "visualization"]
 deprecated_installs = [
     subpackage for subpackage in SUBPACKAGES if importlib.util.find_spec(f"deprecated_eolearn_{subpackage}") is not None
```

### Comparing `eo_learn-1.5.3/eolearn/core/__init__.py` & `eo_learn-1.5.4/eolearn/core/__init__.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/constants.py` & `eo_learn-1.5.4/eolearn/core/constants.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/core_tasks.py` & `eo_learn-1.5.4/eolearn/core/core_tasks.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/eodata.py` & `eo_learn-1.5.4/eolearn/core/eodata.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/eodata_io.py` & `eo_learn-1.5.4/eolearn/core/eodata_io.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/eodata_merge.py` & `eo_learn-1.5.4/eolearn/core/eodata_merge.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/eoexecution.py` & `eo_learn-1.5.4/eolearn/core/eoexecution.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         self.start_time: dt.datetime | None = None
         self.report_folder: str | None = None
         self.general_stats: dict[str, object] = {}
         self.execution_results: list[WorkflowResults] = []
 
     @staticmethod
     def _parse_and_validate_execution_kwargs(
-        execution_kwargs: Iterable[dict[EONode, dict[str, object]]]
+        execution_kwargs: Iterable[dict[EONode, dict[str, object]]],
     ) -> list[dict[EONode, dict[str, object]]]:
         """Parses and validates execution arguments provided by user and raises an error if something is wrong."""
         for input_kwargs in execution_kwargs:
             EOWorkflow.validate_input_kwargs(input_kwargs)
 
         return list(execution_kwargs)
```

### Comparing `eo_learn-1.5.3/eolearn/core/eonode.py` & `eo_learn-1.5.4/eolearn/core/eonode.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/eotask.py` & `eo_learn-1.5.4/eolearn/core/eotask.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/eoworkflow.py` & `eo_learn-1.5.4/eolearn/core/eoworkflow.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/eoworkflow_tasks.py` & `eo_learn-1.5.4/eolearn/core/eoworkflow_tasks.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/exceptions.py` & `eo_learn-1.5.4/eolearn/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/graph.py` & `eo_learn-1.5.4/eolearn/core/graph.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/types.py` & `eo_learn-1.5.4/eolearn/core/types.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/extra/ray.py` & `eo_learn-1.5.4/eolearn/core/extra/ray.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/utils/common.py` & `eo_learn-1.5.4/eolearn/core/utils/common.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/utils/fs.py` & `eo_learn-1.5.4/eolearn/core/utils/fs.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/utils/logging.py` & `eo_learn-1.5.4/eolearn/core/utils/logging.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/utils/parallelize.py` & `eo_learn-1.5.4/eolearn/core/utils/parallelize.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/utils/parsing.py` & `eo_learn-1.5.4/eolearn/core/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/utils/raster.py` & `eo_learn-1.5.4/eolearn/core/utils/raster.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/core/utils/testing.py` & `eo_learn-1.5.4/eolearn/core/utils/testing.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/coregistration/coregistration.py` & `eo_learn-1.5.4/eolearn/coregistration/coregistration.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/features/feature_manipulation.py` & `eo_learn-1.5.4/eolearn/features/feature_manipulation.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/features/ndi.py` & `eo_learn-1.5.4/eolearn/features/ndi.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/features/utils.py` & `eo_learn-1.5.4/eolearn/features/utils.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/features/extra/clustering.py` & `eo_learn-1.5.4/eolearn/features/extra/clustering.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/features/extra/interpolation.py` & `eo_learn-1.5.4/eolearn/features/extra/interpolation.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,18 +269,20 @@
 
                 new_data[:, idx] = obs_interpolating_func(resampled_times[:, np.newaxis])
 
             return new_data
 
         # array defining index correspondence between reference times and resampled times
         min_time, max_time = np.min(resampled_times), np.max(resampled_times)
-        ori2res = np.array([
-            np.abs(resampled_times - orig_time).argmin() if min_time <= orig_time <= max_time else None
-            for orig_time in times
-        ])
+        ori2res = np.array(
+            [
+                np.abs(resampled_times - orig_time).argmin() if min_time <= orig_time <= max_time else None
+                for orig_time in times
+            ]
+        )
 
         # find NaNs that start or end a time-series
         row_nans, col_nans = np.where(self._get_start_end_nans(data))
         nan_row_res_indices = np.array([index for index in ori2res[row_nans] if index is not None], dtype=np.int32)
         nan_col_res_indices = np.array([index is not None for index in ori2res[row_nans]], dtype=bool)
 
         # define time values as linear monotonically increasing over the observations
```

### Comparing `eo_learn-1.5.3/eolearn/geometry/morphology.py` & `eo_learn-1.5.4/eolearn/geometry/morphology.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/geometry/transformations.py` & `eo_learn-1.5.4/eolearn/geometry/transformations.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/io/geometry_io.py` & `eo_learn-1.5.4/eolearn/io/geometry_io.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/io/raster_io.py` & `eo_learn-1.5.4/eolearn/io/raster_io.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/io/sentinelhub_process.py` & `eo_learn-1.5.4/eolearn/io/sentinelhub_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Input tasks that collect data from `Sentinel-Hub Process API
+"""Input tasks that collect data from `Sentinel-Hub Process API
 <https://docs.sentinel-hub.com/api/latest/api/process/>`__
 
 Copyright (c) 2017- Sinergise and contributors
 For the full list of contributors, see the CREDITS file in the root directory of this source tree.
 
 This source code is licensed under the MIT license, see the LICENSE file in the root directory of this source tree.
 """
```

### Comparing `eo_learn-1.5.3/eolearn/mask/masking.py` & `eo_learn-1.5.4/eolearn/mask/masking.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/mask/snow_mask.py` & `eo_learn-1.5.4/eolearn/mask/snow_mask.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/mask/extra/cloud_mask.py` & `eo_learn-1.5.4/eolearn/mask/extra/cloud_mask.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/ml_tools/sampling.py` & `eo_learn-1.5.4/eolearn/ml_tools/sampling.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/visualization/eoexecutor.py` & `eo_learn-1.5.4/eolearn/visualization/eoexecutor.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,23 +159,25 @@
                 duration_report = "unknown"
             else:
                 duration_report = (
                     f"Between {np.min(durations):.4g} and {np.max(durations):.4g} seconds,"
                     f" usually {np.mean(durations):.4g} ± {np.std(durations):.4g} seconds"
                 )
 
-            descriptions.append({
-                "name": f"{node_name} ({node.uid})",
-                "uid": node.uid,
-                "args": {
-                    key: value.replace("<", "&lt;").replace(">", "&gt;")  # type: ignore[attr-defined]
-                    for key, value in node.task.private_task_config.init_args.items()
-                },
-                "duration_report": duration_report,
-            })
+            descriptions.append(
+                {
+                    "name": f"{node_name} ({node.uid})",
+                    "uid": node.uid,
+                    "args": {
+                        key: value.replace("<", "&lt;").replace(">", "&gt;")  # type: ignore[attr-defined]
+                        for key, value in node.task.private_task_config.init_args.items()
+                    },
+                    "duration_report": duration_report,
+                }
+            )
         return descriptions
 
     def _render_execution_tracebacks(self, formatter: pygments.formatter.Formatter) -> list:
         """Renders stack traces of those executions which failed"""
         tb_lexer = pygments.lexers.get_lexer_by_name("py3tb", stripall=True)
 
         tracebacks = []
```

### Comparing `eo_learn-1.5.3/eolearn/visualization/eopatch.py` & `eo_learn-1.5.4/eolearn/visualization/eopatch.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/visualization/eoworkflow.py` & `eo_learn-1.5.4/eolearn/visualization/eoworkflow.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/visualization/utils.py` & `eo_learn-1.5.4/eolearn/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/eolearn/visualization/report_templates/report.html` & `eo_learn-1.5.4/eolearn/visualization/report_templates/report.html`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/.gitignore` & `eo_learn-1.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/LICENSE` & `eo_learn-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eo_learn-1.5.3/README.md` & `eo_learn-1.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -198,8 +198,8 @@
 
 ## License
 
 See [LICENSE](https://github.com/sentinel-hub/eo-learn/blob/master/LICENSE).
 
 ## Acknowledgements
 
-This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreements No. 776115, No. 101004112 and No. 101059548.
+This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreements No. 776115, No. 101004112, No. 101059548 and No. 101086461.
```

### Comparing `eo_learn-1.5.3/pyproject.toml` & `eo_learn-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -68,27 +68,26 @@
 extra = ["numba>=0.53.0", "scikit-learn", "scipy", "s2cloudless"]
 visualization = ["graphviz>=0.10.1", "jinja2", "matplotlib", "pygments"]
 docs = [
     "eo-learn[FULL]",
     "jupyter",
     "nbsphinx",
     "sphinx==7.1.2",
-    "sphinx_mdinclude",
+    "sphinx_mdinclude==0.5.4",  #0.6 didn't work last time
     "sphinx_rtd_theme==1.3.0",
 ]
 dev = [
     "build",
     "eo-learn[FULL]",
     "hypothesis",
-    "moto",
+    "moto[s3]>=5.0.0",
     "mypy>=0.990",
     "pylint>=2.14.0",
     "pytest>=7.0.0",
     "pytest-cov",
-    "pytest-lazy-fixture",
     "pytest-mock",
     "twine",
     "types-python-dateutil",
 ]
 
 [project.urls]
 Homepage = "https://github.com/sentinel-hub/eo-learn"
```

### Comparing `eo_learn-1.5.3/PKG-INFO` & `eo_learn-1.5.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: eo-learn
-Version: 1.5.3
+Version: 1.5.4
 Summary: Earth observation processing framework for machine learning in Python
 Project-URL: Homepage, https://github.com/sentinel-hub/eo-learn
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Issues, https://github.com/sentinel-hub/eo-learn/issues
 Project-URL: Source, https://github.com/sentinel-hub/eo-learn
 Project-URL: Forum, https://forum.sentinel-hub.com
 Author-email: Sinergise EO research team <eoresearch@sinergise.com>
@@ -69,39 +69,68 @@
 Requires-Dist: rasterio>=1.3.8
 Requires-Dist: sentinelhub>=3.9.0
 Requires-Dist: shapely
 Requires-Dist: tqdm>=4.27
 Requires-Dist: typing-extensions>=4.5.0
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
-Requires-Dist: eo-learn[full]; extra == 'dev'
+Requires-Dist: graphviz>=0.10.1; extra == 'dev'
 Requires-Dist: hypothesis; extra == 'dev'
-Requires-Dist: moto; extra == 'dev'
+Requires-Dist: jinja2; extra == 'dev'
+Requires-Dist: matplotlib; extra == 'dev'
+Requires-Dist: moto[s3]>=5.0.0; extra == 'dev'
 Requires-Dist: mypy>=0.990; extra == 'dev'
+Requires-Dist: numba>=0.53.0; extra == 'dev'
+Requires-Dist: pygments; extra == 'dev'
 Requires-Dist: pylint>=2.14.0; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
-Requires-Dist: pytest-lazy-fixture; extra == 'dev'
 Requires-Dist: pytest-mock; extra == 'dev'
 Requires-Dist: pytest>=7.0.0; extra == 'dev'
+Requires-Dist: ray[default]; extra == 'dev'
+Requires-Dist: s2cloudless; extra == 'dev'
+Requires-Dist: s3fs; extra == 'dev'
+Requires-Dist: scikit-learn; extra == 'dev'
+Requires-Dist: scipy; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Requires-Dist: types-python-dateutil; extra == 'dev'
+Requires-Dist: zarr; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: eo-learn[full]; extra == 'docs'
+Requires-Dist: graphviz>=0.10.1; extra == 'docs'
+Requires-Dist: jinja2; extra == 'docs'
 Requires-Dist: jupyter; extra == 'docs'
+Requires-Dist: matplotlib; extra == 'docs'
 Requires-Dist: nbsphinx; extra == 'docs'
-Requires-Dist: sphinx-mdinclude; extra == 'docs'
+Requires-Dist: numba>=0.53.0; extra == 'docs'
+Requires-Dist: pygments; extra == 'docs'
+Requires-Dist: ray[default]; extra == 'docs'
+Requires-Dist: s2cloudless; extra == 'docs'
+Requires-Dist: s3fs; extra == 'docs'
+Requires-Dist: scikit-learn; extra == 'docs'
+Requires-Dist: scipy; extra == 'docs'
+Requires-Dist: sphinx-mdinclude==0.5.4; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme==1.3.0; extra == 'docs'
 Requires-Dist: sphinx==7.1.2; extra == 'docs'
+Requires-Dist: zarr; extra == 'docs'
 Provides-Extra: extra
 Requires-Dist: numba>=0.53.0; extra == 'extra'
 Requires-Dist: s2cloudless; extra == 'extra'
 Requires-Dist: scikit-learn; extra == 'extra'
 Requires-Dist: scipy; extra == 'extra'
 Provides-Extra: full
-Requires-Dist: eo-learn[extra,ray,visualization,zarr]; extra == 'full'
+Requires-Dist: graphviz>=0.10.1; extra == 'full'
+Requires-Dist: jinja2; extra == 'full'
+Requires-Dist: matplotlib; extra == 'full'
+Requires-Dist: numba>=0.53.0; extra == 'full'
+Requires-Dist: pygments; extra == 'full'
+Requires-Dist: ray[default]; extra == 'full'
+Requires-Dist: s2cloudless; extra == 'full'
+Requires-Dist: s3fs; extra == 'full'
+Requires-Dist: scikit-learn; extra == 'full'
+Requires-Dist: scipy; extra == 'full'
+Requires-Dist: zarr; extra == 'full'
 Provides-Extra: ray
 Requires-Dist: ray[default]; extra == 'ray'
 Provides-Extra: visualization
 Requires-Dist: graphviz>=0.10.1; extra == 'visualization'
 Requires-Dist: jinja2; extra == 'visualization'
 Requires-Dist: matplotlib; extra == 'visualization'
 Requires-Dist: pygments; extra == 'visualization'
@@ -310,8 +339,8 @@
 
 ## License
 
 See [LICENSE](https://github.com/sentinel-hub/eo-learn/blob/master/LICENSE).
 
 ## Acknowledgements
 
-This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreements No. 776115, No. 101004112 and No. 101059548.
+This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreements No. 776115, No. 101004112, No. 101059548 and No. 101086461.
```

