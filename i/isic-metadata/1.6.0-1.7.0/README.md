# Comparing `tmp/isic_metadata-1.6.0.tar.gz` & `tmp/isic_metadata-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic_metadata-1.6.0.tar", last modified: Wed May  1 17:49:57 2024, max compression
+gzip compressed data, was "isic_metadata-1.7.0.tar", last modified: Mon May 13 20:43:41 2024, max compression
```

## Comparing `isic_metadata-1.6.0.tar` & `isic_metadata-1.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.782658 isic_metadata-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.774659 isic_metadata-1.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.778658 isic_metadata-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-01 17:49:57.782658 isic_metadata-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.778658 isic_metadata-1.6.0/isic_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/isic_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/isic_metadata/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/isic_metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/isic_metadata/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/isic_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.782658 isic_metadata-1.6.0/isic_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-01 17:49:57.000000 isic_metadata-1.6.0/isic_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-01 17:49:57.000000 isic_metadata-1.6.0/isic_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:49:57.000000 isic_metadata-1.6.0/isic_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 17:49:57.000000 isic_metadata-1.6.0/isic_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 17:49:57.000000 isic_metadata-1.6.0/isic_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:49:57.782658 isic_metadata-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.782658 isic_metadata-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tests/test_dependent_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.601458 isic_metadata-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.593458 isic_metadata-1.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.597458 isic_metadata-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 20:43:41.601458 isic_metadata-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.597458 isic_metadata-1.7.0/isic_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/isic_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/isic_metadata/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/isic_metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/isic_metadata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/isic_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.601458 isic_metadata-1.7.0/isic_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 20:43:41.000000 isic_metadata-1.7.0/isic_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-13 20:43:41.000000 isic_metadata-1.7.0/isic_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:43:41.000000 isic_metadata-1.7.0/isic_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 20:43:41.000000 isic_metadata-1.7.0/isic_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 20:43:41.000000 isic_metadata-1.7.0/isic_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:43:41.601458 isic_metadata-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.601458 isic_metadata-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tests/test_dependent_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tox.ini
```

### Comparing `isic_metadata-1.6.0/.github/workflows/ci.yml` & `isic_metadata-1.7.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.6.0/.github/workflows/release.yml` & `isic_metadata-1.7.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.6.0/.gitignore` & `isic_metadata-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.6.0/LICENSE` & `isic_metadata-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.6.0/PKG-INFO` & `isic_metadata-1.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 1.6.0
+Version: 1.7.0
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic_metadata-1.6.0/isic_metadata/__init__.py` & `isic_metadata-1.7.0/isic_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.6.0/isic_metadata/fields.py` & `isic_metadata-1.7.0/isic_metadata/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 
 class ImageTypeEnum(str, Enum):
     dermoscopic = "dermoscopic"
     clinical_overview = "clinical: overview"
     clinical_close_up = "clinical: close-up"
     tbp_tile_close_up = "TBP tile: close-up"
     tbp_tile_overview = "TBP tile: overview"
+    rcm_macroscopic = "RCM: macroscopic"
 
 
 class DermoscopicTypeEnum(str, Enum):
     contact_polarized = "contact polarized"
     contact_non_polarized = "contact non-polarized"
     non_contact_polarized = "non-contact polarized"
```

### Comparing `isic_metadata-1.6.0/isic_metadata/metadata.py` & `isic_metadata-1.7.0/isic_metadata/metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -129,14 +129,36 @@
                 "one_lesion_multiple_patients",
                 "One or more lesions belong to multiple patients.",
                 {"examples": bad_lesions[:5]},
             )
 
         return self
 
