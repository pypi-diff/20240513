# Comparing `tmp/hmt-basemodels-1.0.0.tar.gz` & `tmp/hmt_basemodels-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmt-basemodels-1.0.0.tar", last modified: Wed May  1 14:58:49 2024, max compression
+gzip compressed data, was "hmt_basemodels-1.1.0.tar", last modified: Mon May 13 11:11:48 2024, max compression
```

## Comparing `hmt-basemodels-1.0.0.tar` & `hmt_basemodels-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.793386 hmt-basemodels-1.0.0/
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     1071 2023-10-31 09:29:49.000000 hmt-basemodels-1.0.0/LICENSE
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)       18 2023-10-31 09:29:49.000000 hmt-basemodels-1.0.0/MANIFEST.in
--rw-r--r--   0 alidzm    (1000) alidzm    (1000)      467 2024-05-01 14:58:49.793386 hmt-basemodels-1.0.0/PKG-INFO
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     2155 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/README.md
-drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.789386 hmt-basemodels-1.0.0/basemodels/
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      445 2023-10-31 09:29:49.000000 hmt-basemodels-1.0.0/basemodels/__init__.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     1505 2024-04-17 08:57:12.000000 hmt-basemodels-1.0.0/basemodels/constants.py
-drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.789386 hmt-basemodels-1.0.0/basemodels/manifest/
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      172 2023-10-31 09:29:49.000000 hmt-basemodels-1.0.0/basemodels/manifest/__init__.py
-drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.789386 hmt-basemodels-1.0.0/basemodels/manifest/data/
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      327 2023-10-31 09:29:49.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/__init__.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     4706 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/groundtruth.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      595 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/helpers.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      479 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/preprocess.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      982 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/requester_question_example.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     1329 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/requester_restricted_answer_set.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     3338 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/taskdata.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)    19300 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/manifest.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     3031 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/restricted_audience.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     1695 2024-04-17 08:57:12.000000 hmt-basemodels-1.0.0/basemodels/via.py
-drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.793386 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/
--rw-r--r--   0 alidzm    (1000) alidzm    (1000)      467 2024-05-01 14:58:49.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/PKG-INFO
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      846 2024-05-01 14:58:49.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)        1 2024-05-01 14:58:49.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)       46 2024-05-01 14:58:49.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/requires.txt
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)       11 2024-05-01 14:58:49.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/top_level.txt
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)        1 2024-04-24 07:32:50.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/zip-safe
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      462 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/pyproject.toml
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)       38 2024-05-01 14:58:49.793386 hmt-basemodels-1.0.0/setup.cfg
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      604 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/setup.py
-drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.793386 hmt-basemodels-1.0.0/tests/
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)    39004 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/tests/test_manifest_validation.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     1181 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/tests/test_preprocess.py
--rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     3188 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/tests/test_restricted_answer_set.py
+drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-05-13 11:11:48.537924 hmt_basemodels-1.1.0/
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     1071 2024-01-29 14:58:22.000000 hmt_basemodels-1.1.0/LICENSE
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)       18 2024-01-29 14:58:22.000000 hmt_basemodels-1.1.0/MANIFEST.in
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      467 2024-05-13 11:11:48.537689 hmt_basemodels-1.1.0/PKG-INFO
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     2155 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/README.md
+drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-05-13 11:11:48.533964 hmt_basemodels-1.1.0/basemodels/
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      475 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/basemodels/__init__.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     1505 2024-03-21 13:40:44.000000 hmt_basemodels-1.1.0/basemodels/constants.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      500 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/basemodels/helpers.py
+drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-05-13 11:11:48.534901 hmt_basemodels-1.1.0/basemodels/manifest/
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      202 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/basemodels/manifest/__init__.py
+drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-05-13 11:11:48.535950 hmt_basemodels-1.1.0/basemodels/manifest/data/
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      327 2024-01-29 14:58:22.000000 hmt_basemodels-1.1.0/basemodels/manifest/data/__init__.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     4903 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/basemodels/manifest/data/groundtruth.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      664 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/basemodels/manifest/data/helpers.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      479 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/basemodels/manifest/data/preprocess.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     1098 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/basemodels/manifest/data/requester_question_example.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     1425 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/basemodels/manifest/data/requester_restricted_answer_set.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     3498 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/basemodels/manifest/data/taskdata.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)    21764 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/basemodels/manifest/manifest.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     3031 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/basemodels/manifest/restricted_audience.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     1695 2024-01-29 14:58:22.000000 hmt_basemodels-1.1.0/basemodels/via.py
+drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-05-13 11:11:48.537430 hmt_basemodels-1.1.0/hmt_basemodels.egg-info/
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      467 2024-05-13 11:11:48.000000 hmt_basemodels-1.1.0/hmt_basemodels.egg-info/PKG-INFO
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      868 2024-05-13 11:11:48.000000 hmt_basemodels-1.1.0/hmt_basemodels.egg-info/SOURCES.txt
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)        1 2024-05-13 11:11:48.000000 hmt_basemodels-1.1.0/hmt_basemodels.egg-info/dependency_links.txt
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)       46 2024-05-13 11:11:48.000000 hmt_basemodels-1.1.0/hmt_basemodels.egg-info/requires.txt
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)       11 2024-05-13 11:11:48.000000 hmt_basemodels-1.1.0/hmt_basemodels.egg-info/top_level.txt
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)        1 2024-05-13 11:11:48.000000 hmt_basemodels-1.1.0/hmt_basemodels.egg-info/zip-safe
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      462 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/pyproject.toml
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)       38 2024-05-13 11:11:48.537973 hmt_basemodels-1.1.0/setup.cfg
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      604 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/setup.py
+drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-05-13 11:11:48.537121 hmt_basemodels-1.1.0/tests/
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)    40881 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/tests/test_manifest_validation.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     1181 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/tests/test_preprocess.py
+-rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     3188 2024-05-13 11:11:07.000000 hmt_basemodels-1.1.0/tests/test_restricted_answer_set.py
```

### Comparing `hmt-basemodels-1.0.0/LICENSE` & `hmt_basemodels-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-1.0.0/README.md` & `hmt_basemodels-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-1.0.0/basemodels/constants.py` & `hmt_basemodels-1.1.0/basemodels/constants.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-1.0.0/basemodels/manifest/data/groundtruth.py` & `hmt_basemodels-1.1.0/basemodels/manifest/data/groundtruth.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import List, Optional, Union
 from uuid import UUID
 
 import requests
