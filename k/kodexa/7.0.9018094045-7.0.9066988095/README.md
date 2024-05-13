# Comparing `tmp/kodexa-7.0.9018094045.tar.gz` & `tmp/kodexa-7.0.9066988095.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.9018094045.tar", max compression
+gzip compressed data, was "kodexa-7.0.9066988095.tar", max compression
```

## Comparing `kodexa-7.0.9018094045.tar` & `kodexa-7.0.9066988095.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2024-05-09 13:33:29.529817 kodexa-7.0.9018094045/LICENSE
--rw-r--r--   0        0        0     2178 2024-05-09 13:33:29.529817 kodexa-7.0.9018094045/README.md
--rw-r--r--   0        0        0      957 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/model/base.py
--rw-r--r--   0        0        0        0 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/model/entities/__init__.py
--rw-r--r--   0        0        0     3526 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/model/entities/product.py
--rw-r--r--   0        0        0     3810 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/model/entities/product_subscription.py
--rw-r--r--   0        0        0   115561 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/model/model.py
--rw-r--r--   0        0        0   174318 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/model/objects.py
--rw-r--r--   0        0        0    62032 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   218158 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    34024 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-05-09 13:33:29.537817 kodexa-7.0.9018094045/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 13:33:29.541817 kodexa-7.0.9018094045/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1389 2024-05-09 13:33:43.577948 kodexa-7.0.9018094045/pyproject.toml
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.9018094045/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 17:09:53.216595 kodexa-7.0.9066988095/LICENSE
+-rw-r--r--   0        0        0     2178 2024-05-13 17:09:53.216595 kodexa-7.0.9066988095/README.md
+-rw-r--r--   0        0        0      957 2024-05-13 17:09:53.220595 kodexa-7.0.9066988095/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-13 17:09:53.220595 kodexa-7.0.9066988095/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-05-13 17:09:53.220595 kodexa-7.0.9066988095/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-05-13 17:09:53.220595 kodexa-7.0.9066988095/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-05-13 17:09:53.220595 kodexa-7.0.9066988095/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-05-13 17:09:53.220595 kodexa-7.0.9066988095/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-05-13 17:09:53.220595 kodexa-7.0.9066988095/kodexa/model/base.py
+-rw-r--r--   0        0        0        0 2024-05-13 17:09:53.220595 kodexa-7.0.9066988095/kodexa/model/entities/__init__.py
+-rw-r--r--   0        0        0     3526 2024-05-13 17:09:53.220595 kodexa-7.0.9066988095/kodexa/model/entities/product.py
+-rw-r--r--   0        0        0     3810 2024-05-13 17:09:53.220595 kodexa-7.0.9066988095/kodexa/model/entities/product_subscription.py
+-rw-r--r--   0        0        0   115561 2024-05-13 17:09:53.220595 kodexa-7.0.9066988095/kodexa/model/model.py
+-rw-r--r--   0        0        0   174318 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/model/objects.py
+-rw-r--r--   0        0        0    62032 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   218157 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    34024 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 17:09:53.224595 kodexa-7.0.9066988095/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1389 2024-05-13 17:10:08.144878 kodexa-7.0.9066988095/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.9066988095/PKG-INFO
```

### Comparing `kodexa-7.0.9018094045/LICENSE` & `kodexa-7.0.9066988095/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/README.md` & `kodexa-7.0.9066988095/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/__init__.py` & `kodexa-7.0.9066988095/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/assistant/assistant.py` & `kodexa-7.0.9066988095/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/connectors/connectors.py` & `kodexa-7.0.9066988095/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/model/__init__.py` & `kodexa-7.0.9066988095/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/model/base.py` & `kodexa-7.0.9066988095/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/model/entities/product.py` & `kodexa-7.0.9066988095/kodexa/model/entities/product.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/model/entities/product_subscription.py` & `kodexa-7.0.9066988095/kodexa/model/entities/product_subscription.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/model/model.py` & `kodexa-7.0.9066988095/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/model/objects.py` & `kodexa-7.0.9066988095/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/model/persistence.py` & `kodexa-7.0.9066988095/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/pipeline/pipeline.py` & `kodexa-7.0.9066988095/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/platform/client.py` & `kodexa-7.0.9066988095/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2900,15 +2900,15 @@
 
         if sort is not None:
             params["sort"] = sort
 
         if self.organization is not None:
             params["filter"].append(f"organization.id: '{self.organization.id}'")
 
-        get_response = self.client.get(f"/api/{self.get_type()}/", params=params)
+        get_response = self.client.get(f"/api/{self.get_type()}", params=params)
 
         return PageProjectEndpoint.model_validate(get_response.json()).set_client(
             self.client
         )
 
     def create(self, project: Project, template_ref: str = None) -> Project:
         """
```

### Comparing `kodexa-7.0.9018094045/kodexa/platform/interaction.py` & `kodexa-7.0.9066988095/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/platform/kodexa.py` & `kodexa-7.0.9066988095/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/selectors/ast.py` & `kodexa-7.0.9066988095/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/selectors/core.py` & `kodexa-7.0.9066988095/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/selectors/lexrules.py` & `kodexa-7.0.9066988095/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/selectors/lextab.py` & `kodexa-7.0.9066988095/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/selectors/parserules.py` & `kodexa-7.0.9066988095/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/selectors/parsetab.py` & `kodexa-7.0.9066988095/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/spatial/azure_models.py` & `kodexa-7.0.9066988095/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/spatial/bbox_common.py` & `kodexa-7.0.9066988095/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/spatial/table_form_common.py` & `kodexa-7.0.9066988095/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/steps/common.py` & `kodexa-7.0.9066988095/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/testing/test_components.py` & `kodexa-7.0.9066988095/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/kodexa/testing/test_utils.py` & `kodexa-7.0.9066988095/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9018094045/pyproject.toml` & `kodexa-7.0.9066988095/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.09018094045"
+version = "7.0.09066988095"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.9018094045/PKG-INFO` & `kodexa-7.0.9066988095/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.9018094045
+Version: 7.0.9066988095
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

