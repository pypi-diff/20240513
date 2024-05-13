# Comparing `tmp/valor_client-0.24.0.tar.gz` & `tmp/valor_client-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valor_client-0.24.0.tar", last modified: Thu May  9 22:43:42 2024, max compression
+gzip compressed data, was "valor_client-0.25.0.tar", last modified: Mon May 13 19:10:08 2024, max compression
```

## Comparing `valor_client-0.24.0.tar` & `valor_client-0.25.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.013657 valor_client-0.24.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-09 22:43:37.000000 valor_client-0.24.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-09 22:43:42.013657 valor_client-0.24.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-09 22:43:37.000000 valor_client-0.24.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 22:43:42.013657 valor_client-0.24.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-09 22:43:37.000000 valor_client-0.24.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.005657 valor_client-0.24.0/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.005657 valor_client-0.24.0/unit-tests/coretypes/
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/coretypes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/coretypes/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/coretypes/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.005657 valor_client-0.24.0/unit-tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/schemas/test_evaluation_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/schemas/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/schemas/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/schemas/test_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.005657 valor_client-0.24.0/unit-tests/symbolic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.009657 valor_client-0.24.0/unit-tests/symbolic/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/collections/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/collections/test_static_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/collections/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.009657 valor_client-0.24.0/unit-tests/symbolic/types/
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/types/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/symbolic/types/test_symbolic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-09 22:43:37.000000 valor_client-0.24.0/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.009657 valor_client-0.24.0/valor/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29488 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54922 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/metatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.009657 valor_client-0.24.0/valor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.009657 valor_client-0.24.0/valor/schemas/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/symbolic/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/symbolic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/schemas/symbolic/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-09 22:43:37.000000 valor_client-0.24.0/valor/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:43:42.013657 valor_client-0.24.0/valor_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-09 22:43:41.000000 valor_client-0.24.0/valor_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-09 22:43:42.000000 valor_client-0.24.0/valor_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 22:43:41.000000 valor_client-0.24.0/valor_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 22:43:41.000000 valor_client-0.24.0/valor_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 22:43:41.000000 valor_client-0.24.0/valor_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.094879 valor_client-0.25.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 19:10:03.000000 valor_client-0.25.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-13 19:10:08.094879 valor_client-0.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 19:10:03.000000 valor_client-0.25.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:10:08.094879 valor_client-0.25.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-13 19:10:03.000000 valor_client-0.25.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/coretypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/coretypes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/coretypes/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/coretypes/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/schemas/test_evaluation_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/schemas/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/schemas/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/symbolic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/symbolic/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/collections/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/collections/test_static_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/collections/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/symbolic/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/types/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38078 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/types/test_symbolic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.090878 valor_client-0.25.0/valor/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29488 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54799 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/metatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.090878 valor_client-0.25.0/valor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.090878 valor_client-0.25.0/valor/schemas/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/symbolic/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/symbolic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59078 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/symbolic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.090878 valor_client-0.25.0/valor_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-13 19:10:08.000000 valor_client-0.25.0/valor_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-13 19:10:08.000000 valor_client-0.25.0/valor_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:10:08.000000 valor_client-0.25.0/valor_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 19:10:08.000000 valor_client-0.25.0/valor_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 19:10:08.000000 valor_client-0.25.0/valor_client.egg-info/top_level.txt
```

### Comparing `valor_client-0.24.0/LICENSE` & `valor_client-0.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/PKG-INFO` & `valor_client-0.25.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.24.0
+Version: 0.25.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.24.0/pyproject.toml` & `valor_client-0.25.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/unit-tests/conftest.py` & `valor_client-0.25.0/unit-tests/conftest.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/unit-tests/coretypes/test_core.py` & `valor_client-0.25.0/unit-tests/coretypes/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,21 +208,19 @@
         ),
         Annotation(
             task_type=enums.TaskType.CLASSIFICATION,
             labels=[scored_label],
         ),
     ]
 
-    # valid
-    Prediction(datum=datum, annotations=pds)
-
-    string = str(Prediction(datum=datum, annotations=pds))
+    pred = Prediction(datum=datum, annotations=pds)
+    string = str(pred)
     assert (
         string
-        == "{'datum': {'uid': 'somefile', 'metadata': {}}, 'annotations': [{'task_type': 'classification', 'metadata': {}, 'labels': [{'key': 'test', 'value': 'value', 'score': 1.0}], 'bounding_box': None, 'polygon': None, 'raster': None, 'embedding': None}, {'task_type': 'classification', 'metadata': {}, 'labels': [{'key': 'test', 'value': 'value', 'score': 1.0}], 'bounding_box': None, 'polygon': None, 'raster': None, 'embedding': None}]}"
+        == "{'datum': {'uid': 'somefile', 'metadata': {}}, 'annotations': [{'task_type': <TaskType.CLASSIFICATION: 'classification'>, 'metadata': {}, 'labels': [{'key': 'test', 'value': 'value', 'score': 1.0}], 'bounding_box': None, 'polygon': None, 'raster': None, 'embedding': None}, {'task_type': <TaskType.CLASSIFICATION: 'classification'>, 'metadata': {}, 'labels': [{'key': 'test', 'value': 'value', 'score': 1.0}], 'bounding_box': None, 'polygon': None, 'raster': None, 'embedding': None}]}"
     )
     assert "dataset_name" not in string
 
     # test `__post_init__`
     with pytest.raises(TypeError):
         Prediction(datum="datum", annotations=pds)  # type: ignore
     with pytest.raises(TypeError) as e:
```

### Comparing `valor_client-0.24.0/unit-tests/coretypes/test_evaluation.py` & `valor_client-0.25.0/unit-tests/coretypes/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/unit-tests/coretypes/test_filtering.py` & `valor_client-0.25.0/unit-tests/coretypes/test_filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             Label.score > 0.75,
             Annotation.polygon.area > 1000,
             Annotation.polygon.area < 5000,
             (Annotation.raster.area > 100) & (Annotation.raster.area < 500),
             Dataset.metadata["some_str"] == "foobar",
             Dataset.metadata["some_float"] >= 0.123,
             Dataset.metadata["some_datetime"] > datetime.timedelta(days=1),
-            Dataset.metadata["some_geospatial"].intersects(polygon),
+            Dataset.metadata["some_geospatial"].intersects(polygon),  # type: ignore
         ]
     )
 
     filter_from_dictionary = _format_filter(
         {
             "dataset_names": ["a", "b", "c"],
             "model_names": ["x", "y", "z"],
```

### Comparing `valor_client-0.24.0/unit-tests/schemas/test_filters.py` & `valor_client-0.25.0/unit-tests/schemas/test_filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/unit-tests/schemas/test_geojson.py` & `valor_client-0.25.0/unit-tests/schemas/test_geojson.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/unit-tests/schemas/test_label.py` & `valor_client-0.25.0/unit-tests/schemas/test_label.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/unit-tests/symbolic/collections/test_dictionary.py` & `valor_client-0.25.0/unit-tests/symbolic/collections/test_dictionary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import datetime
 
 import pytest
 
-from valor.schemas import Dictionary, Float, Integer
+from valor.schemas import Dictionary
 
 
 def test_validate_metadata():
     Dictionary({"test": "test"})
     Dictionary({"test": 1})
     Dictionary({"test": 1.0})
 
     with pytest.raises(TypeError):
         Dictionary({123: 123})  # type: ignore
 
     # Check int to float conversion
-    assert type(Dictionary({"test": 1})["test"]) is Integer
-    assert type(Dictionary({"test": 1.0})["test"]) is Float
+    assert type(Dictionary({"test": 1})["test"]) is int
+    assert type(Dictionary({"test": 1.0})["test"]) is float
 
 
 def test_init_dictionary_from_builtin_dict():
     metadata = dict()
     metadata["a"] = int(123.4)
     metadata["b"] = float(123.4)
     metadata["c"] = str(123.4)
```

### Comparing `valor_client-0.24.0/unit-tests/symbolic/collections/test_static_collection.py` & `valor_client-0.25.0/unit-tests/symbolic/collections/test_static_collection.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,18 +103,25 @@
     # test dictionary generation
     assert v1.to_dict() == {
         "type": "a",
         "value": {"w": 101, "x": 0.123, "y": "foobar", "z": True},
     }
 
     # test value members
-    assert v1.w.to_dict() == {"type": "integer", "value": 101}
-    assert v1.x.to_dict() == {"type": "float", "value": 0.123}
-    assert v1.y.to_dict() == {"type": "string", "value": "foobar"}
-    assert v1.z.to_dict() == {"type": "bool", "value": True}
+    assert isinstance(v1.w, int)
+    assert v1.w == 101
+
+    assert isinstance(v1.x, float)
+    assert v1.x == 0.123
+
+    assert isinstance(v1.y, str)
+    assert v1.y == "foobar"
+
+    assert isinstance(v1.z, bool)
+    assert v1.z is True
 
 
 def test__get_static_types():
     class A(StaticCollection):
         w: Integer
         x: "Float"
         y: "String"
```

### Comparing `valor_client-0.24.0/unit-tests/symbolic/collections/test_structures.py` & `valor_client-0.25.0/unit-tests/symbolic/collections/test_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
             "key": None,
             "attribute": None,
         },
     }
 
     # test creating valued lists
     variable = List[Float]([0.1, 0.2, 0.3])
-    assert variable.__str__() == "[0.1, 0.2, 0.3]"
+    assert variable.__str__() == "[Float(0.1), Float(0.2), Float(0.3)]"
     assert variable.to_dict() == {
         "type": "list[float]",
         "value": [0.1, 0.2, 0.3],
     }
 
     # test setting value in list by index
     assert variable[1].get_value() == 0.2
```

### Comparing `valor_client-0.24.0/unit-tests/symbolic/test_operators.py` & `valor_client-0.25.0/unit-tests/symbolic/test_operators.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,32 +23,40 @@
     return (x, y, z)
 
 
 def test_function(variables):
     x, y, z = variables
 
     # test stringify
