# Comparing `tmp/getstream-1.0.0.tar.gz` & `tmp/getstream-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getstream-1.0.0.tar", max compression
+gzip compressed data, was "getstream-1.0.1.tar", max compression
```

## Comparing `getstream-1.0.0.tar` & `getstream-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    14204 2024-05-10 07:12:10.747895 getstream-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     3708 2024-05-10 07:12:10.747895 getstream-1.0.0/README.md
--rw-r--r--   0        0        0       50 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/__init__.py
--rw-r--r--   0        0        0     6264 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/base.py
--rw-r--r--   0        0        0        0 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/chat/__init__.py
--rw-r--r--   0        0        0       24 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/chat/channel.py
--rw-r--r--   0        0        0      267 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/chat/client.py
--rw-r--r--   0        0        0    45004 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/chat/rest_client.py
--rw-r--r--   0        0        0        0 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/common/__init__.py
--rw-r--r--   0        0        0      275 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/common/client.py
--rw-r--r--   0        0        0    20751 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/common/rest_client.py
--rw-r--r--   0        0        0      925 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/config.py
--rw-r--r--   0        0        0       46 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/generic.py
--rw-r--r--   0        0        0      497 2024-05-10 07:12:10.747895 getstream-1.0.0/getstream/meta.py
--rw-r--r--   0        0        0   298794 2024-05-10 07:12:10.751895 getstream-1.0.0/getstream/models/__init__.py
--rw-r--r--   0        0        0     1168 2024-05-10 07:12:10.751895 getstream-1.0.0/getstream/rate_limit.py
--rw-r--r--   0        0        0     4489 2024-05-10 07:12:10.751895 getstream-1.0.0/getstream/stream.py
--rw-r--r--   0        0        0     1024 2024-05-10 07:12:10.751895 getstream-1.0.0/getstream/stream_response.py
--rw-r--r--   0        0        0     3942 2024-05-10 07:12:10.751895 getstream-1.0.0/getstream/utils.py
--rw-r--r--   0        0        0       18 2024-05-10 07:12:10.751895 getstream-1.0.0/getstream/version.py
--rw-r--r--   0        0        0        0 2024-05-10 07:12:10.751895 getstream-1.0.0/getstream/video/__init__.py
--rw-r--r--   0        0        0    10156 2024-05-10 07:12:10.751895 getstream-1.0.0/getstream/video/call.py
--rw-r--r--   0        0        0      817 2024-05-10 07:12:10.751895 getstream-1.0.0/getstream/video/client.py
--rw-r--r--   0        0        0    20586 2024-05-10 07:12:10.751895 getstream-1.0.0/getstream/video/rest_client.py
--rw-r--r--   0        0        0      696 2024-05-10 07:12:10.751895 getstream-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 getstream-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    14204 2024-05-13 12:18:46.349243 getstream-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     3708 2024-05-13 12:18:46.349243 getstream-1.0.1/README.md
+-rw-r--r--   0        0        0       50 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/__init__.py
+-rw-r--r--   0        0        0     6264 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/base.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/chat/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/chat/channel.py
+-rw-r--r--   0        0        0      267 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/chat/client.py
+-rw-r--r--   0        0        0    45004 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/chat/rest_client.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/common/__init__.py
+-rw-r--r--   0        0        0      275 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/common/client.py
+-rw-r--r--   0        0        0    23158 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/common/rest_client.py
+-rw-r--r--   0        0        0      925 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/config.py
+-rw-r--r--   0        0        0       46 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/generic.py
+-rw-r--r--   0        0        0      497 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/meta.py
+-rw-r--r--   0        0        0   298794 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/models/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/rate_limit.py
+-rw-r--r--   0        0        0     4489 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/stream.py
+-rw-r--r--   0        0        0     1024 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/stream_response.py
+-rw-r--r--   0        0        0     3942 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/utils.py
+-rw-r--r--   0        0        0       18 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/version.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/video/__init__.py
+-rw-r--r--   0        0        0    10156 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/video/call.py
+-rw-r--r--   0        0        0      817 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/video/client.py
+-rw-r--r--   0        0        0    18149 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/video/rest_client.py
+-rw-r--r--   0        0        0      696 2024-05-13 12:18:46.353243 getstream-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 getstream-1.0.1/PKG-INFO
```

### Comparing `getstream-1.0.0/LICENSE.md` & `getstream-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/README.md` & `getstream-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/getstream/base.py` & `getstream-1.0.1/getstream/base.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/getstream/chat/rest_client.py` & `getstream-1.0.1/getstream/chat/rest_client.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/getstream/common/rest_client.py` & `getstream-1.0.1/getstream/common/rest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,14 +236,96 @@
         return self.post("/api/v2/devices", Response, json=json)
 
     def export_users(self, user_ids: List[str]) -> StreamResponse[ExportUsersResponse]:
         json = build_body_dict(user_ids=user_ids)
 
         return self.post("/api/v2/export/users", ExportUsersResponse, json=json)
 
