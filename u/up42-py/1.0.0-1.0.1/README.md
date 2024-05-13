# Comparing `tmp/up42_py-1.0.0.tar.gz` & `tmp/up42_py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up42_py-1.0.0.tar", max compression
+gzip compressed data, was "up42_py-1.0.1.tar", max compression
```

## Comparing `up42_py-1.0.0.tar` & `up42_py-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1061 2024-04-17 09:59:47.743636 up42_py-1.0.0/LICENSE
--rw-r--r--   0        0        0     2990 2024-04-17 09:59:47.743636 up42_py-1.0.0/README.md
--rw-r--r--   0        0        0     1786 2024-04-17 09:59:47.763636 up42_py-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1731 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/__init__.py
--rw-r--r--   0        0        0     7991 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/asset.py
--rw-r--r--   0        0        0     3754 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/asset_searcher.py
--rw-r--r--   0        0        0     5068 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/auth.py
--rw-r--r--   0        0        0    20308 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/catalog.py
--rw-r--r--   0        0        0      706 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/data/aoi_berlin.geojson
--rw-r--r--   0        0        0      703 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/data/aoi_washington.geojson
--rw-r--r--   0        0        0      135 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/host.py
--rw-r--r--   0        0        0        0 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/__init__.py
--rw-r--r--   0        0        0     1782 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/client.py
--rw-r--r--   0        0        0      484 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/config.py
--rw-r--r--   0        0        0      673 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/http_adapter.py
--rw-r--r--   0        0        0     3290 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/oauth.py
--rw-r--r--   0        0        0     1113 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/session.py
--rw-r--r--   0        0        0     1885 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/initialization.py
--rw-r--r--   0        0        0     3424 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/main.py
--rw-r--r--   0        0        0     8372 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/order.py
--rw-r--r--   0        0        0      910 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/stac_client.py
--rw-r--r--   0        0        0     8485 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/storage.py
--rw-r--r--   0        0        0    10622 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/tasking.py
--rw-r--r--   0        0        0     3287 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/tools.py
--rw-r--r--   0        0        0    14820 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/utils.py
--rw-r--r--   0        0        0     6749 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/webhooks.py
--rw-r--r--   0        0        0     4034 1970-01-01 00:00:00.000000 up42_py-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-13 13:28:15.224450 up42_py-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2927 2024-05-13 13:28:15.224450 up42_py-1.0.1/README.md
+-rw-r--r--   0        0        0     1785 2024-05-13 13:28:15.244451 up42_py-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1731 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/__init__.py
+-rw-r--r--   0        0        0     7963 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/asset.py
+-rw-r--r--   0        0        0     3754 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/asset_searcher.py
+-rw-r--r--   0        0        0     5068 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/auth.py
+-rw-r--r--   0        0        0    20308 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/catalog.py
+-rw-r--r--   0        0        0      706 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/data/aoi_berlin.geojson
+-rw-r--r--   0        0        0      703 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/data/aoi_washington.geojson
+-rw-r--r--   0        0        0      135 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/host.py
+-rw-r--r--   0        0        0        0 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/__init__.py
+-rw-r--r--   0        0        0     1782 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/client.py
+-rw-r--r--   0        0        0      482 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/config.py
+-rw-r--r--   0        0        0      673 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/http_adapter.py
+-rw-r--r--   0        0        0     3290 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/oauth.py
+-rw-r--r--   0        0        0     1113 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/session.py
+-rw-r--r--   0        0        0     1885 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/initialization.py
+-rw-r--r--   0        0        0     3424 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/main.py
+-rw-r--r--   0        0        0     8372 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/order.py
+-rw-r--r--   0        0        0      910 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/stac_client.py
+-rw-r--r--   0        0        0     8485 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/storage.py
+-rw-r--r--   0        0        0    10622 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/tasking.py
+-rw-r--r--   0        0        0     3287 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/tools.py
+-rw-r--r--   0        0        0    15164 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/utils.py
+-rw-r--r--   0        0        0     6749 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/webhooks.py
+-rw-r--r--   0        0        0     3964 1970-01-01 00:00:00.000000 up42_py-1.0.1/PKG-INFO
```

### Comparing `up42_py-1.0.0/LICENSE` & `up42_py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/README.md` & `up42_py-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -73,8 +73,8 @@
 asset = up42.initialize_order(order_id=order.order_id).get_assets()[0]
 stac_items = asset.stac_items
 asset.get_stac_asset_url(stac_asset=stac_items[0].assets.get("b02.tiff"))
 ```
 
 ## Support
 
-For any kind of issues or suggestions please see the [documentation](https://sdk.up42.com/), open a [GitHub issue](https://github.com/up42/up42-py/issues) or [contact support](https://up42.com/company/contact-support).
+For any kind of issues or suggestions please see the [documentation](https://sdk.up42.com/) or [contact support](https://up42.com/company/contact-support).
```