-    assert Function(x, y, z).__repr__() == "Function(1, '2', 0.3)"
-    assert Function(x, y, z).__str__() == "Function(1, '2', 0.3)"
+    assert (
+        Function(x, y, z).__repr__()
+        == "Function(Integer(1), String('2'), Float(0.3))"
+    )
+    assert (
+        Function(x, y, z).__str__()
+        == "Function(Integer(1), String('2'), Float(0.3))"
+    )
 
     # test dictionary generation
     assert Function(x, y, z).to_dict() == {
         "op": "function",
         "args": [
             {"type": "integer", "value": 1},
             {"type": "string", "value": "2"},
             {"type": "float", "value": 0.3},
         ],
     }
 
     # test stringify w/ operator
     assert issubclass(And, Function)
     assert And._operator is not None
-    assert And(x, y, z).__repr__() == "And(1, '2', 0.3)"
-    assert And(x, y, z).__str__() == "(1 & '2' & 0.3)"
+    assert (
+        And(x, y, z).__repr__() == "And(Integer(1), String('2'), Float(0.3))"
+    )
+    assert And(x, y, z).__str__() == "(Integer(1) & String('2') & Float(0.3))"
 
     # test logical operators
     assert type(Function(x) & Function(y)) is And
     assert type(Function(x) | Function(y)) is Or
     assert type(Function(x) ^ Function(y)) is Xor
     assert type(~Function(x)) is Negate
```

### Comparing `valor_client-0.24.0/unit-tests/symbolic/types/test_schemas.py` & `valor_client-0.25.0/unit-tests/symbolic/types/test_schemas.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/unit-tests/symbolic/types/test_symbolic_types.py` & `valor_client-0.25.0/unit-tests/symbolic/types/test_symbolic_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     )
     assert s != "symbol"
 
 
 def _test_symbolic_outputs(v, s=Symbol(name="test")):
     assert s.to_dict() == v.to_dict()
     assert s.to_dict() == v.get_symbol().to_dict()
-    assert s.__repr__() == v.__repr__()
+    assert f"Variable({s.__repr__()})" == v.__repr__()
     assert s.__str__() == v.__str__()
     assert v.is_symbolic and not v.is_value
 
     with pytest.raises(TypeError):
         v.get_value()
```

### Comparing `valor_client-0.24.0/unit-tests/test_client.py` & `valor_client-0.25.0/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/unit-tests/test_viz.py` & `valor_client-0.25.0/unit-tests/test_viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     detections = [
         GroundTruth(
             datum=ImageMetadata.create("test", 300, 300).datum,
             annotations=[
                 Annotation(
                     task_type=TaskType.OBJECT_DETECTION,
                     labels=[Label(key="k", value="v")],
-                    polygon=Polygon(bounding_poly.get_value()),
+                    polygon=bounding_poly,
                 )
             ],
         ),
     ]
     img = PIL.Image.new("RGB", (300, 300))
 
     img = draw_detections_on_image(detections, img)
```

### Comparing `valor_client-0.24.0/valor/__init__.py` & `valor_client-0.25.0/valor/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/valor/client.py` & `valor_client-0.25.0/valor/client.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/valor/coretypes.py` & `valor_client-0.25.0/valor/coretypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         annotations : List[Annotation]
             The list of ground truth annotations.
         """
         super().__init__(datum=datum, annotations=annotations)
 
         for annotation in self.annotations:
             for label in annotation.labels:
-                if label.score.get_value() is not None:
+                if label.score is not None:
                     raise ValueError(
                         "GroundTruth labels should not have scores."
                     )
 
 
 class Prediction(StaticCollection):
     """
@@ -156,31 +156,31 @@
         annotations : List[Annotation]
             The list of predicted annotations.
         """
         super().__init__(datum=datum, annotations=annotations)
 
         # validation
         for annotation in self.annotations:
-            task_type = annotation.task_type.get_value()
+            task_type = annotation.task_type
             if task_type in [
                 TaskType.CLASSIFICATION,
                 TaskType.OBJECT_DETECTION,
             ]:
                 for label in annotation.labels:
-                    label_score = label.score._value
+                    label_score = label.score
                     if label_score is None:
                         raise ValueError(
                             f"For task type `{task_type}` prediction labels must have scores, but got `None`"
                         )
             if task_type == TaskType.CLASSIFICATION:
 
                 label_keys_to_sum = {}
                 for scored_label in annotation.labels:
-                    label_key = scored_label.key.get_value()
-                    label_score = scored_label.score.get_value()
+                    label_key = scored_label.key
+                    label_score = scored_label.score
                     if label_key not in label_keys_to_sum:
                         label_keys_to_sum[label_key] = 0.0
                     label_keys_to_sum[label_key] += label_score
 
                 for k, total_score in label_keys_to_sum.items():
                     if abs(total_score - 1) > 1e-5:
                         raise ValueError(
@@ -547,17 +547,14 @@
         Returns
         ----------
         Union[GroundTruth, None]
             The matching ground truth or 'None' if it doesn't exist.
         """
         return Client(self.conn).get_groundtruth(dataset=self, datum=datum)
 