+    def list_external_storage(self) -> StreamResponse[ListExternalStorageResponse]:
+        return self.get("/api/v2/external_storage", ListExternalStorageResponse)
+
+    def create_external_storage(
+        self,
+        bucket: str,
+        name: str,
+        storage_type: str,
+        gcs_credentials: Optional[str] = None,
+        path: Optional[str] = None,
+        aws_s3: Optional[S3Request] = None,
+        azure_blob: Optional[AzureRequest] = None,
+    ) -> StreamResponse[CreateExternalStorageResponse]:
+        json = build_body_dict(
+            bucket=bucket,
+            name=name,
+            storage_type=storage_type,
+            gcs_credentials=gcs_credentials,
+            path=path,
+            aws_s3=aws_s3,
+            azure_blob=azure_blob,
+        )
+
+        return self.post(
+            "/api/v2/external_storage", CreateExternalStorageResponse, json=json
+        )
+
+    def delete_external_storage(
+        self, name: str
+    ) -> StreamResponse[DeleteExternalStorageResponse]:
+        path_params = {
+            "name": name,
+        }
+
+        return self.delete(
+            "/api/v2/external_storage/{name}",
+            DeleteExternalStorageResponse,
+            path_params=path_params,
+        )
+
+    def update_external_storage(
+        self,
+        name: str,
+        bucket: str,
+        storage_type: str,
+        gcs_credentials: Optional[str] = None,
+        path: Optional[str] = None,
+        aws_s3: Optional[S3Request] = None,
+        azure_blob: Optional[AzureRequest] = None,
+    ) -> StreamResponse[UpdateExternalStorageResponse]:
+        path_params = {
+            "name": name,
+        }
+        json = build_body_dict(
+            bucket=bucket,
+            storage_type=storage_type,
+            gcs_credentials=gcs_credentials,
+            path=path,
+            aws_s3=aws_s3,
+            azure_blob=azure_blob,
+        )
+
+        return self.put(
+            "/api/v2/external_storage/{name}",
+            UpdateExternalStorageResponse,
+            path_params=path_params,
+            json=json,
+        )
+
+    def check_external_storage(
+        self, name: str
+    ) -> StreamResponse[CheckExternalStorageResponse]:
+        path_params = {
+            "name": name,
+        }
+
+        return self.get(
+            "/api/v2/external_storage/{name}/check",
+            CheckExternalStorageResponse,
+            path_params=path_params,
+        )
+
     def create_guest(self, user: UserRequest) -> StreamResponse[CreateGuestResponse]:
         json = build_body_dict(user=user)
 
         return self.post("/api/v2/guest", CreateGuestResponse, json=json)
 
     def create_import_url(
         self, filename: Optional[str] = None
```

### Comparing `getstream-1.0.0/getstream/config.py` & `getstream-1.0.1/getstream/config.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/getstream/models/__init__.py` & `getstream-1.0.1/getstream/models/__init__.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/getstream/rate_limit.py` & `getstream-1.0.1/getstream/rate_limit.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/getstream/stream.py` & `getstream-1.0.1/getstream/stream.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/getstream/stream_response.py` & `getstream-1.0.1/getstream/stream_response.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/getstream/utils.py` & `getstream-1.0.1/getstream/utils.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/getstream/video/call.py` & `getstream-1.0.1/getstream/video/call.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/getstream/video/client.py` & `getstream-1.0.1/getstream/video/client.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.0/getstream/video/rest_client.py` & `getstream-1.0.1/getstream/video/rest_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -611,89 +611,7 @@
             UpdateCallTypeResponse,
             path_params=path_params,
             json=json,
         )
 
     def get_edges(self) -> StreamResponse[GetEdgesResponse]:
         return self.get("/api/v2/video/edges", GetEdgesResponse)