#### html2text {}

```diff
@@ -26,10 +26,9 @@
 scene order_parameters = catalog.construct_order_parameters
 ( data_product_id=data_product_id, image_id=search_results.id[0])
 catalog.estimate_order(order_parameters) order = catalog.place_order
 (order_parameters, track_status=True) # Stream cloud-native files directly for
 your use case asset = up42.initialize_order(order_id=order.order_id).get_assets
 ()[0] stac_items = asset.stac_items asset.get_stac_asset_url
 (stac_asset=stac_items[0].assets.get("b02.tiff")) ``` ## Support For any kind
-of issues or suggestions please see the [documentation](https://sdk.up42.com/),
-open a [GitHub issue](https://github.com/up42/up42-py/issues) or [contact
-support](https://up42.com/company/contact-support).
+of issues or suggestions please see the [documentation](https://sdk.up42.com/
+) or [contact support](https://up42.com/company/contact-support).
```

### Comparing `up42_py-1.0.0/pyproject.toml` & `up42_py-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "up42-py"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python SDK for UP42, the geospatial marketplace and developer platform."
 authors = ["UP42 GmbH <support@up42.com>"]
 license = "https://github.com/up42/up42-py/blob/master/LICENSE"
 readme = "README.md"
 packages = [
     { include = "up42", from = "." },
 ]
@@ -16,15 +16,15 @@
     "Intended Audience :: Developers",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4"
 requests = "^2.31.0"
 tqdm = "^4.66.0"
-geojson = "^3.0.1"
+geojson = "3.1.0"
 geopandas = "^0.13.2"
 pystac-client = "^0.7.2"
 pyproj = "^3.6.1"
 
 
 [tool.poetry.dev-dependencies]
 nbconvert = "^7.16.2"
```

### Comparing `up42_py-1.0.0/up42/__init__.py` & `up42_py-1.0.1/up42/__init__.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/asset.py` & `up42_py-1.0.1/up42/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,20 +162,20 @@
         else:
             output_directory = pathlib.Path(output_directory)
         output_directory.mkdir(parents=True, exist_ok=True)
         logger.info("Download directory: %s", output_directory)
 
         download_url = self._get_download_url()
         if unpacking:
-            out_filepaths = utils.download_from_gcs_unpack(
+            out_filepaths = utils.download_archive(
                 download_url=download_url,
                 output_directory=output_directory,
             )
         else:
-            out_filepaths = utils.download_gcs_not_unpack(
+            out_filepaths = utils.download_file(
                 download_url=download_url,
                 output_directory=output_directory,
             )
 
         self.results = out_filepaths
         return out_filepaths
 
@@ -206,9 +206,9 @@
         else:
             output_directory = pathlib.Path(output_directory)
         output_directory.mkdir(parents=True, exist_ok=True)
         logger.info("Download directory: %s", output_directory)
         download_url = self.get_stac_asset_url(stac_asset=stac_asset)
         file_name = utils.get_filename(download_url, default_filename="stac_asset")
         out_file_path = output_directory / file_name
-        utils.download_gcs_not_unpack(download_url, output_directory)
+        utils.download_file(download_url, output_directory)
         return out_file_path
```

### Comparing `up42_py-1.0.0/up42/asset_searcher.py` & `up42_py-1.0.1/up42/asset_searcher.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/auth.py` & `up42_py-1.0.1/up42/auth.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/catalog.py` & `up42_py-1.0.1/up42/catalog.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/data/aoi_berlin.geojson` & `up42_py-1.0.1/up42/data/aoi_berlin.geojson`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/data/aoi_washington.geojson` & `up42_py-1.0.1/up42/data/aoi_washington.geojson`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/http/client.py` & `up42_py-1.0.1/up42/http/client.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/http/http_adapter.py` & `up42_py-1.0.1/up42/http/http_adapter.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/http/oauth.py` & `up42_py-1.0.1/up42/http/oauth.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/http/session.py` & `up42_py-1.0.1/up42/http/session.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/initialization.py` & `up42_py-1.0.1/up42/initialization.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/main.py` & `up42_py-1.0.1/up42/main.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/order.py` & `up42_py-1.0.1/up42/order.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/stac_client.py` & `up42_py-1.0.1/up42/stac_client.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/storage.py` & `up42_py-1.0.1/up42/storage.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/tasking.py` & `up42_py-1.0.1/up42/tasking.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/tools.py` & `up42_py-1.0.1/up42/tools.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/up42/utils.py` & `up42_py-1.0.1/up42/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,74 +93,84 @@
             return func(*args, **kwargs)
 
         return wrapper
 
     return actual_decorator
 
 
-def download_from_gcs_unpack(
+def _unpack_tar_files(file_path: str, output_directory: Union[str, pathlib.Path]) -> List[pathlib.Path]:
+    out_filepaths: List[pathlib.Path] = []
+    if tarfile.is_tarfile(file_path):
+        with tarfile.open(file_path) as tar_file:
+            for tar_member in tar_file.getmembers():
+                if tar_member.isfile():
+                    if "output/" in tar_member.name:
+                        tar_member.name = tar_member.name.split("output/")[1]
+                    tar_file.extract(tar_member, output_directory)
+                    out_filepaths.append(pathlib.Path(output_directory) / tar_member.name)
+    return out_filepaths
+
+
+def _unpack_zip_files(file_path: str, output_directory: Union[str, pathlib.Path]) -> List[pathlib.Path]:
+    out_filepaths: List[pathlib.Path] = []
+    if zipfile.is_zipfile(file_path):
+        with zipfile.ZipFile(file_path) as zip_file:
+            for zip_info in zip_file.infolist():
+                if not zip_info.filename.endswith("/"):
+                    if "output/" in zip_info.filename:
+                        zip_info.filename = zip_info.filename.split("output/")[1]
+                    zip_file.extract(zip_info, output_directory)
+                    out_filepaths.append(pathlib.Path(output_directory) / zip_info.filename)
+    return out_filepaths
+
+
+def download_archive(
     download_url: str,
     output_directory: Union[str, pathlib.Path],
 ) -> List[str]:
     """
     General download function for results of storage assets, job & jobtask from cloud storage
     provider.
 
     Args:
         download_url: The signed gcs url to download.
         output_directory: The file output directory, defaults to the current working
             directory.
     """
     # Download
-    out_temp = tempfile.mkstemp()[1]
-    with open(out_temp, "wb") as dst:
+    with tempfile.NamedTemporaryFile(dir=output_directory) as dst:
         try:
             r = requests.get(download_url, stream=True, timeout=TIMEOUT)
             r.raise_for_status()
             for chunk in tqdm.tqdm(r.iter_content(chunk_size=CHUNK_SIZE)):
                 if chunk:  # filter out keep-alive new chunks
                     dst.write(chunk)
+            dst.flush()
         except requests.exceptions.HTTPError as err:
             error_message = f"Connection error, please try again! {err}"
             logger.debug(error_message)
             raise requests.exceptions.HTTPError(error_message)
+        # Order results are zip, job results are tgz(tar.gzipped)
+        out_filepaths = _unpack_tar_files(dst.name, output_directory) + _unpack_zip_files(dst.name, output_directory)
 
-    # Unpack
-    # Order results are zip, job results are tgz(tar.gzipped)
-    out_filepaths: List[pathlib.Path] = []
-    if tarfile.is_tarfile(out_temp):
-        with tarfile.open(out_temp) as tar_file:
-            for tar_member in tar_file.getmembers():
-                if tar_member.isfile():
-                    # Avoid up42 inherent output/ .. directory
-                    if "output/" in tar_member.name:
-                        tar_member.name = tar_member.name.split("output/")[1]
-                    tar_file.extract(tar_member, output_directory)
-                    out_filepaths.append(pathlib.Path(output_directory) / tar_member.name)
-    elif zipfile.is_zipfile(out_temp):
-        with zipfile.ZipFile(out_temp) as zip_file:
-            for zip_info in zip_file.infolist():
-                if not zip_info.filename.endswith("/"):
-                    # Avoid up42 inherent output/ .. directory
-                    if "output/" in zip_info.filename:
-                        zip_info.filename = zip_info.filename.split("output/")[1]
-                    zip_file.extract(zip_info, output_directory)
-                    out_filepaths.append(pathlib.Path(output_directory) / zip_info.filename)
-    else:
-        raise ValueError("Downloaded file is not a TGZ/TAR or ZIP archive.")
-    logger.info(
-        "Download successful of %s files to output_directory '%s': %s",
-        len(out_filepaths),
-        output_directory,
-        [p.name for p in out_filepaths],
-    )
+        if not out_filepaths:
+            raise UnsupportedArchive("Downloaded file is not a TGZ/TAR or ZIP archive.")
+        logger.info(
+            "Download successful of %s files to output_directory %s",
+            len(out_filepaths),
+            output_directory,
+        )
     return [str(p) for p in out_filepaths]
 
 
-def download_gcs_not_unpack(download_url: str, output_directory: Union[str, pathlib.Path]) -> List[str]:
+class UnsupportedArchive(ValueError):
+    pass
+
+
+def download_file(download_url: str, output_directory: Union[str, pathlib.Path]) -> List[str]:
     """
     General download function for assets, job and jobtasks from cloud storage
     provider.
 
     Args:
         download_url: The signed gcs url to download.
         output_directory: The file output directory, defaults to the current working
```

### Comparing `up42_py-1.0.0/up42/webhooks.py` & `up42_py-1.0.1/up42/webhooks.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.0/PKG-INFO` & `up42_py-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up42-py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python SDK for UP42, the geospatial marketplace and developer platform.
 License: https://github.com/up42/up42-py/blob/master/LICENSE
 Author: UP42 GmbH
 Author-email: support@up42.com
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: geojson (>=3.0.1,<4.0.0)
+Requires-Dist: geojson (==3.1.0)
 Requires-Dist: geopandas (>=0.13.2,<0.14.0)
 Requires-Dist: pyproj (>=3.6.1,<4.0.0)
 Requires-Dist: pystac-client (>=0.7.2,<0.8.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.0,<5.0.0)
 Description-Content-Type: text/markdown
 
@@ -99,9 +99,9 @@
 asset = up42.initialize_order(order_id=order.order_id).get_assets()[0]
 stac_items = asset.stac_items
 asset.get_stac_asset_url(stac_asset=stac_items[0].assets.get("b02.tiff"))
 ```
 
 ## Support
 
-For any kind of issues or suggestions please see the [documentation](https://sdk.up42.com/), open a [GitHub issue](https://github.com/up42/up42-py/issues) or [contact support](https://up42.com/company/contact-support).
+For any kind of issues or suggestions please see the [documentation](https://sdk.up42.com/) or [contact support](https://up42.com/company/contact-support).
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: up42-py Version: 1.0.0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: up42-py Version: 1.0.1 Summary: Python SDK for
 UP42, the geospatial marketplace and developer platform. License: https://
 github.com/up42/up42-py/blob/master/LICENSE Author: UP42 GmbH Author-email:
 support@up42.com Requires-Python: >=3.9,<4 Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
-Dist: geojson (>=3.0.1,<4.0.0) Requires-Dist: geopandas (>=0.13.2,<0.14.0)
-Requires-Dist: pyproj (>=3.6.1,<4.0.0) Requires-Dist: pystac-client
-(>=0.7.2,<0.8.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: tqdm
-(>=4.66.0,<5.0.0) Description-Content-Type: text/markdown
+Dist: geojson (==3.1.0) Requires-Dist: geopandas (>=0.13.2,<0.14.0) Requires-
+Dist: pyproj (>=3.6.1,<4.0.0) Requires-Dist: pystac-client (>=0.7.2,<0.8.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: tqdm (>=4.66.0,<5.0.0)
+Description-Content-Type: text/markdown
     PPyytthhoonn SSDDKK ffoorr UUPP4422,, tthhee ggeeoossppaattiiaall mmaarrkkeettppllaaccee aanndd ddeevveellooppeerr ppllaattffoorrmm..
 ![](docs/assets/github-banner-3.jpg)
       _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_u_p_4_2_-_p_y_?_c_o_l_o_r_=_b_r_i_g_h_t_g_r_e_e_n_][https://
 sonarcloud.io/api/project_badges/measure?project=up42_up42-py&metric=coverage]
         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/_U_P_4_2___._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_]
                 _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ?  ?â??¢ ?  _UU_PP_44_22_.._cc_oo_mm ?  ?â??¢ ?  _SS_uu_pp_pp_oo_rr_tt
 ## Highlights - Python package for easy access to [UP42's](http://www.up42.com)
@@ -40,10 +40,9 @@
 scene order_parameters = catalog.construct_order_parameters
 ( data_product_id=data_product_id, image_id=search_results.id[0])
 catalog.estimate_order(order_parameters) order = catalog.place_order
 (order_parameters, track_status=True) # Stream cloud-native files directly for
 your use case asset = up42.initialize_order(order_id=order.order_id).get_assets
 ()[0] stac_items = asset.stac_items asset.get_stac_asset_url
 (stac_asset=stac_items[0].assets.get("b02.tiff")) ``` ## Support For any kind
-of issues or suggestions please see the [documentation](https://sdk.up42.com/),
-open a [GitHub issue](https://github.com/up42/up42-py/issues) or [contact
-support](https://up42.com/company/contact-support).
+of issues or suggestions please see the [documentation](https://sdk.up42.com/
+) or [contact support](https://up42.com/company/contact-support).
```