-    def get_name(self) -> str:
-        return self.name.get_value()
-
     def get_labels(
         self,
     ) -> List[Label]:
         """
         Get all labels associated with a given dataset.
 
         Returns
@@ -587,15 +584,15 @@
         if isinstance(filter_, Filter):
             filter_ = asdict(filter_)
 
         if filter_.get("dataset_names"):
             raise ValueError(
                 "Cannot filter by dataset_names when calling `Dataset.get_datums`."
             )
-        filter_["dataset_names"] = [self.get_name()]
+        filter_["dataset_names"] = [self.name]  # type: ignore
         return Client(self.conn).get_datums(filter_by=filter_)
 
     def get_evaluations(
         self,
         metrics_to_sort_by: Optional[
             Dict[str, Union[Dict[str, str], str]]
         ] = None,
@@ -645,15 +642,15 @@
 
             datum_metadata: list of the unique metadata dictionaries in the dataset that are associated
             to datums
 
             groundtruth_annotation_metadata: list of the unique metadata dictionaries in the dataset that are
             associated to annotations
         """
-        return Client(self.conn).get_dataset_summary(self.get_name())
+        return Client(self.conn).get_dataset_summary(self.name)  # type: ignore
 
     def finalize(
         self,
     ):
         """
         Finalizes the dataset such that new ground truths cannot be added to it.
         """
@@ -667,15 +664,15 @@
         Delete the dataset from the back end.
 
         Parameters
         ----------
         timeout : int, default=0
             Sets a timeout in seconds.
         """
-        Client(self.conn).delete_dataset(self.get_name(), timeout)
+        Client(self.conn).delete_dataset(self.name, timeout)  # type: ignore
 
 
 class Model(StaticCollection):
     """
     A class describing a model that was trained on a particular dataset.
 
     Attributes
@@ -804,17 +801,14 @@
         """
         Client(self.conn).create_predictions(
             dataset=dataset,
             model=self,
             predictions=predictions,
         )
 
-    def get_name(self) -> str:
-        return self.name.get_value()
-
     def get_prediction(
         self, dataset: Union[Dataset, str], datum: Union[Datum, str]
     ) -> Union[Prediction, None]:
         """
         Get a particular prediction.
 
         Parameters
@@ -847,31 +841,29 @@
         filter_by: Optional[FilterType] = None,
     ) -> Filter:
         """Formats the 'datum_filter' for any evaluation requests."""
 
         # get list of dataset names
         dataset_names_from_obj = []
         if isinstance(datasets, list):
-            dataset_names_from_obj = [
-                dataset.get_name() for dataset in datasets
-            ]
+            dataset_names_from_obj = [dataset.name for dataset in datasets]
         elif isinstance(datasets, Dataset):
-            dataset_names_from_obj = [datasets.get_name()]
+            dataset_names_from_obj = [datasets.name]
 
         # create a 'schemas.Filter' object from the constraints.
         filter_ = _format_filter(filter_by)
 
         # reset model name
         filter_.model_names = None
         filter_.model_metadata = None
 
         # set dataset names
         if not filter_.dataset_names:
             filter_.dataset_names = []
-        filter_.dataset_names.extend(dataset_names_from_obj)
+        filter_.dataset_names.extend(dataset_names_from_obj)  # type: ignore
         return filter_
 
     def _create_label_map(
         self,
         label_map: Optional[Dict[Label, Label]],
     ) -> Union[List[List[List[str]]], None]:
         """Convert a dictionary of label maps to a serializable list format."""
