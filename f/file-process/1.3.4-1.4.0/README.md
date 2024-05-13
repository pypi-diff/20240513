# Comparing `tmp/file_process-1.3.4.tar.gz` & `tmp/file_process-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_process-1.3.4.tar", last modified: Tue Apr 30 15:34:19 2024, max compression
+gzip compressed data, was "file_process-1.4.0.tar", last modified: Mon May 13 11:56:20 2024, max compression
```

## Comparing `file_process-1.3.4.tar` & `file_process-1.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:34:19.689818 file_process-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 15:34:17.000000 file_process-1.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-30 15:34:19.689818 file_process-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-30 15:34:17.000000 file_process-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:34:19.685818 file_process-1.3.4/file_process/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:34:19.689818 file_process-1.3.4/file_process/csv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/csv/csv_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/csv/csv_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/csv/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/file_processor_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:34:19.689818 file_process-1.3.4/file_process/h5ad/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/h5ad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/h5ad/h5ad_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/h5ad/h5ad_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/h5ad/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:34:19.689818 file_process-1.3.4/file_process/txt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/txt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-30 15:34:17.000000 file_process-1.3.4/file_process/txt/txt_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:34:19.689818 file_process-1.3.4/file_process.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-30 15:34:19.000000 file_process-1.3.4/file_process.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 15:34:19.000000 file_process-1.3.4/file_process.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:34:19.000000 file_process-1.3.4/file_process.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 15:34:19.000000 file_process-1.3.4/file_process.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 15:34:19.000000 file_process-1.3.4/file_process.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 15:34:19.689818 file_process-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-30 15:34:17.000000 file_process-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:56:20.675714 file_process-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 11:56:17.000000 file_process-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-13 11:56:20.675714 file_process-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-13 11:56:17.000000 file_process-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:56:20.671714 file_process-1.4.0/file_process/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:56:20.675714 file_process-1.4.0/file_process/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/csv/csv_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/csv/csv_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/csv/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/file_processor_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:56:20.675714 file_process-1.4.0/file_process/h5ad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/h5ad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/h5ad/h5ad_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/h5ad/h5ad_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/h5ad/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:56:20.675714 file_process-1.4.0/file_process/txt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/txt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-13 11:56:17.000000 file_process-1.4.0/file_process/txt/txt_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:56:20.675714 file_process-1.4.0/file_process.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-13 11:56:20.000000 file_process-1.4.0/file_process.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-13 11:56:20.000000 file_process-1.4.0/file_process.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:56:20.000000 file_process-1.4.0/file_process.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 11:56:20.000000 file_process-1.4.0/file_process.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 11:56:20.000000 file_process-1.4.0/file_process.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 11:56:20.675714 file_process-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-13 11:56:17.000000 file_process-1.4.0/setup.py
```

### Comparing `file_process-1.3.4/LICENSE.txt` & `file_process-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `file_process-1.3.4/README.md` & `file_process-1.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 ```
 from file_process import preview_file
 try:
     processor = FileProcessFactory.get(file_data.filename, file_data.file)
 except WrongExtension as exc:
     raise CustomException from exc
 processor.validate(model_metadata_file)
-target_names, var_preview, obs_preview = processor.get_preview()
+var_target_names, obs_target_names, obs_preview, var_preview, text_preview  = processor.get_preview()
 ```
 
 where:
 
 - file: an object of io.BytesIo or FileStorage which will be validated and previewed
 - filename: name of the validated file (only it's extention will be used)
 - model_metadata_file (optional parameter): file with metadata of a model that will be used for validation. If this file is provided, the code will check that this file has the same set of columns as the validated file. If this file is not provided, no validation will be applied.
 
-The code returns a list of targets (columns from the validated file), var preview and obs preview.
+The code returns a list of var targets and obs targets (columns from the validated file), var preview and obs preview and text preview.
 If some is not applicable for the file, None will be returned).
 
 How to release:
 
 1. Make your changes
 2. Change the version in setup.py
 3. Merge changes into the main branch; it will be automatically released to [pypi](https://pypi.org/project/file-process/#history)
```

