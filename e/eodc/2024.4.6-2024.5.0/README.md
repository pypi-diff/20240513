# Comparing `tmp/eodc-2024.4.6.tar.gz` & `tmp/eodc-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2024.4.6.tar", max compression
+gzip compressed data, was "eodc-2024.5.0.tar", max compression
```

## Comparing `eodc-2024.4.6.tar` & `eodc-2024.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      676 2024-04-30 13:16:50.862928 eodc-2024.4.6/README.md
--rw-r--r--   0        0        0      195 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/auth.py
--rw-r--r--   0        0        0     1311 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/dask.py
--rw-r--r--   0        0        0    13711 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/faas.py
--rw-r--r--   0        0        0     1183 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/settings.py
--rw-r--r--   0        0        0     2240 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/storage.py
--rw-r--r--   0        0        0        0 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/__init__.py
--rwxr-xr-x   0        0        0    15080 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/app.py
--rw-r--r--   0        0        0      261 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/assets/app.css
--rw-r--r--   0        0        0     2539 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/cards.py
--rw-r--r--   0        0        0     8522 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/navbar.py
--rw-r--r--   0        0        0     2867 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/utils.py
--rw-r--r--   0        0        0    32166 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/workspace.py
--rw-r--r--   0        0        0     1890 2024-04-30 13:16:50.866928 eodc-2024.4.6/pyproject.toml
--rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 eodc-2024.4.6/PKG-INFO
+-rw-r--r--   0        0        0      676 2024-05-13 13:27:29.542054 eodc-2024.5.0/README.md
+-rw-r--r--   0        0        0      195 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/__init__.py
+-rw-r--r--   0        0        0     1794 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/auth.py
+-rw-r--r--   0        0        0     1311 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/dask.py
+-rw-r--r--   0        0        0    13711 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/faas.py
+-rw-r--r--   0        0        0     1183 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/settings.py
+-rw-r--r--   0        0        0     2240 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/storage.py
+-rw-r--r--   0        0        0        0 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/__init__.py
+-rwxr-xr-x   0        0        0    15080 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/app.py
+-rw-r--r--   0        0        0      261 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/assets/app.css
+-rw-r--r--   0        0        0     2539 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/cards.py
+-rw-r--r--   0        0        0     8522 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/navbar.py
+-rw-r--r--   0        0        0     2867 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/visualisation/vessel_detection/utils.py
+-rw-r--r--   0        0        0    32787 2024-05-13 13:27:29.542054 eodc-2024.5.0/eodc/workspace.py
+-rw-r--r--   0        0        0     1890 2024-05-13 13:27:29.546054 eodc-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 eodc-2024.5.0/PKG-INFO
```

### Comparing `eodc-2024.4.6/README.md` & `eodc-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.6/eodc/auth.py` & `eodc-2024.5.0/eodc/auth.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.6/eodc/dask.py` & `eodc-2024.5.0/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.6/eodc/faas.py` & `eodc-2024.5.0/eodc/faas.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.6/eodc/settings.py` & `eodc-2024.5.0/eodc/settings.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.6/eodc/storage.py` & `eodc-2024.5.0/eodc/storage.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.6/eodc/visualisation/vessel_detection/app.py` & `eodc-2024.5.0/eodc/visualisation/vessel_detection/app.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.6/eodc/visualisation/vessel_detection/cards.py` & `eodc-2024.5.0/eodc/visualisation/vessel_detection/cards.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.6/eodc/visualisation/vessel_detection/navbar.py` & `eodc-2024.5.0/eodc/visualisation/vessel_detection/navbar.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.6/eodc/visualisation/vessel_detection/utils.py` & `eodc-2024.5.0/eodc/visualisation/vessel_detection/utils.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.6/eodc/workspace.py` & `eodc-2024.5.0/eodc/workspace.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 import os
 import subprocess as sp
 import uuid
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 from enum import Enum
 from pathlib import Path
 from typing import Any, Optional, TypedDict, Union
 
 import boto3
 import fsspec
 import pystac
