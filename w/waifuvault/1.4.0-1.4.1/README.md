# Comparing `tmp/waifuvault-1.4.0.tar.gz` & `tmp/waifuvault-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waifuvault-1.4.0.tar", last modified: Mon Apr 22 15:05:46 2024, max compression
+gzip compressed data, was "waifuvault-1.4.1.tar", last modified: Mon May 13 13:26:54 2024, max compression
```

## Comparing `waifuvault-1.4.0.tar` & `waifuvault-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:05:46.216951 waifuvault-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 15:05:34.000000 waifuvault-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-22 15:05:46.212951 waifuvault-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-04-22 15:05:34.000000 waifuvault-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-22 15:05:34.000000 waifuvault-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:05:46.216951 waifuvault-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:05:46.212951 waifuvault-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:05:46.212951 waifuvault-1.4.0/src/waifuvault/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-22 15:05:34.000000 waifuvault-1.4.0/src/waifuvault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-22 15:05:34.000000 waifuvault-1.4.0/src/waifuvault/waifumodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-22 15:05:34.000000 waifuvault-1.4.0/src/waifuvault/waifuvault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:05:46.212951 waifuvault-1.4.0/src/waifuvault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-22 15:05:46.000000 waifuvault-1.4.0/src/waifuvault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-22 15:05:46.000000 waifuvault-1.4.0/src/waifuvault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:05:46.000000 waifuvault-1.4.0/src/waifuvault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 15:05:46.000000 waifuvault-1.4.0/src/waifuvault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 15:05:46.000000 waifuvault-1.4.0/src/waifuvault.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:05:46.212951 waifuvault-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-22 15:05:34.000000 waifuvault-1.4.0/tests/test_waifuvault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:26:54.739047 waifuvault-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 13:26:43.000000 waifuvault-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-05-13 13:26:54.739047 waifuvault-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-13 13:26:43.000000 waifuvault-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-13 13:26:43.000000 waifuvault-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:26:54.739047 waifuvault-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:26:54.735047 waifuvault-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:26:54.739047 waifuvault-1.4.1/src/waifuvault/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-13 13:26:43.000000 waifuvault-1.4.1/src/waifuvault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-13 13:26:43.000000 waifuvault-1.4.1/src/waifuvault/waifumodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-13 13:26:43.000000 waifuvault-1.4.1/src/waifuvault/waifuvault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:26:54.739047 waifuvault-1.4.1/src/waifuvault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-05-13 13:26:54.000000 waifuvault-1.4.1/src/waifuvault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-13 13:26:54.000000 waifuvault-1.4.1/src/waifuvault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:26:54.000000 waifuvault-1.4.1/src/waifuvault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 13:26:54.000000 waifuvault-1.4.1/src/waifuvault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 13:26:54.000000 waifuvault-1.4.1/src/waifuvault.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:26:54.739047 waifuvault-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-05-13 13:26:43.000000 waifuvault-1.4.1/tests/test_waifuvault.py
```

### Comparing `waifuvault-1.4.0/LICENSE` & `waifuvault-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `waifuvault-1.4.0/PKG-INFO` & `waifuvault-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waifuvault
-Version: 1.4.0
+Version: 1.4.1
 Summary: waifuVault Python API module
 Author-email: Walker Aldridge <walker@waifuvault.moe>
 Project-URL: Homepage, https://github.com/waifuvault/waifuVault-python-api
 Project-URL: Issues, https://github.com/waifuvault/waifuVault-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `waifuvault-1.4.0/README.md` & `waifuvault-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `waifuvault-1.4.0/pyproject.toml` & `waifuvault-1.4.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waifuvault"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
     { name="Walker Aldridge", email="walker@waifuvault.moe" },
 ]
 description = "waifuVault Python API module"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `waifuvault-1.4.0/src/waifuvault/waifumodels.py` & `waifuvault-1.4.1/src/waifuvault/waifumodels.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,16 +17,14 @@
         return self.target.lower().startswith("http://") or self.target.lower().startswith("https://")
 
     def is_buffer(self):
         return isinstance(self.target, io.BytesIO)
 
     def build_parameters(self):
         parameters = {}
-        if self.password:
-            parameters['password'] = self.password
         if self.expires:
             parameters['expires'] = self.expires
         if self.hidefilename:
             parameters['hide_filename'] = str(self.hidefilename).lower()
         if self.one_time_download:
             parameters['one_time_download'] = str(self.one_time_download).lower()
         return parameters
```

### Comparing `waifuvault-1.4.0/src/waifuvault/waifuvault.py` & `waifuvault-1.4.1/src/waifuvault/waifuvault.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,25 +8,31 @@
 from requests_toolbelt import MultipartEncoder
 
 from .waifumodels import FileResponse, FileUpload, FileOptions
 
 
 # Upload File
 def upload_file(file_obj: FileUpload):
+    fields = {}
+    if file_obj.password:
+        fields['password'] = file_obj.password
     if file_obj.is_buffer():
+        fields['file'] = (file_obj.target_name, file_obj.target)
         multipart_data = MultipartEncoder(
-            fields={'file': (file_obj.target_name, file_obj.target)}
+            fields=fields
         )
         header_data = {'Content-Type': multipart_data.content_type}
     elif file_obj.is_url():
-        multipart_data = {'url': file_obj.target}
+        fields['url'] = file_obj.target
+        multipart_data = fields
         header_data = None
     else:
+        fields['file'] = (os.path.basename(file_obj.target), open(file_obj.target, 'rb'))
         multipart_data = MultipartEncoder(
-            fields={'file': (os.path.basename(file_obj.target), open(file_obj.target, 'rb'))}
+            fields=fields
         )
         header_data = {'Content-Type': multipart_data.content_type}
 
     response = requests.put(
         __base_url__,
         params=file_obj.build_parameters(),
         data=multipart_data,
```

### Comparing `waifuvault-1.4.0/src/waifuvault.egg-info/PKG-INFO` & `waifuvault-1.4.1/src/waifuvault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waifuvault
-Version: 1.4.0
+Version: 1.4.1
 Summary: waifuVault Python API module
 Author-email: Walker Aldridge <walker@waifuvault.moe>
 Project-URL: Homepage, https://github.com/waifuvault/waifuVault-python-api
 Project-URL: Issues, https://github.com/waifuvault/waifuVault-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `waifuvault-1.4.0/tests/test_waifuvault.py` & `waifuvault-1.4.1/tests/test_waifuvault.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,10 +219,9 @@
     file_down = waifuvault.FileUpload("https://waifuvault.moe/test", expires="1d", password="testpassword", hidefilename=True, oneTimeDownload=True)
 
     # When
     args = file_down.build_parameters()
 
     # Then
     assert (args.get("expires") == "1d"), "expires not in arguments"
-    assert (args.get("password") == "testpassword"), "password not in arguments"
     assert (args.get("hide_filename") == "true"), "hide_filename not in arguments"
     assert (args.get("one_time_download") == "true"), "one_time_download not in arguments"
```