-
-    def list_external_storage(self) -> StreamResponse[ListExternalStorageResponse]:
-        return self.get("/api/v2/video/external_storage", ListExternalStorageResponse)
-
-    def create_external_storage(
-        self,
-        bucket: str,
-        name: str,
-        storage_type: str,
-        gcs_credentials: Optional[str] = None,
-        path: Optional[str] = None,
-        aws_s3: Optional[S3Request] = None,
-        azure_blob: Optional[AzureRequest] = None,
-    ) -> StreamResponse[CreateExternalStorageResponse]:
-        json = build_body_dict(
-            bucket=bucket,
-            name=name,
-            storage_type=storage_type,
-            gcs_credentials=gcs_credentials,
-            path=path,
-            aws_s3=aws_s3,
-            azure_blob=azure_blob,
-        )
-
-        return self.post(
-            "/api/v2/video/external_storage", CreateExternalStorageResponse, json=json
-        )
-
-    def delete_external_storage(
-        self, name: str
-    ) -> StreamResponse[DeleteExternalStorageResponse]:
-        path_params = {
-            "name": name,
-        }
-
-        return self.delete(
-            "/api/v2/video/external_storage/{name}",
-            DeleteExternalStorageResponse,
-            path_params=path_params,
-        )
-
-    def update_external_storage(
-        self,
-        name: str,
-        bucket: str,
-        storage_type: str,
-        gcs_credentials: Optional[str] = None,
-        path: Optional[str] = None,
-        aws_s3: Optional[S3Request] = None,
-        azure_blob: Optional[AzureRequest] = None,
-    ) -> StreamResponse[UpdateExternalStorageResponse]:
-        path_params = {
-            "name": name,
-        }
-        json = build_body_dict(
-            bucket=bucket,
-            storage_type=storage_type,
-            gcs_credentials=gcs_credentials,
-            path=path,
-            aws_s3=aws_s3,
-            azure_blob=azure_blob,
-        )
-
-        return self.put(
-            "/api/v2/video/external_storage/{name}",
-            UpdateExternalStorageResponse,
-            path_params=path_params,
-            json=json,
-        )
-
-    def check_external_storage(
-        self, name: str
-    ) -> StreamResponse[CheckExternalStorageResponse]:
-        path_params = {
-            "name": name,
-        }
-
-        return self.get(
-            "/api/v2/video/external_storage/{name}/check",
-            CheckExternalStorageResponse,
-            path_params=path_params,
-        )
```

### Comparing `getstream-1.0.0/pyproject.toml` & `getstream-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getstream"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = [
     "sachaarbonel <sacha.arbonel@hotmail.fr>",
     "tbarbugli <tbarbugli@gmail.com>"
 ]
 readme = "README.md"
```

### Comparing `getstream-1.0.0/PKG-INFO` & `getstream-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getstream
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: sachaarbonel
 Author-email: sacha.arbonel@hotmail.fr
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