-from azure.identity import DefaultAzureCredential
 from azure.storage.blob import BlobServiceClient
 from minio import Minio, MinioAdmin
 from pydantic import SecretStr
 from pystac import Item, Link
 from pystac.extensions.eo import Band, EOExtension
 from pystac.stac_io import DefaultStacIO
 from typing_extensions import Self
@@ -28,40 +27,41 @@
 
 class StorageType(Enum):
     MINIO = "minio"
     AZURE = "azure"
     CEPH = "ceph"
 
 
-class WorkspaceAdapter(ABC):
+class WorkspaceAdapter(DefaultStacIO):
     """
     The WorkspaceAdapter is an abstract class that defines the minimum
     interface for interacting with workspaces. It abstracts away the
     underlying storage system, so that the EODC API can be used with
     different providers.
+
+    It also implements the DefaultStacIO interface, which allows it to
+    be used with the pystac library.
     """
 
     @staticmethod
     def create_adapter(
-        tenant_url: str = None,
+        tenant_url: str = None,  # Can be ignored for Azure
         storage_type: StorageType = StorageType.MINIO,
         parameters: dict[str, Any] = {},
     ) -> Self:
         if storage_type == StorageType.MINIO:
             return MinIOAdapter(
                 url=tenant_url,
                 access_key=parameters["access_key"],
                 secret_key=parameters["secret_key"],
                 mc_bin_path=parameters["mc_bin_path"],
             )
         elif storage_type == StorageType.AZURE:
             return AzureAdapter(
-                url=tenant_url,
-                access_key=parameters["client_id"],
-                secret_key=parameters["client_secret"],
+                connection_string=parameters["connection_string"],
             )
         elif storage_type == StorageType.CEPH:
             return CephAdapter(
                 url=tenant_url,
                 access_key=parameters["access_key"],
                 secret_key=parameters["secret_key"],
             )
@@ -87,15 +87,15 @@
         pass
 
     @abstractmethod
     def list_workspace_files(self, workspace_name: str):
         pass
 
     @abstractmethod
-    def upload_file(self, workspace_name: str, file_path: str):
+    def upload_file(self, workspace_name: str, file_path: str, path_in_workspace: str):
         pass
 
     @abstractmethod
     def upload_stream(self, workspace_name: str, stream: Any, file_name: str):
         pass
 
     @abstractmethod
@@ -110,14 +110,119 @@
     def download_stream(self, workspace_name: str, file_name: str):
         pass
 
     @abstractmethod
     def get_fsspec(self, workspace_name: str):
         pass
 