### Comparing `file_process-1.3.4/file_process/csv/csv_processor.py` & `file_process-1.4.0/file_process/csv/csv_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     def get_var_names(self):
         return list(self.data_df.columns)
 
     def get_preview(self):
         var_names = self.get_var_names()
         obs_preview = self.get_observations(PREVIEW_ROWS_COUNT)
-        return var_names, self.create_tabular_response(obs_preview), None, None
+        return var_names, None, self.create_tabular_response(obs_preview), None, None
 
     @staticmethod
     def create_tabular_response(data_df: pd.DataFrame) -> List[dict]:
         if data_df is None:
             return []
         numeric_columns = data_df.select_dtypes(include=number).columns
         rows = data_df.replace({nan: None})
```

### Comparing `file_process-1.3.4/file_process/csv/csv_validator.py` & `file_process-1.4.0/file_process/csv/csv_validator.py`

 * *Files identical despite different names*

### Comparing `file_process-1.3.4/file_process/csv/schemas.py` & `file_process-1.4.0/file_process/csv/schemas.py`

 * *Files identical despite different names*

### Comparing `file_process-1.3.4/file_process/exceptions.py` & `file_process-1.4.0/file_process/exceptions.py`

 * *Files identical despite different names*

### Comparing `file_process-1.3.4/file_process/file_processor_factory.py` & `file_process-1.4.0/file_process/file_processor_factory.py`

 * *Files identical despite different names*

### Comparing `file_process-1.3.4/file_process/h5ad/h5ad_processor.py` & `file_process-1.4.0/file_process/h5ad/h5ad_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,28 +18,33 @@
     def validate(self, model_metadata_file: Optional[BytesIO] = None, _: Optional[dict] = None):
         model_data = None
         if model_metadata_file:
             model_data = SbioModelDataForH5ad(model_metadata_file)
         validator = H5ADValidator(self.adata, model_data, enable_warnings=False)
         validator()
 
-    def get_targets(self, is_var_targets: Optional[bool] = False):
-        return list(self.adata.var.columns) if is_var_targets else list(self.adata.obs.columns)
+    def get_obs_targets(self):
+        return list(self.adata.obs.columns)
+
+    def get_var_targets(self):
+        return list(self.adata.var.columns)
 
     def get_observations(self, rows_number: Optional[int] = None):
         return self.adata.obs.head(n=rows_number)
 
     def get_variables(self, rows_number: Optional[int] = None):
         return self.adata.var.head(n=rows_number)
 
-    def get_preview(self, is_var_targets: Optional[bool] = False):
-        target_names = self.get_targets(is_var_targets)
+    def get_preview(self):
+        var_target_names = self.get_var_targets()
+        obs_target_names = self.get_obs_targets()
         obs_preview = self.get_observations(PREVIEW_ROWS_COUNT)
         var_preview = self.get_variables(PREVIEW_ROWS_COUNT)
-        return target_names, self.create_tabular_response(obs_preview), self.create_tabular_response(var_preview), None
+        return var_target_names, obs_target_names, self.create_tabular_response(
+            obs_preview), self.create_tabular_response(var_preview), None
 
     @staticmethod
     def create_tabular_response(data_df: pd.DataFrame) -> List[dict]:
         if data_df is None:
             return []
         data_df = data_df.astype(object)
         rows = data_df.round(2).where(pd.notnull(data_df), None).to_dict(orient='records')
```

### Comparing `file_process-1.3.4/file_process/h5ad/h5ad_validator.py` & `file_process-1.4.0/file_process/h5ad/h5ad_validator.py`

 * *Files identical despite different names*

### Comparing `file_process-1.3.4/file_process.egg-info/SOURCES.txt` & `file_process-1.4.0/file_process.egg-info/SOURCES.txt`

 * *Files identical despite different names*

