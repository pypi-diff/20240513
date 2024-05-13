# Comparing `tmp/alibabacloud_aimiaobi20230801-1.4.0.tar.gz` & `tmp/alibabacloud_aimiaobi20230801-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aimiaobi20230801-1.4.0.tar", last modified: Tue Mar 12 17:14:30 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aimiaobi20230801-1.5.0.tar", last modified: Mon May 13 17:15:09 2024, max compression
```

## Comparing `alibabacloud_aimiaobi20230801-1.4.0.tar` & `alibabacloud_aimiaobi20230801-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/
--rw-r--r--   0 root         (0) root         (0)      497 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   167894 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801/client.py
--rw-r--r--   0 root         (0) root         (0)   357678 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-03-12 17:14:30.000000 alibabacloud_aimiaobi20230801-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1187 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   224740 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801/client.py
+-rw-r--r--   0 root         (0) root         (0)   387261 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/setup.py
```

### Comparing `alibabacloud_aimiaobi20230801-1.4.0/LICENSE` & `alibabacloud_aimiaobi20230801-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aimiaobi20230801-1.4.0/PKG-INFO` & `alibabacloud_aimiaobi20230801-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aimiaobi20230801
-Version: 1.4.0
+Version: 1.5.0
 Summary: Alibaba Cloud AiMiaoBi (20230801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aimiaobi20230801-1.4.0/README-CN.md` & `alibabacloud_aimiaobi20230801-1.5.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aimiaobi20230801-1.4.0/README.md` & `alibabacloud_aimiaobi20230801-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801/models.py` & `alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 class CancelAsyncTaskRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -136,14 +137,15 @@
 
 
 class ClearIntervenesRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -304,21 +306,25 @@
         content_text: str = None,
         keywords: List[str] = None,
         prompt: str = None,
         task_id: str = None,
         title: str = None,
         uuid: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.content = content
         self.content_domain = content_domain
         self.content_text = content_text
         self.keywords = keywords
         self.prompt = prompt
+        # This parameter is required.
         self.task_id = task_id
+        # This parameter is required.
         self.title = title
         self.uuid = uuid
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -379,21 +385,25 @@
         content_text: str = None,
         keywords_shrink: str = None,
         prompt: str = None,
         task_id: str = None,
         title: str = None,
         uuid: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.content = content
         self.content_domain = content_domain
         self.content_text = content_text
         self.keywords_shrink = keywords_shrink
         self.prompt = prompt
+        # This parameter is required.
         self.task_id = task_id
+        # This parameter is required.
         self.title = title
         self.uuid = uuid
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -544,14 +554,15 @@
 
 
 class CreateTokenRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -699,21 +710,162 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateTokenResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteCustomTextRequest(TeaModel):
+    def __init__(
+        self,
+        agent_key: str = None,
+        commodity_code: str = None,
+        id: int = None,
+    ):
+        # This parameter is required.
+        self.agent_key = agent_key
+        self.commodity_code = commodity_code
+        # This parameter is required.
+        self.id = id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.agent_key is not None:
+            result['AgentKey'] = self.agent_key
+        if self.commodity_code is not None:
+            result['CommodityCode'] = self.commodity_code
+        if self.id is not None:
+            result['Id'] = self.id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AgentKey') is not None:
+            self.agent_key = m.get('AgentKey')
+        if m.get('CommodityCode') is not None:
+            self.commodity_code = m.get('CommodityCode')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        return self
+
+
+class DeleteCustomTextResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: bool = None,
+        http_status_code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.http_status_code = http_status_code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.http_status_code is not None:
+            result['HttpStatusCode'] = self.http_status_code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('HttpStatusCode') is not None:
+            self.http_status_code = m.get('HttpStatusCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DeleteCustomTextResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteCustomTextResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteCustomTextResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteGeneratedContentRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         id: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.id = id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -836,14 +988,15 @@
 
 class DeleteInterveneRuleRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         rule_id: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.rule_id = rule_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1002,15 +1155,17 @@
 
 class DeleteMaterialByIdRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         id: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.id = id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1133,15 +1288,17 @@
 
 class ExportGeneratedContentRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         id: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.id = id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1263,14 +1420,15 @@
 
 
 class ExportIntervenesRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1424,20 +1582,22 @@
         good_text: str = None,
         modified_response: str = None,
         rating: str = None,
         rating_tags: List[str] = None,
         session_id: str = None,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.customer_response = customer_response
         self.good_text = good_text
         self.modified_response = modified_response
         self.rating = rating
         self.rating_tags = rating_tags
+        # This parameter is required.
         self.session_id = session_id
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1493,20 +1653,22 @@
         good_text: str = None,
         modified_response: str = None,
         rating: str = None,
         rating_tags_shrink: str = None,
         session_id: str = None,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.customer_response = customer_response
         self.good_text = good_text
         self.modified_response = modified_response
         self.rating = rating
         self.rating_tags_shrink = rating_tags_shrink
+        # This parameter is required.
         self.session_id = session_id
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1649,16 +1811,19 @@
 class FetchImageTaskRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         article_task_id: str = None,
         task_id_list: List[str] = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.article_task_id = article_task_id
+        # This parameter is required.
         self.task_id_list = task_id_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1688,16 +1853,19 @@
 class FetchImageTaskShrinkRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         article_task_id: str = None,
         task_id_list_shrink: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.article_task_id = article_task_id
+        # This parameter is required.
         self.task_id_list_shrink = task_id_list_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1954,14 +2122,15 @@
 class GenerateFileUrlByKeyRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         file_key: str = None,
         file_name: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.file_key = file_key
         self.file_name = file_name
 
     def validate(self):
         pass
 
@@ -2092,15 +2261,17 @@
     def __init__(
         self,
         content: str = None,
         id: int = None,
         task_id: str = None,
         task_status: str = None,
     ):
+        # This parameter is required.
         self.content = content
+        # This parameter is required.
         self.id = id
         self.task_id = task_id
         self.task_status = task_status
 
     def validate(self):
         pass
 
@@ -2138,18 +2309,23 @@
         self,
         agent_key: str = None,
         article_task_id: str = None,
         paragraph_list: List[GenerateImageTaskRequestParagraphList] = None,
         size: str = None,
         style: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.article_task_id = article_task_id
+        # This parameter is required.
         self.paragraph_list = paragraph_list
+        # This parameter is required.
         self.size = size
+        # This parameter is required.
         self.style = style
 
     def validate(self):
         if self.paragraph_list:
             for k in self.paragraph_list:
                 if k:
                     k.validate()
@@ -2197,18 +2373,23 @@
         self,
         agent_key: str = None,
         article_task_id: str = None,
         paragraph_list_shrink: str = None,
         size: str = None,
         style: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.article_task_id = article_task_id
+        # This parameter is required.
         self.paragraph_list_shrink = paragraph_list_shrink
+        # This parameter is required.
         self.size = size
+        # This parameter is required.
         self.style = style
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2426,16 +2607,18 @@
 class GenerateUploadConfigRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         file_name: str = None,
         parent_dir: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.file_name = file_name
+        # This parameter is required.
         self.parent_dir = parent_dir
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2630,14 +2813,15 @@
 
 class GenerateViewPointRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         reference_data: GenerateViewPointRequestReferenceData = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.reference_data = reference_data
 
     def validate(self):
         if self.reference_data:
             self.reference_data.validate()
 
@@ -2665,14 +2849,15 @@
 
 class GenerateViewPointShrinkRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         reference_data_shrink: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.reference_data_shrink = reference_data_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2825,21 +3010,227 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GenerateViewPointResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetCustomTextRequest(TeaModel):
+    def __init__(
+        self,
+        agent_key: str = None,
+        commodity_code: str = None,
+        id: int = None,
+    ):
+        # This parameter is required.
+        self.agent_key = agent_key
+        self.commodity_code = commodity_code
+        # This parameter is required.
+        self.id = id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.agent_key is not None:
+            result['AgentKey'] = self.agent_key
+        if self.commodity_code is not None:
+            result['CommodityCode'] = self.commodity_code
+        if self.id is not None:
+            result['Id'] = self.id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AgentKey') is not None:
+            self.agent_key = m.get('AgentKey')
+        if m.get('CommodityCode') is not None:
+            self.commodity_code = m.get('CommodityCode')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        return self
+
+
+class GetCustomTextResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        content: str = None,
+        create_time: str = None,
+        create_user: str = None,
+        id: int = None,
+        title: str = None,
+        update_time: str = None,
+        update_user: str = None,
+    ):
+        self.content = content
+        self.create_time = create_time
+        self.create_user = create_user
+        self.id = id
+        self.title = title
+        self.update_time = update_time
+        self.update_user = update_user
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.create_user is not None:
+            result['CreateUser'] = self.create_user
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.title is not None:
+            result['Title'] = self.title
+        if self.update_time is not None:
+            result['UpdateTime'] = self.update_time
+        if self.update_user is not None:
+            result['UpdateUser'] = self.update_user
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('CreateUser') is not None:
+            self.create_user = m.get('CreateUser')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        if m.get('UpdateTime') is not None:
+            self.update_time = m.get('UpdateTime')
+        if m.get('UpdateUser') is not None:
+            self.update_user = m.get('UpdateUser')
+        return self
+
+
+class GetCustomTextResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: GetCustomTextResponseBodyData = None,
+        http_status_code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.http_status_code = http_status_code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.http_status_code is not None:
+            result['HttpStatusCode'] = self.http_status_code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetCustomTextResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('HttpStatusCode') is not None:
+            self.http_status_code = m.get('HttpStatusCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetCustomTextResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetCustomTextResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetCustomTextResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetDataSourceOrderConfigRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         product_code: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.product_code = product_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3044,15 +3435,17 @@
 
 class GetGeneratedContentRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         id: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.id = id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3287,14 +3680,15 @@
 
 
 class GetInterveneGlobalReplyRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3483,14 +3877,15 @@
 
 class GetInterveneImportTaskInfoRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3696,14 +4091,15 @@
 
 class GetInterveneRuleDetailRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         rule_id: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.rule_id = rule_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4003,14 +4399,15 @@
 
 
 class GetInterveneTemplateFileUrlRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4158,15 +4555,17 @@
 
 class GetMaterialByIdRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         id: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.id = id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4425,14 +4824,15 @@
 
 
 class GetPropertiesRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5035,14 +5435,15 @@
     def __init__(
         self,
         agent_key: str = None,
         doc_name: str = None,
         file_key: str = None,
         file_url: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.doc_name = doc_name
         self.file_key = file_key
         self.file_url = file_url
 
     def validate(self):
         pass
@@ -5213,14 +5614,15 @@
     def __init__(
         self,
         agent_key: str = None,
         doc_name: str = None,
         file_key: str = None,
         file_url: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.doc_name = doc_name
         self.file_key = file_key
         self.file_url = file_url
 
     def validate(self):
         pass
@@ -5422,14 +5824,15 @@
 
 class InsertInterveneGlobalReplyRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         reply_messag_list: List[InsertInterveneGlobalReplyRequestReplyMessagList] = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.reply_messag_list = reply_messag_list
 
     def validate(self):
         if self.reply_messag_list:
             for k in self.reply_messag_list:
                 if k:
@@ -5463,14 +5866,15 @@
 
 class InsertInterveneGlobalReplyShrinkRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         reply_messag_list_shrink: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.reply_messag_list_shrink = reply_messag_list_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5830,14 +6234,15 @@
 
 class InsertInterveneRuleRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         intervene_rule_config: InsertInterveneRuleRequestInterveneRuleConfig = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.intervene_rule_config = intervene_rule_config
 
     def validate(self):
         if self.intervene_rule_config:
             self.intervene_rule_config.validate()
 
@@ -5865,14 +6270,15 @@
 
 class InsertInterveneRuleShrinkRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         intervene_rule_config_shrink: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.intervene_rule_config_shrink = intervene_rule_config_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6034,14 +6440,15 @@
         task_code: str = None,
         task_name: str = None,
         task_status: int = None,
         task_status_list: List[int] = None,
         task_type: str = None,
         task_type_list: List[str] = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.create_time_end = create_time_end
         self.create_time_start = create_time_start
         self.current = current
         self.size = size
         self.task_code = task_code
         self.task_name = task_name
@@ -6121,14 +6528,15 @@
         task_code: str = None,
         task_name: str = None,
         task_status: int = None,
         task_status_list_shrink: str = None,
         task_type: str = None,
         task_type_list_shrink: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.create_time_end = create_time_end
         self.create_time_start = create_time_start
         self.current = current
         self.size = size
         self.task_code = task_code
         self.task_name = task_name
@@ -6470,14 +6878,15 @@
 
 class ListBuildConfigsRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         type: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6725,25 +7134,229 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListBuildConfigsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListCustomTextRequest(TeaModel):
+    def __init__(
+        self,
+        agent_key: str = None,
+        commodity_code: str = None,
+    ):
+        # This parameter is required.
+        self.agent_key = agent_key
+        self.commodity_code = commodity_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.agent_key is not None:
+            result['AgentKey'] = self.agent_key
+        if self.commodity_code is not None:
+            result['CommodityCode'] = self.commodity_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AgentKey') is not None:
+            self.agent_key = m.get('AgentKey')
+        if m.get('CommodityCode') is not None:
+            self.commodity_code = m.get('CommodityCode')
+        return self
+
+
+class ListCustomTextResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        content: str = None,
+        create_time: str = None,
+        create_user: str = None,
+        id: int = None,
+        title: str = None,
+        update_time: str = None,
+        update_user: str = None,
+    ):
+        self.content = content
+        self.create_time = create_time
+        self.create_user = create_user
+        self.id = id
+        self.title = title
+        self.update_time = update_time
+        self.update_user = update_user
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.create_user is not None:
+            result['CreateUser'] = self.create_user
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.title is not None:
+            result['Title'] = self.title
+        if self.update_time is not None:
+            result['UpdateTime'] = self.update_time
+        if self.update_user is not None:
+            result['UpdateUser'] = self.update_user
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('CreateUser') is not None:
+            self.create_user = m.get('CreateUser')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        if m.get('UpdateTime') is not None:
+            self.update_time = m.get('UpdateTime')
+        if m.get('UpdateUser') is not None:
+            self.update_user = m.get('UpdateUser')
+        return self
+
+
+class ListCustomTextResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: List[ListCustomTextResponseBodyData] = None,
+        http_status_code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.http_status_code = http_status_code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.http_status_code is not None:
+            result['HttpStatusCode'] = self.http_status_code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = ListCustomTextResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('HttpStatusCode') is not None:
+            self.http_status_code = m.get('HttpStatusCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class ListCustomTextResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListCustomTextResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListCustomTextResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListDialoguesRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         current: int = None,
         dialogue_type: int = None,
         end_time: str = None,
         size: int = None,
         start_time: str = None,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.current = current
         self.dialogue_type = dialogue_type
         self.end_time = end_time
         self.size = size
         self.start_time = start_time
         self.task_id = task_id
@@ -6980,14 +7593,15 @@
         content_domain: str = None,
         current: int = None,
         end_time: str = None,
         size: int = None,
         start_time: str = None,
         title: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.content_domain = content_domain
         self.current = current
         self.end_time = end_time
         self.size = size
         self.start_time = start_time
         self.title = title
@@ -7276,14 +7890,15 @@
         self,
         agent_key: str = None,
         current: int = None,
         news_type: str = None,
         news_types: List[str] = None,
         size: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.current = current
         self.news_type = news_type
         self.news_types = news_types
         self.size = size
 
     def validate(self):
@@ -7327,14 +7942,15 @@
         self,
         agent_key: str = None,
         current: int = None,
         news_type: str = None,
         news_types_shrink: str = None,
         size: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.current = current
         self.news_type = news_type
         self.news_types_shrink = news_types_shrink
         self.size = size
 
     def validate(self):
@@ -7634,14 +8250,15 @@
 class ListInterveneCntRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         page_index: int = None,
         page_size: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.page_index = page_index
         self.page_size = page_size
 
     def validate(self):
         pass
 
@@ -7818,14 +8435,15 @@
 class ListInterveneImportTasksRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         page_index: int = None,
         page_size: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.page_index = page_index
         self.page_size = page_size
 
     def validate(self):
         pass
 
@@ -8061,14 +8679,15 @@
 class ListInterveneRulesRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         page_index: int = None,
         page_size: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.page_index = page_index
         self.page_size = page_size
 
     def validate(self):
         pass
 
@@ -8366,14 +8985,15 @@
         agent_key: str = None,
         intervene_type: int = None,
         page_index: int = None,
         page_size: int = None,
         query: str = None,
         rule_id: int = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.intervene_type = intervene_type
         self.page_index = page_index
         self.page_size = page_size
         self.query = query
         self.rule_id = rule_id
 
@@ -8620,14 +9240,15 @@
         query: str = None,
         share_attr: int = None,
         size: int = None,
         title: str = None,
         update_time_end: str = None,
         update_time_start: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.content = content
         self.create_time_end = create_time_end
         self.create_time_start = create_time_start
         self.current = current
         self.doc_type = doc_type
         self.doc_type_list = doc_type_list
@@ -8737,14 +9358,15 @@
         query: str = None,
         share_attr: int = None,
         size: int = None,
         title: str = None,
         update_time_end: str = None,
         update_time_start: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.content = content
         self.create_time_end = create_time_end
         self.create_time_start = create_time_start
         self.current = current
         self.doc_type = doc_type
         self.doc_type_list_shrink = doc_type_list_shrink
@@ -9110,14 +9732,15 @@
 
 
 class ListVersionsRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9337,14 +9960,15 @@
 
 class QueryAsyncTaskRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -9569,25 +10193,172 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryAsyncTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SaveCustomTextRequest(TeaModel):
+    def __init__(
+        self,
+        agent_key: str = None,
+        commodity_code: str = None,
+        content: str = None,
+        title: str = None,
+    ):
+        # This parameter is required.
+        self.agent_key = agent_key
+        self.commodity_code = commodity_code
+        self.content = content
+        self.title = title
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.agent_key is not None:
+            result['AgentKey'] = self.agent_key
+        if self.commodity_code is not None:
+            result['CommodityCode'] = self.commodity_code
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.title is not None:
+            result['Title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AgentKey') is not None:
+            self.agent_key = m.get('AgentKey')
+        if m.get('CommodityCode') is not None:
+            self.commodity_code = m.get('CommodityCode')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        return self
+
+
+class SaveCustomTextResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: int = None,
+        http_status_code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.http_status_code = http_status_code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.http_status_code is not None:
+            result['HttpStatusCode'] = self.http_status_code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('HttpStatusCode') is not None:
+            self.http_status_code = m.get('HttpStatusCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class SaveCustomTextResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SaveCustomTextResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SaveCustomTextResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SaveDataSourceOrderConfigRequestUserConfigDataSourceList(TeaModel):
     def __init__(
         self,
         code: str = None,
         name: str = None,
         number: int = None,
         type: str = None,
     ):
+        # This parameter is required.
         self.code = code
         self.name = name
+        # This parameter is required.
         self.number = number
+        # This parameter is required.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9621,16 +10392,19 @@
 class SaveDataSourceOrderConfigRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         product_code: str = None,
         user_config_data_source_list: List[SaveDataSourceOrderConfigRequestUserConfigDataSourceList] = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.product_code = product_code
+        # This parameter is required.
         self.user_config_data_source_list = user_config_data_source_list
 
     def validate(self):
         if self.user_config_data_source_list:
             for k in self.user_config_data_source_list:
                 if k:
                     k.validate()
@@ -9668,16 +10442,19 @@
 class SaveDataSourceOrderConfigShrinkRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         product_code: str = None,
         user_config_data_source_list_shrink: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.product_code = product_code
+        # This parameter is required.
         self.user_config_data_source_list_shrink = user_config_data_source_list_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9816,18 +10593,20 @@
         share_attr: int = None,
         src_from: str = None,
         summary: str = None,
         text_content: str = None,
         title: str = None,
         url: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.author = author
         self.both_save_private_and_share = both_save_private_and_share
         self.doc_keywords = doc_keywords
+        # This parameter is required.
         self.doc_type = doc_type
         self.external_url = external_url
         self.html_content = html_content
         self.pub_time = pub_time
         self.share_attr = share_attr
         self.src_from = src_from
         self.summary = summary
@@ -9921,18 +10700,20 @@
         share_attr: int = None,
         src_from: str = None,
         summary: str = None,
         text_content: str = None,
         title: str = None,
         url: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.author = author
         self.both_save_private_and_share = both_save_private_and_share
         self.doc_keywords_shrink = doc_keywords_shrink
+        # This parameter is required.
         self.doc_type = doc_type
         self.external_url = external_url
         self.html_content = html_content
         self.pub_time = pub_time
         self.share_attr = share_attr
         self.src_from = src_from
         self.summary = summary
@@ -10117,14 +10898,15 @@
         filter_not_null: bool = None,
         include_content: bool = None,
         page: int = None,
         page_size: int = None,
         query: str = None,
         search_sources: List[str] = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.filter_not_null = filter_not_null
         self.include_content = include_content
         self.page = page
         self.page_size = page_size
         self.query = query
         self.search_sources = search_sources
@@ -10180,14 +10962,15 @@
         filter_not_null: bool = None,
         include_content: bool = None,
         page: int = None,
         page_size: int = None,
         query: str = None,
         search_sources_shrink: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.filter_not_null = filter_not_null
         self.include_content = include_content
         self.page = page
         self.page_size = page_size
         self.query = query
         self.search_sources_shrink = search_sources_shrink
@@ -10464,15 +11247,17 @@
         self,
         agent_key: str = None,
         task_code: str = None,
         task_execute_time: str = None,
         task_name: str = None,
         task_param: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
+        # This parameter is required.
         self.task_code = task_code
         self.task_execute_time = task_execute_time
         self.task_name = task_name
         self.task_param = task_param
 
     def validate(self):
         pass
@@ -10645,28 +11430,181 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SubmitAsyncTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateCustomTextRequest(TeaModel):
+    def __init__(
+        self,
+        agent_key: str = None,
+        commodity_code: str = None,
+        content: str = None,
+        id: int = None,
+        title: str = None,
+    ):
+        # This parameter is required.
+        self.agent_key = agent_key
+        self.commodity_code = commodity_code
+        self.content = content
+        # This parameter is required.
+        self.id = id
+        self.title = title
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.agent_key is not None:
+            result['AgentKey'] = self.agent_key
+        if self.commodity_code is not None:
+            result['CommodityCode'] = self.commodity_code
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.title is not None:
+            result['Title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AgentKey') is not None:
+            self.agent_key = m.get('AgentKey')
+        if m.get('CommodityCode') is not None:
+            self.commodity_code = m.get('CommodityCode')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        return self
+
+
+class UpdateCustomTextResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: int = None,
+        http_status_code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.http_status_code = http_status_code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.http_status_code is not None:
+            result['HttpStatusCode'] = self.http_status_code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('HttpStatusCode') is not None:
+            self.http_status_code = m.get('HttpStatusCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class UpdateCustomTextResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateCustomTextResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateCustomTextResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateGeneratedContentRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         content: str = None,
         content_text: str = None,
         id: int = None,
         keywords: List[str] = None,
         prompt: str = None,
         title: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.content = content
         self.content_text = content_text
+        # This parameter is required.
         self.id = id
         self.keywords = keywords
         self.prompt = prompt
         self.title = title
 
     def validate(self):
         pass
@@ -10719,17 +11657,19 @@
         content: str = None,
         content_text: str = None,
         id: int = None,
         keywords_shrink: str = None,
         prompt: str = None,
         title: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.content = content
         self.content_text = content_text
+        # This parameter is required.
         self.id = id
         self.keywords_shrink = keywords_shrink
         self.prompt = prompt
         self.title = title
 
     def validate(self):
         pass
@@ -10887,20 +11827,23 @@
         share_attr: int = None,
         src_from: str = None,
         summary: str = None,
         text_content: str = None,
         title: str = None,
         url: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.author = author
         self.doc_keywords = doc_keywords
+        # This parameter is required.
         self.doc_type = doc_type
         self.external_url = external_url
         self.html_content = html_content
+        # This parameter is required.
         self.id = id
         self.pub_time = pub_time
         self.share_attr = share_attr
         self.src_from = src_from
         self.summary = summary
         self.text_content = text_content
         self.title = title
@@ -10992,20 +11935,23 @@
         share_attr: int = None,
         src_from: str = None,
         summary: str = None,
         text_content: str = None,
         title: str = None,
         url: str = None,
     ):
+        # This parameter is required.
         self.agent_key = agent_key
         self.author = author
         self.doc_keywords_shrink = doc_keywords_shrink
+        # This parameter is required.
         self.doc_type = doc_type
         self.external_url = external_url
         self.html_content = html_content
+        # This parameter is required.
         self.id = id
         self.pub_time = pub_time
         self.share_attr = share_attr
         self.src_from = src_from
         self.summary = summary
         self.text_content = text_content
         self.title = title
```

### Comparing `alibabacloud_aimiaobi20230801-1.4.0/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO` & `alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aimiaobi20230801
-Version: 1.4.0
+Version: 1.5.0
 Summary: Alibaba Cloud AiMiaoBi (20230801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aimiaobi20230801-1.4.0/setup.py` & `alibabacloud_aimiaobi20230801-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aimiaobi20230801.
 
-Created on 12/03/2024
+Created on 13/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aimiaobi20230801"
 NAME = "alibabacloud_aimiaobi20230801" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AiMiaoBi (20230801) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