+    @abstractmethod
+    def get_signed_url(
+        self, bucket_name, object_key, method="GET", expiration_time=3600
+    ):
+        pass
+
+    def upload_path(
+        self,
+        workspace_name: str = "",
+        path: str = "",
+        path_in_workspace: str = "",
+        recursive: bool = False,
+    ):
+        path_in_workspace = path_in_workspace.removesuffix("/")
+        files = Path(path).rglob("*") if recursive else Path(path).glob("*")
+
+        for file in files:
+            if not file.is_file():
+                continue
+            relative_path = "/".join(os.path.relpath(file, path).split("/")[:-1])
+            new_path_in_workspace = os.path.join(path_in_workspace, relative_path)
+
+            self.upload_file(
+                workspace_name,
+                str(file),
+                "" if new_path_in_workspace == "/" else new_path_in_workspace,
+            )
+
+    def _wrap_urls_modifier(
+        self,
+        item: pystac.Item,
+        bucket_name,
+        collection_name,
+        url_modifier=None,
+        **kwargs,
+    ):
+        # Get the signed URL for the item
+
+        object_key = f"{collection_name}/{item.id}.tif"
+        if not url_modifier:
+            modified_url = self.get_signed_url(
+                bucket_name, object_key=object_key, **kwargs
+            )
+        else:
+            modified_url = url_modifier(bucket_name, object_key, **kwargs)
+
+        # Update the item's href with the signed URL
+
+        item_dict = item.to_dict(transform_hrefs=False)
+        item_dict["assets"]["raster-result"]["href"] = modified_url
+
+        return pystac.Item.from_dict(item_dict, preserve_dict=False)
+
+    def get_stac_items(
+        self, bucket_name, collection_name, url_modifier=None, **kwargs
+    ) -> list[Item]:
+        collection: pystac.Collection = pystac.read_file(
+            href=f"/{bucket_name}/{collection_name}/STAC/{collection_name}_collection.json",
+            stac_io=self,
+        )
+
+        items: list[Item] = [
+            pystac.Item.from_file(
+                href=self._modify_href(item, bucket_name, collection_name), stac_io=self
+            )
+            for item in collection.get_item_links()
+        ]
+
+        for item in items:
+            eo = EOExtension.ext(item, add_if_missing=True)
+            eo.apply(bands=raster_band)
+            # re = RasterExtension.ext(item, add_if_missing=True)
+
+        return [
+            self._wrap_urls_modifier(
+                item, bucket_name, collection_name, url_modifier, **kwargs
+            )
+            for item in items
+        ]
+
+    # Implement the abstract methods from DefaultStacIO
+    def read_text(self, source: Union[str, Link], *args: Any, **kwargs: Any) -> str:
+        bucket_name, object_key = self.parse_workspace_STAC_source(source)
+        data = self.download_stream(bucket_name, object_key).read().decode("utf-8")
+        return data
+
+    def write_text(
+        self, dest: Union[str, Link], txt: str, *args: Any, **kwargs: Any
+    ) -> None:
+        pass
+
+    def parse_workspace_STAC_source(self, source: Union[str, Link]) -> tuple[str, str]:
+        """ """
+        split_source = source.split("/")
+
+        workspace_name = split_source[1]
+        object_key = "/".join(split_source[2:])
+
+        return workspace_name, object_key
+
+    def _modify_href(self, href: Link, bucket_name: str, collection_name: str):
+        id = str(href.target).split("/")[-1].split(".")[0]
+
+        return f"/{bucket_name}/{collection_name}/STAC/items/{id}.json"
+
 
 class MinIOAdapter(WorkspaceAdapter):
     """
     The system on which this is running needs to have the mc (Minio Client)
     CLI tool installed
 
     This Adapter implements the MinIO API for the EODC Tenant, for local workspaces
@@ -340,15 +445,15 @@
     def _create_workspace(self, workspace_name: str):
         """
         raises S3Error
         """
         self.minio_client.make_bucket(workspace_name)
 
 
-class CephAdapter(WorkspaceAdapter, DefaultStacIO):
+class CephAdapter(WorkspaceAdapter):
     """
     This Adapter implements the Ceph API for the Workspaces API.
 
     Workspaces are implemented as buckets, and files are implemented
     as objects.
     """
 
@@ -419,35 +524,14 @@
         path_in_workspace = path_in_workspace.removesuffix("/")
         self.s3_client.upload_file(
             file_path,
             workspace_name,
             os.path.join(path_in_workspace, file_path.split("/")[-1]),
         )
 
-    def upload_path(
-        self,
-        workspace_name: str,
-        path: str,
-        path_in_workspace: str = "",
-        recursive: bool = False,
-    ):
-        path_in_workspace = path_in_workspace.removesuffix("/")
-        files = Path(path).rglob("*") if recursive else Path(path).glob("*")
-
-        for file in files:
-            if not file.is_file():
-                continue
-            relative_path = "/".join(os.path.relpath(file, path).split("/")[:-1])
-            new_path_in_workspace = os.path.join(path_in_workspace + relative_path)
-            self.upload_file(
-                workspace_name,
-                str(file),
-                "" if new_path_in_workspace == "/" else new_path_in_workspace,
-            )
-
     def upload_openeo_results():
         pass
 
     def upload_stream(self, workspace_name: str, stream: Any, file_name: str):
         self.s3_client.put_object(Bucket=workspace_name, Key=file_name, Body=stream)
 
     def delete_file(self, workspace_name: str, file_name: str):
@@ -482,71 +566,14 @@
             ClientMethod=method,
             Params={"Bucket": bucket_name, "Key": object_key},
             ExpiresIn=expiration_time,
         )
 
         return signed_url
 
-    def _modify_href(self, href: Link, bucket_name: str, collection_name: str):
-        id = str(href.target).split("/")[-1].split(".")[0]
-
-        return f"/{bucket_name}/{collection_name}/STAC/items/{id}.json"
-
-    def _wrap_urls_modifier(
-        self,
-        item: pystac.Item,
-        bucket_name,
-        collection_name,
-        url_modifier=None,
-        **kwargs,
-    ):
-        # Get the signed URL for the item
-
-        object_key = f"{collection_name}/{item.id}.tif"
-        if not url_modifier:
-            modified_url = self.get_signed_url(
-                bucket_name, object_key=object_key, **kwargs
-            )
-        else:
-            modified_url = url_modifier(bucket_name, object_key, **kwargs)
-
-        # Update the item's href with the signed URL
-
-        item_dict = item.to_dict(transform_hrefs=False)
-        item_dict["assets"]["raster-result"]["href"] = modified_url
-
-        return pystac.Item.from_dict(item_dict, preserve_dict=False)
-
-    def get_stac_items(
-        self, bucket_name, collection_name, url_modifier=None, **kwargs
-    ) -> list[Item]:
-        collection: pystac.Collection = pystac.read_file(
-            href=f"/{bucket_name}/{collection_name}/STAC/{collection_name}_collection.json",
-            stac_io=self,
-        )
-
-        items: list[Item] = [
-            pystac.Item.from_file(
-                href=self._modify_href(item, bucket_name, collection_name), stac_io=self
-            )
-            for item in collection.get_item_links()
-        ]
-
-        for item in items:
-            eo = EOExtension.ext(item, add_if_missing=True)
-            eo.apply(bands=raster_band)
-            # re = RasterExtension.ext(item, add_if_missing=True)
-
-        return [
-            self._wrap_urls_modifier(
-                item, bucket_name, collection_name, url_modifier, **kwargs
-            )
-            for item in items
-        ]
-
     # Policies
     def _grant_policy_to_workspace(self, workspace_name: str, policy_string: str):
         self.s3_client.put_bucket_policy(Bucket=workspace_name, Policy=policy_string)
 
     def grant_workspace_to_user(self, user_name: str, workspace_name: str, tenant_name):
         policy_str = (
             S3PolicyBuilder(f"BASIC_{workspace_name.upper()}_{tenant_name}_{user_name}")
@@ -558,71 +585,55 @@
         self._grant_policy_to_workspace(
             workspace_name=workspace_name, policy_string=json.dumps(policy_str)
         )
 
     def describe_workspace_policy(self, workspace_name: str):
         return self.s3_client.get_bucket_policy(Bucket=workspace_name)
 
-    # Implement the abstract methods from DefaultStacIO
-
-    def parse_workspace_STAC_source(self, source: Union[str, Link]) -> tuple[str, str]:
-        """ """
-        split_source = source.split("/")
-
-        bucket_name = split_source[1]
-        object_key = "/".join(split_source[2:])
-
-        return bucket_name, object_key
-
-    def read_text(self, source: Union[str, Link], *args: Any, **kwargs: Any) -> str:
-        bucket_name, object_key = self.parse_workspace_STAC_source(source)
-        data = self.download_stream(bucket_name, object_key).read().decode("utf-8")
-        return data
-
-    def write_text(
-        self, dest: Union[str, Link], txt: str, *args: Any, **kwargs: Any
-    ) -> None:
-        pass
-
 
 class AzureAdapter(WorkspaceAdapter):
     """
     This Adapter implements the Azure API for the Workspaces API.
 
     Workspaces are implemented as containers, and files are implemented
     as blobs.
     """
 
     blob_service_client: BlobServiceClient
 
     def __init__(
         self,
-        url: str,
-        client_id: SecretStr,
-        client_secret: SecretStr,
+        connection_string: SecretStr,
     ):
-        self.blob_service_client = BlobServiceClient(
-            account_url=url,
-            credential=DefaultAzureCredential(
-                client_id=client_id.get_secret_value(),
-                client_secret=client_secret.get_secret_value(),
-            ),
+        self.blob_service_client = BlobServiceClient.from_connection_string(
+            conn_str=connection_string.get_secret_value()
         )
 
+    def create_user_workspace(self, workspace_name: str, user_name: str, **kwargs):
+        self.blob_service_client.create_container(workspace_name)
+
+    def delete_user_workspace(self, workspace_name: str):
+        self.blob_service_client.delete_container(workspace_name)
+
     def get_fsspec(self, workspace_name: str):
         return fsspec.filesystem(
             "az",
             anon=False,
             key=self.blob_service_client.credential.token["access_token"],
             client_kwargs={
                 "account_url": self.blob_service_client.url,
                 "container": workspace_name,
             },
         )
 
+    def get_signed_url(
+        self, bucket_name, object_key, method="GET", expiration_time=3600
+    ):
+        return ""
+
     def workspace_exists(self, workspace_name: str) -> bool:
         return self.blob_service_client.get_container_client(
             container=workspace_name
         ).exists()
 
     def list_workspaces(self) -> list[str]:
         return [
@@ -633,18 +644,25 @@
         return [
             blob.name
             for blob in self.blob_service_client.get_container_client(
                 container=workspace_name
             ).list_blobs()
         ]
 
-    def upload_file(self, workspace_name: str, file_path: str):
-        self.blob_service_client.get_blob_client(
-            container=workspace_name, blob=file_path.split("/")[-1]
-        ).upload_blob(file_path)
+    def upload_file(
+        self, workspace_name: str, file_path: str, path_in_workspace: str
+    ) -> None:
+        blob_path = str(
+            Path(path_in_workspace).joinpath(file_path.split("/")[-1]),
+        )
+        with open(file_path, "rb") as data:
+            self.blob_service_client.get_blob_client(
+                container=workspace_name,
+                blob=blob_path,
+            ).upload_blob(data)
 
     def upload_stream(self, workspace_name: str, stream: Any, file_name: str):
         self.blob_service_client.get_blob_client(
             container=workspace_name, blob=file_name
         ).upload_blob(stream)
 
     def delete_file(self, workspace_name: str, file_name: str):
@@ -654,21 +672,17 @@
 
     def download_file(self, workspace_name: str, file_name: str, path: str):
         self.blob_service_client.get_blob_client(
             container=workspace_name, blob=file_name
         ).download_blob().readinto(open(path, "wb"))
 
     def download_stream(self, workspace_name: str, file_name: str):
-        return (
-            self.blob_service_client.get_blob_client(
-                container=workspace_name, blob=file_name
-            )
-            .download_blob()
-            .readall()
-        )
+        return self.blob_service_client.get_blob_client(
+            container=workspace_name, blob=file_name
+        ).download_blob()
 
 
 class S3PolicyBuilder:
     """
     The s3 policy builder is a handy tool for building s3 policies in a structured way.
     It allows for the creation of policies that can be used to grant or deny access to
     various resources in an s3 bucket. The policy builder can be used to create policies
@@ -681,14 +695,15 @@
     attached to workspaces and objects, as ceph does not support user policies.
 
     This means you add user specific privileges to the policy, and then
     you grant it to the workspace. For this use all functions that look like:
     'add_user_..._privileges'
 
 
+    If the user parameter is '*', the policy will be granted to all users.
     """
 
     class PolicyEntry(TypedDict):
         Effect: bool
         Action: list[str]
         Resource: list[str]
         Condition: Optional[dict[str, Any]]
```

### Comparing `eodc-2024.4.6/pyproject.toml` & `eodc-2024.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "eodc"
 
-version = "2024.4.6"
+version = "2024.5.0"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>", "Christoph Reimer <christoph.reimer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2024.4.6/PKG-INFO` & `eodc-2024.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2024.4.6
+Version: 2024.5.0
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