-from pydantic import BaseModel, HttpUrl, ValidationError, ConfigDict
+from pydantic import BaseModel, HttpUrl, ConfigDict
 from requests import RequestException
 from typing_extensions import Literal
 
 from basemodels.constants import SUPPORTED_CONTENT_TYPES, BaseJobTypesEnum
+from basemodels.helpers import raise_validation_error
 
 
 def create_wrapper_model(type):
     class WrapperModel(BaseModel):
         model_config = ConfigDict(arbitrary_types_allowed=True)
         data: Optional[type] = None
 
@@ -138,21 +139,26 @@
 
 def validate_content_type(uri: str) -> None:
     """Validate uri content type"""
     try:
         response = requests.head(uri, timeout=(3.5, 5))
         response.raise_for_status()
     except RequestException as e:
-        raise ValidationError(f"groundtruth content type ({uri}) validation failed", GroundtruthEntryKeyModel()) from e
+        raise_validation_error(
+            location=("groundtruth_uri",),
+            error_message=f"groundtruth content type ({uri}) validation failed",
+            input_data={"groundtruth_uri": uri}
+        )
 
     content_type = response.headers.get("Content-Type", "")
     if content_type not in SUPPORTED_CONTENT_TYPES:
-        raise ValidationError(
-            f"groundtruth entry has unsupported type {content_type}",
-            GroundtruthEntryKeyModel(),
+        raise_validation_error(
+            location=("groundtruth_uri",),
+            error_message=f"groundtruth entry has unsupported type {content_type}",
+            input_data={"groundtruth_uri": uri}
         )
 
 
 def validate_groundtruth_entry(
     key: str,
     value: Union[dict, list],
     request_type: str,
```

### Comparing `hmt-basemodels-1.0.0/basemodels/manifest/data/helpers.py` & `hmt_basemodels-1.1.0/basemodels/manifest/data/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import requests
-from pydantic import ValidationError, BaseModel, HttpUrl
+from pydantic import BaseModel, HttpUrl
 
 from basemodels.constants import SUPPORTED_CONTENT_TYPES
+from basemodels.helpers import raise_validation_error
 
 
 class ExampleResourceModel(BaseModel):
     answer_example_uri: HttpUrl
 
 
 def validate_content_type(uri: str) -> None:
     """Validate uri content type"""
     response = requests.head(uri, timeout=(3.5, 5))
     response.raise_for_status()
     content_type = response.headers.get("Content-Type", "")
     if content_type not in SUPPORTED_CONTENT_TYPES:
-        raise ValidationError(f"Unsupported type {content_type}", "answer_example_uri", ExampleResourceModel())
+        raise_validation_error(
+            location=("taskdata_uri",),
+            error_message=f"Unsupported type {content_type}",
+        )
```

### Comparing `hmt-basemodels-1.0.0/basemodels/manifest/data/requester_restricted_answer_set.py` & `hmt_basemodels-1.1.0/basemodels/manifest/data/requester_restricted_answer_set.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from requests import RequestException
-from pydantic.v1 import ValidationError
-from .helpers import validate_content_type, ExampleResourceModel
+from pydantic import ValidationError
+from .helpers import validate_content_type
+from basemodels.helpers import raise_validation_error
 
 
 def extract_answer_uri(restricted_answer_set: dict) -> list:
     """Extract the answer_uri from the answer set"""
     answer_uris = []
     for _, value in restricted_answer_set.items():
         if isinstance(value, dict) and value.get("answer_example_uri"):
@@ -18,16 +19,16 @@
     if not isinstance(restricted_answer_set, dict):
         raise ValueError("Requester restricted set should be a dict")
     uris = extract_answer_uri(restricted_answer_set)
     for uri in uris:
         try:
             validate_content_type(uri)
         except RequestException as e:
-            raise ValidationError(
-                f"could not retrieve requester restricted answer set example uri ({uri})",
-                ExampleResourceModel()
-            ) from e
+            raise_validation_error(
+                location=("requester_restricted_answer_set",),
+                error_message=f"could not retrieve requester restricted answer set example uri ({uri})",
+            )
         except ValidationError as e:
-            raise ValidationError(
-                f"requester restricted answer set example uri({uri}) content type failed validation",
-                ExampleResourceModel()
-            ) from e
+            raise_validation_error(
+                location=("requester_restricted_answer_set",),
+                error_message=f"requester restricted answer set uri({uri}) content type failed validation: {e.title}",
+            )
```

### Comparing `hmt-basemodels-1.0.0/basemodels/manifest/data/taskdata.py` & `hmt_basemodels-1.1.0/basemodels/manifest/data/taskdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Dict, Optional, Union, Any, List, Tuple
 from uuid import UUID
 
 import requests
-from pydantic import BaseModel, AnyHttpUrl, HttpUrl, ValidationError, field_validator, model_validator
-from pydantic_core.core_schema import ValidationInfo
+from pydantic import BaseModel, AnyHttpUrl, HttpUrl, field_validator, model_validator
 from requests import RequestException
 
 from basemodels.constants import SUPPORTED_CONTENT_TYPES
+from basemodels.helpers import raise_validation_error
 
 
 class Entity(BaseModel):
     """Entity configuration"""
 
     entity_id: UUID
     entity_uri: AnyHttpUrl
@@ -80,23 +80,31 @@
 
 def validate_content_type(uri: str) -> None:
     """Validate uri content type"""
     try:
         response = requests.head(uri, timeout=(3.5, 5))
         response.raise_for_status()
     except RequestException as e:
-        raise ValidationError(f"taskdata content type ({uri}) validation failed", TaskDataEntry()) from e
+        raise_validation_error(
+            location=("taskdata_uri",),
+            error_message=f"taskdata content type ({uri}) validation failed",
+        )
 
     content_type = response.headers.get("Content-Type", "")
     if content_type not in SUPPORTED_CONTENT_TYPES:
-        raise ValidationError(f"taskdata entry datapoint_uri has unsupported type {content_type}", TaskDataEntry())
+        raise_validation_error(
+            location=("taskdata_uri",),
+            error_message=f"taskdata entry datapoint_uri has unsupported type {content_type}",
+        )
 
 
 def validate_taskdata_entry(value: dict, validate_image_content_type: bool) -> None:
     """Validate taskdata entry"""
     if not isinstance(value, dict):
-        raise ValidationError("taskdata entry should be dict", TaskDataEntry())
-
+        raise_validation_error(
+            location=("taskdata_uri",),
+            error_message=f"taskdata entry should be dict",
+        )
     task_data = TaskDataEntry(**value)
 
     if validate_image_content_type:
         validate_content_type(task_data.datapoint_uri)
```

### Comparing `hmt-basemodels-1.0.0/basemodels/manifest/manifest.py` & `hmt_basemodels-1.1.0/basemodels/manifest/manifest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import json
 import uuid
 from datetime import datetime
 
 import requests
+from pydantic_core import InitErrorDetails
 from pydantic_core.core_schema import ValidationInfo
 from requests.exceptions import RequestException
 from typing_extensions import Literal
 from typing import Any, Dict, List, Optional, Union
 from enum import Enum
 from uuid import UUID, uuid4
 from .data.groundtruth import validate_groundtruth_entry
 from .data.requester_question_example import validate_requester_example_image
 from .data.requester_restricted_answer_set import validate_requester_restricted_answer_set_uris
 from .data.taskdata import validate_taskdata_entry, Entity
 from pydantic import BaseModel, field_validator, ValidationError, HttpUrl, AnyHttpUrl, model_validator, ConfigDict
 from pydantic.fields import Field
-from decimal import Decimal
 from basemodels.manifest.restricted_audience import RestrictedAudience
 from basemodels.constants import JOB_TYPES_FOR_CONTENT_TYPE_VALIDATION, BaseJobTypesEnum
+from basemodels.helpers import raise_validation_error
 
 
 # A validator function for UUID fields
 def validate_uuid(cls, value):
     return value or uuid.uuid4()
 
 
@@ -407,75 +408,146 @@
     """
     request_type = manifest.get("request_type", "")
     validate_image_content_type = request_type in JOB_TYPES_FOR_CONTENT_TYPE_VALIDATION
     uri_key = "groundtruth_uri"
     uri = manifest.get(uri_key)
     if uri is None:
         return
+    entries_count = 0
     try:
         response = requests.get(uri, timeout=(3.5, 5))
         response.raise_for_status()
-
-        entries_count = 0
         data = response.json()
         if isinstance(data, dict):
             for k, v in data.items():
                 entries_count += 1
                 validate_groundtruth_entry(k, v, request_type, validate_image_content_type)
                 validate_image_content_type = False
         else:
             for v in data:
                 entries_count += 1
                 validate_groundtruth_entry("", v, request_type, validate_image_content_type)
                 validate_image_content_type = False
 
-    except (ValidationError, RequestException) as e:
-        raise ValidationError(f"Validation failed for {uri}: {e}", TaskData()) from e
+    except ValidationError as e:
+        raise_validation_error(
+            location=("groundtruth_uri",),
+            error_message=f"Validation failed for {uri}: {e.title}",
+            input_data={"groundtruth_uri": uri}
+        )
+    except RequestException as e:
+        raise_validation_error(
+            location=("groundtruth_uri",),
+            error_message=f"Validation failed for {uri}: {e}",
+            input_data={"groundtruth_uri": uri}
+        )
 
     if entries_count == 0:
-        raise ValidationError(f"fetched {uri} is empty", TaskData())
+        raise_validation_error(
+            location=("groundtruth_uri",),
+            error_message=f"fetched {uri} is empty"f"fetched {uri} is empty",
+            input_data={"groundtruth_uri": uri}
+        )
 
 
 def validate_taskdata_uri(manifest: dict):
     """
     Validate taskdata_uri
     Returns entries count if succeeded
     """
     request_type = manifest.get("request_type", "")
     validate_image_content_type = request_type in JOB_TYPES_FOR_CONTENT_TYPE_VALIDATION
     uri_key = "taskdata_uri"
     uri = manifest.get(uri_key)
     if uri is None:
         return
+    entries_count = 0
     try:
         response = requests.get(uri, timeout=(3.5, 5))
         response.raise_for_status()
-
-        entries_count = 0
         data = response.json()
         for v in data:
             entries_count += 1
             validate_taskdata_entry(v, validate_image_content_type)
             validate_image_content_type = False  # We want to validate only first entry for content type
 
-    except (ValidationError, RequestException) as e:
-        raise ValidationError(f"Validation failed for {uri}: {e}", TaskData())
+    except ValidationError as e:
+        raise_validation_error(
+            location=("taskdata_uri",),
+            error_message=f"Validation failed for {uri}: {e.title}",
+            input_data={"taskdata_uri": uri}
+        )
+    except RequestException as e:
+        raise_validation_error(
+            location=("taskdata_uri",),
+            error_message=f"Validation failed for {uri}: {e}",
+            input_data={"taskdata_uri": uri}
+        )
 
     if entries_count == 0:
-        raise ValidationError(f"fetched {uri} is empty"f"fetched {uri} is empty", TaskData())
+        raise_validation_error(
+            location=("taskdata_uri",),
+            error_message=f"fetched {uri} is empty"f"fetched {uri} is empty",
+            input_data={"taskdata_uri": uri}
+        )
 
 
 def validate_manifest_example_images(manifest: dict):
     """Fetch and validate the example resources."""
     question_example = manifest.get("requester_question_example")
     req_res_answer_set = manifest.get("requester_restricted_answer_set", {})
     if question_example:
         # some jobs might not have requester_question_example
         validate_requester_example_image(question_example)
     if req_res_answer_set:
         validate_requester_restricted_answer_set_uris(req_res_answer_set)
 
 
+def fetch_data_from_uri(data_uri: str):
+    """Fetch data from a given uri."""
+    try:
+        response = requests.get(data_uri, timeout=(3.5, 5))
+        response.raise_for_status()
+        return response.json()
+    except RequestException as e:
+        raise_validation_error(
+            location=("taskdata_uri", "groundtruth_uri",),
+            error_message=f"Failed to fetch data from {data_uri}: {e}"
+        )
+
+
 def validate_manifest_uris(manifest: dict):
     """Fetch & validate manifest's remote objects"""
     validate_taskdata_uri(manifest)
     validate_groundtruth_uri(manifest)
+
+
+def validate_is_verification(manifest: dict):
+    """Check for verification jobs."""
+
+    request_type = manifest.get("request_type")
+    if request_type == BaseJobTypesEnum.image_drag_drop:
+        task_key = "task_key"
+    else:
+        task_key = "datapoint_uri"
+
+    taskdata_uri = manifest.get("taskdata_uri")
+    gt_uri = manifest.get("groundtruth_uri")
+
+    if not gt_uri or not taskdata_uri:
+        raise_validation_error(
+            location=("taskdata_uri", "groundtruth_uri",),
+            error_message="Manifest is missing either of groundtruth or taskdata"
+        )
+
+    taskdata = fetch_data_from_uri(taskdata_uri)
+    groundtruth = fetch_data_from_uri(gt_uri)
+
+    task_keys = {task.get(task_key) for task in taskdata}
+    gt_keys = set(groundtruth.keys())
+
+    if gt_keys != task_keys:
+        raise_validation_error(
+            location=("taskdata_uri", "groundtruth_uri",),
+            error_message="All taskdata entries dont have corresponding groundtruth entry",
+            input_data={"taskdata_uri": taskdata_uri, "groundtruth_uri": gt_uri}
+        )
```

### Comparing `hmt-basemodels-1.0.0/basemodels/manifest/restricted_audience.py` & `hmt_basemodels-1.1.0/basemodels/manifest/restricted_audience.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-1.0.0/basemodels/via.py` & `hmt_basemodels-1.1.0/basemodels/via.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-1.0.0/hmt_basemodels.egg-info/SOURCES.txt` & `hmt_basemodels-1.1.0/hmt_basemodels.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 basemodels/__init__.py
 basemodels/constants.py
+basemodels/helpers.py
 basemodels/via.py
 basemodels/manifest/__init__.py
 basemodels/manifest/manifest.py
 basemodels/manifest/restricted_audience.py
 basemodels/manifest/data/__init__.py
 basemodels/manifest/data/groundtruth.py
 basemodels/manifest/data/helpers.py
```

### Comparing `hmt-basemodels-1.0.0/setup.py` & `hmt_basemodels-1.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="hmt-basemodels",
-    version="1.0.0",
+    version="1.1.0",
     author="HUMAN Protocol",
     description="Common data models shared by various components of the Human Protocol stack",
     url="https://github.com/hCaptcha/hmt-basemodels",
     include_package_data=True,
     zip_safe=True,
     classifiers=[
         "Intended Audience :: Developers",
```

### Comparing `hmt-basemodels-1.0.0/tests/test_manifest_validation.py` & `hmt_basemodels-1.1.0/tests/test_manifest_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -893,48 +893,69 @@
         body = [{"task_key": "not_uuid", "datapoint_uri": "not_uri"}]
 
         self.register_http_response(uri, manifest, body)
 
         with self.assertRaises(ValidationError):
             test_models.validate_manifest_uris(manifest)
 
-    def test_groundtruth_and_taskdata_valid(self):
+    def mock_manifest_uris(self, verification: bool = False, gt_td_same_length: bool = False):
+        """Mocking manifest uris."""
         taskdata_uri = "https://td.com"
         groundtruth_uri = "https://gt.com"
         manifest = {
             "taskdata_uri": taskdata_uri,
             "groundtruth_uri": groundtruth_uri,
             "request_type": "image_label_binary",
         }
-        datapoint_uri = "https://domain.com/file1.jpg"
+        if verification:
+            image_uri_1 = gt_uri_1 = "https://domain.com/123/file1.jpeg"
+            image_uri_2 = gt_uri_2 = "https://domain.com/456/file2.jpeg"
+        else:
+            image_uri_1 = "https://domain.com/123/file1.jpeg"
+            gt_uri_1 = "https://domain.com/file1.jpeg"
+            image_uri_2 = "https://domain.com/456/file2.jpeg"
+            gt_uri_2 = "https://domain.com/file2.jpeg"
+
         taskdata = [
             {
                 "task_key": "407fdd93-687a-46bb-b578-89eb96b4109d",
-                "datapoint_uri": datapoint_uri,
+                "datapoint_uri": image_uri_1,
                 "datapoint_hash": "f4acbe8562907183a484498ba901bfe5c5503aaa",
             },
             {
                 "task_key": "20bd4f3e-4518-4602-b67a-1d8dfabcce0c",
-                "datapoint_uri": "https://domain.com/file2.jpg",
+                "datapoint_uri": image_uri_2,
+                "datapoint_hash": "f4acbe8562907183a484498ba901bfe5c5503aaa",
+            },
+            # task with duplicated datapoint_uri
+            {
+                "task_key": "30bd4f3e-4518-4602-b67a-1d8dfabcce0a",
+                "datapoint_uri": image_uri_2,
                 "datapoint_hash": "f4acbe8562907183a484498ba901bfe5c5503aaa",
             },
         ]
-        groundtruth_image_uri = "https://domain.com/123/file1.jpeg"
         groundtruth = {
-            groundtruth_image_uri: ["false", "false", "false"],
-            "https://domain.com/456/file2.jpeg": ["false", "true", "false"],
+            gt_uri_1: ["false", "false", "false"],
         }
+        if gt_td_same_length:
+            groundtruth[gt_uri_2] = ["false", "true", "false"]
 
-        self.register_http_response(datapoint_uri, method=httpretty.HEAD, headers={"Content-Type": "image/jpeg"})
         self.register_http_response(
-            groundtruth_image_uri, method=httpretty.HEAD, headers={"Content-Type": "image/jpeg"}
+            image_uri_1, method=httpretty.HEAD, headers={"Content-Type": "image/jpeg"}
+        )
+        self.register_http_response(
+            gt_uri_1, method=httpretty.HEAD, headers={"Content-Type": "image/jpeg"}
         )
         self.register_http_response(taskdata_uri, manifest, taskdata)
         self.register_http_response(groundtruth_uri, manifest, groundtruth)
 
+        return manifest
+
+    def test_groundtruth_and_taskdata_valid(self):
+        manifest = self.mock_manifest_uris(gt_td_same_length=True)
         test_models.validate_manifest_uris(manifest)
 
     def test_mitl_in_internal_config(self):
         """Test that mitl config can be part of the internal configuration"""
         model = a_manifest().to_primitive()
         mitl_config = {
             "n_gt": 200,
@@ -991,14 +1012,35 @@
         }
         self.register_http_response(first_uri, method=httpretty.HEAD, headers={"Content-Type": "image/html"})
         self.register_http_response(second_uri, method=httpretty.HEAD, headers={"Content-Type": "image/html"})
         self.register_http_response(third_uri, method=httpretty.HEAD, headers={"Content-Type": "image/jpeg"})
         with self.assertRaises(ValidationError):
             test_models.validate_manifest_example_images(manifest)
 
+    def test_valid_is_verification(self):
+        """Test valid is verification."""
+        manifest = self.mock_manifest_uris(verification=True, gt_td_same_length=True)
+        test_models.validate_is_verification(manifest)
+
+    def test_invalid_is_verification(self):
+        """Test validation of invalid is verification."""
+        # check when it is not verification but with gt and td not same length
+        manifest = self.mock_manifest_uris(verification=True)
+        with self.assertRaises(ValidationError) as val_error:
+            test_models.validate_is_verification(manifest)
+
+        self.assertEqual("All taskdata entries dont have corresponding groundtruth entry", val_error.exception.title)
+
+        # check when it is not verification but with the gt and TD same length
+        manifest = self.mock_manifest_uris(gt_td_same_length=True)
+        with self.assertRaises(ValidationError) as val_error:
+            test_models.validate_is_verification(manifest)
+
+        self.assertEqual("All taskdata entries dont have corresponding groundtruth entry", val_error.exception.title)
+
 
 class TaskEntryTest(unittest.TestCase):
     def test_valid_entry_is_true(self):
         taskdata = deepcopy(TASK)
         TaskDataEntry(**taskdata)
 
         taskdata.get("metadata")["key_1"] = None
```

### Comparing `hmt-basemodels-1.0.0/tests/test_preprocess.py` & `hmt_basemodels-1.1.0/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-1.0.0/tests/test_restricted_answer_set.py` & `hmt_basemodels-1.1.0/tests/test_restricted_answer_set.py`

 * *Files identical despite different names*

