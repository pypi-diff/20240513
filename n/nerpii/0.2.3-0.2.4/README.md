# Comparing `tmp/nerpii-0.2.3.tar.gz` & `tmp/nerpii-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerpii-0.2.3.tar", max compression
+gzip compressed data, was "nerpii-0.2.4.tar", max compression
```

## Comparing `nerpii-0.2.3.tar` & `nerpii-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3336 2024-05-03 10:23:15.578353 nerpii-0.2.3/README.md
--rw-r--r--   0        0        0      209 2024-05-03 10:23:15.578353 nerpii-0.2.3/nerpii/__init__.py
--rw-r--r--   0        0        0    22243 2024-05-03 10:23:15.578353 nerpii-0.2.3/nerpii/faker_generator.py
--rw-r--r--   0        0        0    18421 2024-05-03 10:23:15.578353 nerpii-0.2.3/nerpii/named_entity_recognizer.py
--rw-r--r--   0        0        0      843 2024-05-03 10:23:15.582353 nerpii-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4301 1970-01-01 00:00:00.000000 nerpii-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     3336 2024-05-13 13:11:47.839423 nerpii-0.2.4/README.md
+-rw-r--r--   0        0        0      209 2024-05-13 13:11:47.839423 nerpii-0.2.4/nerpii/__init__.py
+-rw-r--r--   0        0        0    22243 2024-05-13 13:11:47.839423 nerpii-0.2.4/nerpii/faker_generator.py
+-rw-r--r--   0        0        0    18435 2024-05-13 13:11:47.843423 nerpii-0.2.4/nerpii/named_entity_recognizer.py
+-rw-r--r--   0        0        0      843 2024-05-13 13:11:47.843423 nerpii-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4301 1970-01-01 00:00:00.000000 nerpii-0.2.4/PKG-INFO
```

### Comparing `nerpii-0.2.3/README.md` & `nerpii-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nerpii-0.2.3/nerpii/faker_generator.py` & `nerpii-0.2.4/nerpii/faker_generator.py`

 * *Files identical despite different names*

### Comparing `nerpii-0.2.3/nerpii/named_entity_recognizer.py` & `nerpii-0.2.4/nerpii/named_entity_recognizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
 
     def __init__(
         self,
         df_input: Union[str, pd.DataFrame],
         data_sample: Optional[int] = 500,
         nan_filler: str = "?",
         lang: Optional[str] = "en",
-        get_gender: Optional[bool] = False,
+        get_gender_option: Optional[bool] = False,
     ) -> "NamedEntityRecognizer":
         """
         Create a NamedEntityRecognizer instance.
 
         Parameters
         ----------
         df_input : Union[str, pd.DataFrame]
@@ -306,15 +306,15 @@
         NamedEntityRecognizer
             A NamedEntityRecognizer instance.
         """
 
         if not isinstance(df_input, pd.DataFrame):
             df_input = pd.read_csv(df_input)
 
-        if get_gender == True:
+        if get_gender_option == True:
             df_input = get_gender(df_input)
 
         self.dataset = df_input.sample(n=min(data_sample, df_input.shape[0]))
         self.object_columns = list(self.dataset.select_dtypes(["object"]).columns)
         # fill NaN values for object columns
         self.dataset.loc[:, self.object_columns] = self.dataset.loc[
             :, self.object_columns
```

### Comparing `nerpii-0.2.3/pyproject.toml` & `nerpii-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nerpii"
-version = "0.2.3"
+version = "0.2.4"
 description = "A python library to perform NER on structured data and generate PII with Faker"
 authors = ["Clearbox AI <info@clearbox.ai>"]
 license = "GPL"
 readme = "README.md"
 homepage = "https://github.com/Clearbox-AI/nerpii"
 repository = "https://github.com/Clearbox-AI/nerpii"
 packages = [{include = "nerpii"}]
```

### Comparing `nerpii-0.2.3/PKG-INFO` & `nerpii-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerpii
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python library to perform NER on structured data and generate PII with Faker
 Home-page: https://github.com/Clearbox-AI/nerpii
 License: GPL
 Author: Clearbox AI
 Author-email: info@clearbox.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