+    @model_validator(mode="after")
+    def check_rcm_at_most_one_macroscopic_image(self) -> MetadataBatch:
+        rcm_case_to_macroscopic: dict[str, int] = defaultdict(int)
+
+        for item in self.items:
+            if item.rcm_case_id and item.image_type == ImageTypeEnum.rcm_macroscopic:
+                rcm_case_to_macroscopic[item.rcm_case_id] += 1
+
+        bad_rcm_cases = [
+            rcm_case
+            for rcm_case in rcm_case_to_macroscopic
+            if rcm_case_to_macroscopic[rcm_case] > 1
+        ]
+        if bad_rcm_cases:
+            raise PydanticCustomError(
+                "rcm_multiple_macroscopics",
+                "One or more RCM cases have multiple macroscopic images.",
+                {"examples": bad_rcm_cases[:5]},
+            )
+
+        return self
+
 
 class MetadataRow(BaseModel):
     model_config = ConfigDict(
         arbitrary_types_allowed=True,
         # This is useful for patient/lesion id fields, which could be numeric
         coerce_numbers_to_str=True,
         # extra values should be gathered by build_extra, so there's no need to allow them here
@@ -174,14 +196,16 @@
     acquisition_day: int | None = None
 
     nevus_type: NevusTypeEnum | None = None
     image_type: ImageTypeEnum | None = None
     dermoscopic_type: DermoscopicTypeEnum | None = None
     tbp_tile_type: TBPTileTypeEnum | None = None
 
+    rcm_case_id: str | None = None
+
     unstructured: dict[str, Any] = {}
 
     # Unused and undocumented
     marker_pen: bool | None = None
     hairy: bool | None = None
     blurry: bool | None = None
     color_tint: ColorTintEnum | None = None
@@ -285,14 +309,29 @@
                 raise error_incompatible_fields(
                     field, "diagnosis", field2_value=self.diagnosis.value
                 )
 
         return self
 
     @model_validator(mode="after")
+    def validate_rcm_fields(self) -> MetadataRow:
+        if not self.rcm_case_id:
+            return self
+
+        if not self.image_type:
+            raise error_missing_field("rcm_case_id", "image_type")
+
+        if self.image_type != ImageTypeEnum.rcm_macroscopic:
+            raise error_incompatible_fields(
+                "rcm_case_id", "image_type", field2_value=ImageTypeEnum.rcm_macroscopic
+            )
+
+        return self
+
+    @model_validator(mode="after")
     def validate_dermoscopic_fields(self) -> MetadataRow:
         if not self.dermoscopic_type:
             return self
 
         if not self.image_type:
             raise error_missing_field("dermoscopic_type", "image_type")
```

### Comparing `isic_metadata-1.6.0/isic_metadata.egg-info/PKG-INFO` & `isic_metadata-1.7.0/isic_metadata.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 1.6.0
+Version: 1.7.0
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic_metadata-1.6.0/isic_metadata.egg-info/SOURCES.txt` & `isic_metadata-1.7.0/isic_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.6.0/pyproject.toml` & `isic_metadata-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.6.0/setup.py` & `isic_metadata-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.6.0/tests/test_dependent_fields.py` & `isic_metadata-1.7.0/tests/test_dependent_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,23 @@
         MetadataRow.model_validate(
             {"dermoscopic_type": "contact polarized", "image_type": "clinical: overview"}
         )
     assert len(excinfo.value.errors()) == 1
     assert "dermoscopic_type is incompatible with image_type" in excinfo.value.errors()[0]["msg"]
 
 
+def test_rcm_case_id_requires_rcm_image_type():
+    with pytest.raises(ValidationError) as excinfo:
+        MetadataRow.model_validate({"rcm_case_id": "12345"})
+    assert len(excinfo.value.errors()) == 1
+    assert "rcm_case_id requires setting image_type" in excinfo.value.errors()[0]["msg"]
+
+    MetadataRow.model_validate({"rcm_case_id": "12345", "image_type": "RCM: macroscopic"})
+
+
 def test_tbp_tile_type_requires_image_type_tbp_tile():
     with pytest.raises(ValidationError) as excinfo:
         MetadataRow.model_validate({"tbp_tile_type": "2D"})
     assert len(excinfo.value.errors()) == 1
     assert "tbp_tile_type requires setting image_type" in excinfo.value.errors()[0]["msg"]
 
     MetadataRow.model_validate({"tbp_tile_type": "2D", "image_type": "TBP tile: close-up"})
```

### Comparing `isic_metadata-1.6.0/tests/test_fields.py` & `isic_metadata-1.7.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.6.0/tox.ini` & `isic_metadata-1.7.0/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 deps =
     coverage[toml]
     hypothesis
     pytest
     pytest-mock
     pytest-cov
 commands =
-    pytest --cov-report=html --cov-branch --cov=isic_metadata tests
+    pytest --cov-report=html --cov-branch --cov=isic_metadata {posargs} tests
 
 [testenv:type]
 skipsdist = true
 skip_install = true
 deps =
     mypy
 commands =
```