@@ -888,26 +880,23 @@
                 "label_map should be a dictionary with valid Labels for both the key and value."
             )
 
         return_value = []
         for key, value in label_map.items():
             if not all(
                 [
-                    (
-                        isinstance(v.key._value, str)
-                        and isinstance(v.value._value, str)
-                    )
+                    (isinstance(v.key, str) and isinstance(v.value, str))
                     for v in [key, value]
                 ]
             ):
                 raise TypeError
             return_value.append(
                 [
-                    [key.key._value, key.value._value],
-                    [value.key._value, value.value._value],
+                    [key.key, key.value],
+                    [value.key, value.value],
                 ]
             )
         return return_value
 
     def evaluate_classification(
         self,
         datasets: Optional[Union[Dataset, List[Dataset]]] = None,
@@ -941,15 +930,15 @@
             raise ValueError(
                 "Evaluation requires the definition of either datasets, dataset filters or both."
             )
 
         # format request
         datum_filter = self._format_constraints(datasets, filter_by)
         request = EvaluationRequest(
-            model_names=[self.get_name()],
+            model_names=[self.name],  # type: ignore
             datum_filter=datum_filter,
             parameters=EvaluationParameters(
                 task_type=TaskType.CLASSIFICATION,
                 label_map=self._create_label_map(label_map=label_map),
                 compute_pr_curves=compute_pr_curves,
             ),
             meta={},
@@ -1024,15 +1013,15 @@
             label_map=self._create_label_map(label_map=label_map),
             recall_score_threshold=recall_score_threshold,
             compute_pr_curves=compute_pr_curves,
             pr_curve_iou_threshold=pr_curve_iou_threshold,
         )
         datum_filter = self._format_constraints(datasets, filter_by)
         request = EvaluationRequest(
-            model_names=[self.get_name()],
+            model_names=[self.name],  # type: ignore
             datum_filter=datum_filter,
             parameters=parameters,
             meta={},
         )
 
         # create evaluation
         evaluation = Client(self.conn).evaluate(
@@ -1067,15 +1056,15 @@
         -------
         Evaluation
             A job object that can be used to track the status of the job and get the metrics of it upon completion
         """
         # format request
         datum_filter = self._format_constraints(datasets, filter_by)
         request = EvaluationRequest(
-            model_names=[self.get_name()],
+            model_names=[self.name],  # type: ignore
             datum_filter=datum_filter,
             parameters=EvaluationParameters(
                 task_type=TaskType.SEMANTIC_SEGMENTATION,
                 label_map=self._create_label_map(label_map=label_map),
             ),
             meta={},
         )
@@ -1093,15 +1082,15 @@
         Delete the `Model` object from the back end.
 
         Parameters
         ----------
         timeout : int, default=0
             Sets a timeout in seconds.
         """
-        Client(self.conn).delete_model(self.get_name(), timeout)
+        Client(self.conn).delete_model(self.name, timeout)  # type: ignore
 
     def get_labels(
         self,
     ) -> List[Label]:
         """
         Get all labels associated with a given model.
 
@@ -1206,19 +1195,19 @@
 
         Returns
         ------
         List[valor.Label]
             A list of labels.
         """
         dataset_name = (
-            dataset.get_name() if isinstance(dataset, Dataset) else dataset
+            dataset.name if isinstance(dataset, Dataset) else dataset
         )
         return [
             Label(**label)
-            for label in self.conn.get_labels_from_dataset(dataset_name)
+            for label in self.conn.get_labels_from_dataset(dataset_name)  # type: ignore
         ]
 
     def get_labels_from_model(self, model: Union[Model, str]) -> List[Label]:
         """
         Get all labels associated with a model's ground truths.
 
         Parameters
@@ -1227,18 +1216,18 @@
             The model to search by.
 
         Returns
         ------
         List[valor.Label]
             A list of labels.
         """
-        model_name = model.get_name() if isinstance(model, Model) else model
+        model_name = model.name if isinstance(model, Model) else model
         return [
             Label(**label)
-            for label in self.conn.get_labels_from_model(model_name)
+            for label in self.conn.get_labels_from_model(model_name)  # type: ignore
         ]
 
     def create_dataset(
         self,
         dataset: Union[Dataset, dict],
     ) -> None:
         """
@@ -1274,15 +1263,15 @@
             if not isinstance(groundtruth, GroundTruth):
                 raise TypeError(
                     f"Expected ground truth to be of type 'valor.GroundTruth' not '{type(groundtruth)}'."
                 )
             if not isinstance(groundtruth.annotations._value, list):
                 raise TypeError
             groundtruth_dict = groundtruth.encode_value()
-            groundtruth_dict["dataset_name"] = dataset.get_name()
+            groundtruth_dict["dataset_name"] = dataset.name
             groundtruths_json.append(groundtruth_dict)
         self.conn.create_groundtruths(groundtruths_json)
 
     def get_groundtruth(
         self,
         dataset: Union[Dataset, str],
         datum: Union[Datum, str],
@@ -1299,20 +1288,20 @@
 
         Returns
         ----------
         Union[GroundTruth, None]
             The matching ground truth or 'None' if it doesn't exist.
         """
         dataset_name = (
-            dataset.get_name() if isinstance(dataset, Dataset) else dataset
+            dataset.name if isinstance(dataset, Dataset) else dataset
         )
-        datum_uid = datum.get_uid() if isinstance(datum, Datum) else datum
+        datum_uid = datum.uid if isinstance(datum, Datum) else datum
         try:
             resp = self.conn.get_groundtruth(
-                dataset_name=dataset_name, datum_uid=datum_uid
+                dataset_name=dataset_name, datum_uid=datum_uid  # type: ignore
             )
             resp.pop("dataset_name")
             return GroundTruth.decode_value(resp)
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
@@ -1323,17 +1312,17 @@
 
         Parameters
         ----------
         dataset : str
             The dataset to be finalized.
         """
         dataset_name = (
-            dataset.get_name() if isinstance(dataset, Dataset) else dataset
+            dataset.name if isinstance(dataset, Dataset) else dataset
         )
-        return self.conn.finalize_dataset(name=dataset_name)
+        return self.conn.finalize_dataset(name=dataset_name)  # type: ignore
 
     def get_dataset(
         self,
         name: str,
     ) -> Union[Dataset, None]:
         """
         Gets a dataset by name.
@@ -1423,17 +1412,17 @@
             The UID of the datum.
         Returns
         -------
         valor.Datum
             The requested datum or 'None' if it doesn't exist.
         """
         dataset_name = (
-            dataset.get_name() if isinstance(dataset, Dataset) else dataset
+            dataset.name if isinstance(dataset, Dataset) else dataset
         )
-        resp = self.conn.get_datum(dataset_name=dataset_name, uid=uid)
+        resp = self.conn.get_datum(dataset_name=dataset_name, uid=uid)  # type: ignore
         return Datum.decode_value(resp)
 
     def get_dataset_status(
         self,
         name: str,
     ) -> Union[TableStatus, None]:
         """
@@ -1535,16 +1524,16 @@
             if not isinstance(prediction, Prediction):
                 raise TypeError(
                     f"Expected prediction to be of type 'valor.Prediction' not '{type(prediction)}'."
                 )
             if not isinstance(prediction.annotations._value, list):
                 raise TypeError
             prediction_dict = prediction.encode_value()
-            prediction_dict["dataset_name"] = dataset.get_name()
-            prediction_dict["model_name"] = model.get_name()
+            prediction_dict["dataset_name"] = dataset.name
+            prediction_dict["model_name"] = model.name
             predictions_json.append(prediction_dict)
         self.conn.create_predictions(predictions_json)
 
     def get_prediction(
         self,
         dataset: Union[Dataset, str],
         model: Union[Model, str],
@@ -1564,41 +1553,41 @@
 
         Returns
         ----------
         Union[Prediction, None]
             The matching prediction or 'None' if it doesn't exist.
         """
         dataset_name = (
-            dataset.get_name() if isinstance(dataset, Dataset) else dataset
+            dataset.name if isinstance(dataset, Dataset) else dataset
         )
-        model_name = model.get_name() if isinstance(model, Model) else model
-        datum_uid = datum.get_uid() if isinstance(datum, Datum) else datum
+        model_name = model.name if isinstance(model, Model) else model
+        datum_uid = datum.uid if isinstance(datum, Datum) else datum
 
         resp = self.conn.get_prediction(
-            dataset_name=dataset_name,
-            model_name=model_name,
-            datum_uid=datum_uid,
+            dataset_name=dataset_name,  # type: ignore
+            model_name=model_name,  # type: ignore
+            datum_uid=datum_uid,  # type: ignore
         )
         resp.pop("dataset_name")
         resp.pop("model_name")
         return Prediction.decode_value(resp)
 
     def finalize_inferences(
         self, dataset: Union[Dataset, str], model: Union[Model, str]
     ) -> None:
         """
         Finalizes a model-dataset pairing such that new predictions cannot be added to it.
         """
         dataset_name = (
-            dataset.get_name() if isinstance(dataset, Dataset) else dataset
+            dataset.name if isinstance(dataset, Dataset) else dataset
         )
-        model_name = model.get_name() if isinstance(model, Model) else model
+        model_name = model.name if isinstance(model, Model) else model
         return self.conn.finalize_inferences(
-            dataset_name=dataset_name,
-            model_name=model_name,
+            dataset_name=dataset_name,  # type: ignore
+            model_name=model_name,  # type: ignore
         )
 
     def get_model(
         self,
         name: str,
     ) -> Union[Model, None]:
         """
@@ -1690,18 +1679,18 @@
             The model to search by.
 
         Returns
         -------
         List[Evaluation]
             A list of evaluations.
         """
-        model_name = model.get_name() if isinstance(model, Model) else model
+        model_name = model.name if isinstance(model, Model) else model
         return [
             Evaluation(**evaluation, connection=self.conn)
-            for evaluation in self.conn.get_model_eval_requests(model_name)
+            for evaluation in self.conn.get_model_eval_requests(model_name)  # type: ignore
         ]
 
     def delete_model(self, name: str, timeout: int = 0) -> None:
         """
         Deletes a model.
 
         Parameters
@@ -1750,29 +1739,29 @@
 
         Returns
         -------
         List[valor.Evaluation]
             A list of evaluations.
         """
         if isinstance(datasets, list):
-            datasets = [
-                element.get_name() if isinstance(element, Dataset) else element
+            datasets = [  # type: ignore
+                element.name if isinstance(element, Dataset) else element
                 for element in datasets
             ]
         if isinstance(models, list):
-            models = [
-                element.get_name() if isinstance(element, Model) else element
+            models = [  # type: ignore
+                element.name if isinstance(element, Model) else element
                 for element in models
             ]
         return [
             Evaluation(connection=self.conn, **evaluation)
             for evaluation in self.conn.get_evaluations(
                 evaluation_ids=evaluation_ids,
-                models=models,
-                datasets=datasets,
+                models=models,  # type: ignore
+                datasets=datasets,  # type: ignore
                 metrics_to_sort_by=metrics_to_sort_by,
             )
         ]
 
     def evaluate(
         self, request: EvaluationRequest, allow_retries: bool = False
     ) -> List[Evaluation]:
```

### Comparing `valor_client-0.24.0/valor/enums.py` & `valor_client-0.25.0/valor/enums.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/valor/exceptions.py` & `valor_client-0.25.0/valor/exceptions.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/valor/metatypes.py` & `valor_client-0.25.0/valor/metatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,14 @@
             The `Datum` to extract metadata from.
         """
         if not isinstance(datum, Datum):
             raise TypeError
         elif datum.is_symbolic:
             raise ValueError
 
-        height = int(datum.metadata.get_value()["height"].get_value())
-        width = int(datum.metadata.get_value()["width"].get_value())
-        datum.metadata["height"] = Integer(height)
-        datum.metadata["width"] = Integer(width)
         self.datum = datum
 
     @classmethod
     def create(
         cls,
         uid: str,
         height: int,
@@ -88,23 +84,23 @@
         """
         width, height = image.size
         return cls.create(uid=uid, height=height, width=width)
 
     @property
     def height(self) -> int:
         """Returns image height in pixels."""
-        value = self.datum.metadata["height"].get_value()
+        value = self.datum.metadata["height"]
         if not isinstance(value, int):
             raise TypeError
         return int(value)
 
     @property
     def width(self) -> int:
         """Returns image width in pixels."""
-        value = self.datum.metadata["width"].get_value()
+        value = self.datum.metadata["width"]
         if not isinstance(value, int):
             raise TypeError
         return int(value)
 
 
 class VideoFrameMetadata:
     """
```

### Comparing `valor_client-0.24.0/valor/schemas/__init__.py` & `valor_client-0.25.0/valor/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/valor/schemas/evaluation.py` & `valor_client-0.25.0/valor/schemas/evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/valor/schemas/filters.py` & `valor_client-0.25.0/valor/schemas/filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/valor/schemas/symbolic/collections.py` & `valor_client-0.25.0/valor/schemas/symbolic/collections.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from valor.schemas.symbolic.types import List as SymbolicList
 from valor.schemas.symbolic.types import (
     Polygon,
     Raster,
     String,
     TaskTypeEnum,
     Variable,
+    _convert_simple_variables_to_standard_types,
     get_type_by_name,
 )
 
 
 def _get_schema_type_by_name(name: str):
     types_ = {
         "label": Label,
@@ -108,14 +109,20 @@
                 else:
                     return __fmt(__value)
         return __value
 
     def __setattr__(self, __name: str, __value: Any) -> None:
         super().__setattr__(__name, self.format(__name, __value))
 
+    def __getattribute__(self, __name: str) -> Any:
+        ret = super().__getattribute__(__name)
+        if isinstance(ret, Variable) and ret.is_value:
+            return _convert_simple_variables_to_standard_types(ret)
+        return ret
+
     @classmethod
     def __validate__(cls, value: Any):
         """Validate typing."""
         if value is not None:
             raise TypeError(
                 "A StaticCollection does not store an internal value."
             )
@@ -132,15 +139,16 @@
             else:
                 kwargs[k] = v
         return cls(**kwargs)
 
     def encode_value(self):
         """Encode object to JSON compatible dictionary."""
         return {
-            k: v.encode_value() for k, v in self._get_dynamic_values().items()
+            k: (v.encode_value() if hasattr(v, "encode_value") else v)
+            for k, v in self._get_dynamic_values().items()
         }
 
     @classmethod
     def _get_static_types(cls) -> Dict[str, type]:
         """Returns any static members that inherit from 'Variable'."""
         fields = getattr(cls, "__annotations__", dict())
         retval = dict()
@@ -161,15 +169,15 @@
             name: self.__getattribute__(name)
             for name in self._get_static_types().keys()
         }
 
     def __repr__(self):
         if self.is_symbolic:
             return super().__repr__()
-        return self.encode_value().__repr__()
+        return f"{self.__class__.__name__}({self.encode_value().__repr__()})"
 
     def __str__(self):
         if self.is_symbolic:
             return super().__str__()
         return str(self.encode_value())
 
 
@@ -230,19 +238,15 @@
         Defines how the `Label` is turned into a tuple.
 
         Returns
         ----------
         tuple
             A tuple of the `Label's` arguments.
         """
-        return (
-            self.key.get_value(),
-            self.value.get_value(),
-            self.score.get_value(),
-        )
+        return (self.key, self.value, self.score)
 
 
 class Annotation(StaticCollection):
     """
     A class used to annotate `GroundTruths` and `Predictions`.
 
     Attributes
@@ -414,11 +418,7 @@
         ----------
         uid : str
             The UID of the datum.
         metadata : dict, optional
             A dictionary of metadata that describes the datum.
         """
         super().__init__(uid=uid, metadata=metadata if metadata else dict())
-
-    def get_uid(self) -> str:
-        """Extracts the uid from a datum instance."""
-        return self.uid.get_value()
```

### Comparing `valor_client-0.24.0/valor/schemas/symbolic/operators.py` & `valor_client-0.25.0/valor/schemas/symbolic/operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/valor/schemas/symbolic/types.py` & `valor_client-0.25.0/valor/schemas/symbolic/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,29 @@
     Negate,
     Or,
     Outside,
     Xor,
 )
 
 
+def _convert_simple_variables_to_standard_types(var: typing.Any):
+    """Converts a variable to a standard type. This operates recursively.
+    in the case that the variable represents a dictionary
+    """
+    from valor.schemas.symbolic.collections import StaticCollection
+
+    if isinstance(var, StaticCollection):
+        return var
+    if isinstance(var, Variable):
+        val = var.get_value()
+        if isinstance(val, (str, int, float, bool, type(None))):
+            var = val
+    return var
+
+
 class Symbol:
     """
     A symbol contains no value and is defined by the tuple (owner, name, key, attribute).
 
     Examples
     --------
     >>> Symbol(name="a")
@@ -124,15 +139,15 @@
         self,
         value: typing.Any,
     ):
         self.__validate__(value)
         self._value = value
 
     def __repr__(self) -> str:
-        return self._value.__repr__()
+        return f"{self.__class__.__name__}({self._value.__repr__()})"
 
     def __str__(self) -> str:
         return str(self._value)
 
     @classmethod
     def nullable(
         cls,
@@ -209,14 +224,15 @@
             return cls.symbolic(
                 name=value._name,
                 key=value._key,
                 attribute=value._attribute,
                 owner=value._owner,
             )
         elif cls.supports(value):
+            #
             return cls(value=value)
         raise TypeError(
             f"{cls.__name__} does not support operations with value '{value}' of type '{type(value).__name__}'."
         )
 
     @classmethod
     def __validate__(cls, value: typing.Any):
@@ -438,15 +454,15 @@
             lhs = self.encode_value()
             rhs = other.encode_value()
             if lhs is None:
                 return Bool(rhs is None)
             elif rhs is None:
                 return Bool(lhs is None)
             else:
-                return Bool(lhs == rhs)
+                return Bool(bool(lhs == rhs))
         return Eq(self, other)
 
     def __ne__(self, value: typing.Any) -> typing.Union["Bool", Ne]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             lhs = self.encode_value()
             rhs = other.encode_value()
@@ -1665,14 +1681,16 @@
                     Bool,
                     Integer,
                     Float,
                     String,
                 ),
             ):
                 encoding[k] = v.encode_value()
+            elif isinstance(v, (bool, int, float, str)):
+                encoding[k] = v
             else:
                 encoding[k] = v.to_dict()
         return encoding
 
     def __getitem__(self, __key: str):
         if self.is_symbolic:
             symbol = self.get_symbol()
@@ -1682,15 +1700,15 @@
                 attribute=None,
                 key=__key,
             )
         else:
             value = self.get_value()
             if not value:
                 raise KeyError(__key)
-            return value[__key]
+            return _convert_simple_variables_to_standard_types(value[__key])
 
     def __setitem__(self, __key: str, __value: typing.Any):
         if not isinstance(__value, Variable):
             obj = _get_type_by_value(__value)
             __value = obj(__value)
         self.get_value()[__key] = __value
```

### Comparing `valor_client-0.24.0/valor/type_checks.py` & `valor_client-0.25.0/valor/type_checks.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.24.0/valor/viz.py` & `valor_client-0.25.0/valor/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,23 +126,23 @@
         ]
     else:
         task_types = [task_type]
 
     # unpack raster annotations
     annotations: List[Annotation] = []
     for annotation in annotated_datum.annotations:
-        if annotation.task_type.get_value() in task_types:
+        if annotation.task_type in task_types:
             annotations.append(annotation)
 
     # unpack label values
     label_values = []
     for annotation in annotations:
         for label in annotation.labels:
-            if label.key.get_value() == label_key:
-                label_values.append(label.value.get_value())
+            if label.key == label_key:
+                label_values.append(label.value)
     if not label_values:
         raise RuntimeError(
             f"Annotation doesn't have a label with key `{label_key}`"
         )
 
     # assign label coloring
     unique_label_values = list(set(label_values))
@@ -251,15 +251,15 @@
 ) -> Image.Image:
     """Draw a detection on an image."""
     text = ", ".join(
         [f"{label.key}:{label.value}" for label in detection.labels]
     )
     box = detection.bounding_box
     polygon = detection.polygon
-    if polygon.get_value() is not None:
+    if polygon is not None:
         img = _draw_bounding_polygon_on_image(
             polygon,
             img,
             inplace=inplace,
             text=text,
         )
     elif box.get_value() is not None:
```

### Comparing `valor_client-0.24.0/valor_client.egg-info/PKG-INFO` & `valor_client-0.25.0/valor_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.24.0
+Version: 0.25.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.24.0/valor_client.egg-info/SOURCES.txt` & `valor_client-0.25.0/valor_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 pyproject.toml
 tox.ini
 unit-tests/conftest.py
 unit-tests/test_client.py
 unit-tests/test_types.py
+unit-tests/test_typing.py
 unit-tests/test_viz.py
 unit-tests/coretypes/test_core.py
 unit-tests/coretypes/test_evaluation.py
 unit-tests/coretypes/test_filtering.py
 unit-tests/schemas/test_evaluation_schemas.py
 unit-tests/schemas/test_filters.py
 unit-tests/schemas/test_geojson.py
```

