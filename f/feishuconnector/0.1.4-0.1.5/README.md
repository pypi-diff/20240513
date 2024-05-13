# Comparing `tmp/feishuconnector-0.1.4.tar.gz` & `tmp/feishuconnector-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/feishuconnector-0.1.4.tar", last modified: Mon May 16 06:58:44 2022, max compression
+gzip compressed data, was "dist/feishuconnector-0.1.5.tar", last modified: Mon May 13 08:05:50 2024, max compression
```

## Comparing `feishuconnector-0.1.4.tar` & `feishuconnector-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 cjiang     (501) staff       (20)        0 2022-05-16 06:58:44.000000 feishuconnector-0.1.4/
--rw-r--r--   0 cjiang     (501) staff       (20)     1089 2022-01-30 23:46:40.000000 feishuconnector-0.1.4/LICENSE
--rw-r--r--   0 cjiang     (501) staff       (20)     1761 2022-05-16 06:58:44.000000 feishuconnector-0.1.4/PKG-INFO
--rw-r--r--   0 cjiang     (501) staff       (20)     1119 2022-02-09 12:06:39.000000 feishuconnector-0.1.4/README.rst
-drwxr-xr-x   0 cjiang     (501) staff       (20)        0 2022-05-16 06:58:44.000000 feishuconnector-0.1.4/feishuconnector/
--rw-r--r--   0 cjiang     (501) staff       (20)       70 2022-01-31 00:39:54.000000 feishuconnector-0.1.4/feishuconnector/__init__.py
--rw-r--r--   0 cjiang     (501) staff       (20)       22 2022-05-16 06:58:25.000000 feishuconnector-0.1.4/feishuconnector/_version.py
--rw-r--r--   0 cjiang     (501) staff       (20)      442 2022-02-11 10:19:01.000000 feishuconnector-0.1.4/feishuconnector/encoder.py
--rw-r--r--   0 cjiang     (501) staff       (20)    14946 2022-05-13 07:20:27.000000 feishuconnector-0.1.4/feishuconnector/manager.py
-drwxr-xr-x   0 cjiang     (501) staff       (20)        0 2022-05-16 06:58:44.000000 feishuconnector-0.1.4/feishuconnector.egg-info/
--rw-r--r--   0 cjiang     (501) staff       (20)     1761 2022-05-16 06:58:44.000000 feishuconnector-0.1.4/feishuconnector.egg-info/PKG-INFO
--rw-r--r--   0 cjiang     (501) staff       (20)      331 2022-05-16 06:58:44.000000 feishuconnector-0.1.4/feishuconnector.egg-info/SOURCES.txt
--rw-r--r--   0 cjiang     (501) staff       (20)        1 2022-05-16 06:58:44.000000 feishuconnector-0.1.4/feishuconnector.egg-info/dependency_links.txt
--rw-r--r--   0 cjiang     (501) staff       (20)       96 2022-05-16 06:58:44.000000 feishuconnector-0.1.4/feishuconnector.egg-info/requires.txt
--rw-r--r--   0 cjiang     (501) staff       (20)       16 2022-05-16 06:58:44.000000 feishuconnector-0.1.4/feishuconnector.egg-info/top_level.txt
--rw-r--r--   0 cjiang     (501) staff       (20)       38 2022-05-16 06:58:44.000000 feishuconnector-0.1.4/setup.cfg
--rw-r--r--   0 cjiang     (501) staff       (20)     1193 2022-05-16 06:58:25.000000 feishuconnector-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:05:50.955038 feishuconnector-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)      268 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-05-13 08:05:50.955038 feishuconnector-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:05:50.954038 feishuconnector-0.1.5/feishuconnector/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/feishuconnector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-13 08:05:21.000000 feishuconnector-0.1.5/feishuconnector/_version.py
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/feishuconnector/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    16808 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/feishuconnector/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:05:50.955038 feishuconnector-0.1.5/feishuconnector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-05-13 08:05:50.000000 feishuconnector-0.1.5/feishuconnector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-13 08:05:50.000000 feishuconnector-0.1.5/feishuconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 08:05:50.000000 feishuconnector-0.1.5/feishuconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-13 08:05:50.000000 feishuconnector-0.1.5/feishuconnector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-13 08:05:50.000000 feishuconnector-0.1.5/feishuconnector.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 08:05:50.955038 feishuconnector-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1193 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:05:50.955038 feishuconnector-0.1.5/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/test/run.py
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/upload.sh
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `feishuconnector-0.1.4/LICENSE` & `feishuconnector-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `feishuconnector-0.1.4/PKG-INFO` & `feishuconnector-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feishuconnector
-Version: 0.1.4
+Version: 0.1.5
 Summary: connect feishu content franchise
 Home-page: http://www.puyuan.tech
 Author: Changhao Jiang
 Author-email: jch@puyuan.tech
 License: MIT License
 Platform: all
 Classifier: Development Status :: 4 - Beta
@@ -49,8 +49,7 @@
     fc.insert_bitable_records('wikcnlBvPJ8xoTSfVtQwGBkrUWc', 'tblGZPQYMzrwRMeo', records)
 
     # 获取普通表格某range的全部数据，values is a list(rows) of list(cols)
     values = fc.get_sheet_data("wikcnQgBgZCWUx7w6ZpzzLXX3bc", "e792af")
     
     # 在普通表格中追加数据
     fc.append_sheet_data("wikcnQgBgZCWUx7w6ZpzzLXX3bc", "e792af", values)
-
```

### Comparing `feishuconnector-0.1.4/README.rst` & `feishuconnector-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `feishuconnector-0.1.4/feishuconnector/manager.py` & `feishuconnector-0.1.5/feishuconnector/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 
+import uuid
 import requests
 import json
 import tempfile
 from .encoder import JsonEncoder
 from typing import BinaryIO, Dict
 
 import pandas as pd
 import dataframe_image as dfi
 from requests_toolbelt import MultipartEncoder
 
 
+def create_unique_record_id(prefix='rec'):
+    """Generate a unique record id for Feishu Bitable randomly."""
+    
+    return prefix + uuid.uuid4().hex[:10]
+
 class FeishuConnector:
 
     def __init__(self, webhooks: Dict[str, str]):
         self.app_id = None
         self.app_secret = None
         self.token = None
         self._webhooks = webhooks
@@ -97,14 +103,21 @@
             end = min(item_num, num_inserted + 100)
             rs = records[num_inserted: end]
             self._append_bitable_record(app_token, table_id, rs)
             num_inserted = end
             try_num += 1
         self.log(f'records to {node_token} table {table_id} with {try_num} requests. ItemNum={num_inserted}, RecordNum={item_num}')
         return num_inserted
+    
+    def append_bitable_df(self, node_token, table_id, df: pd.DataFrame):
+        d = self.get_node_detail(node_token)
+        app_token = d['obj_token']
+        self.log(f'[bitable] get from sheet: (node){node_token} (bi){app_token} (table){table_id}')
+        self._append_bitable_df(app_token, table_id, df)
+        self.log(f'data to {node_token} table {table_id} with 1 request. RecordNum={len(df)}')
 
     def get_sheet_data(self, node_token, sheet_id):
         app_token = self.get_app_token(node_token)
         values = self._get_sheet_data(app_token, sheet_id)
         sz = len(values)
         self.log(f'data from {node_token} sheet {sheet_id} with {sz} rows')
         return values
@@ -250,14 +263,43 @@
         dt = json.dumps({'records': ds})
         r = requests.post(f'https://open.feishu.cn/open-apis/bitable/v1/apps/{app_token}/tables/{table_id}/records/batch_create', data=dt, headers=headers)
         d = json.loads(r.text)
         sz = len(records)
         assert d.get('code') == 0, f'fail to _append_bitable_record={r.text}'
         self.log(f'bitable records inserted. (table_id){table_id} (num){sz}')
         return d['data']['records']
+    
+    def _append_bitable_df(self, app_token, table_id, df: pd.DataFrame):
+        
+        headers = {
+            'Authorization': f'Bearer {self.token}',
+            'Content-Type': 'application/json; charset=utf-8'
+        }
+        
+        # Convert timestamp data to int
+        timestamp_columns = df.select_dtypes(include='datetime').columns
+        for col in timestamp_columns:
+            df[col] = (df[col].astype(int) / 10**6).astype(int)
+        self.log(f'Timestamp columns: {timestamp_columns.tolist()}, converted to int')
+        
+        # Convert dataframe to format required by Feishu API
+        records = []
+        for _, row in df.iterrows():
+            records.append({
+                'record_id': create_unique_record_id(),
+                'fields': row.to_dict(),
+            })
+            
+        dt = json.dumps({'records': records}, indent=4)
+        r = requests.post(f'https://open.feishu.cn/open-apis/bitable/v1/apps/{app_token}/tables/{table_id}/records/batch_create', data=dt, headers=headers)
+        d = json.loads(r.text)
+        sz = len(records)
+        assert d.get('code') == 0, f'fail to _append_bitable_df={r.text}'
+        self.log(f'bitable records inserted. (table_id){table_id} (num){sz}')
+        return d['data']['records']
 
     def upload_images(self, image_binary: BinaryIO) -> str:
         import json
 
         form = {'image_type': 'message',
                 'image': (image_binary)}
         multi_form = MultipartEncoder(form)
```

### Comparing `feishuconnector-0.1.4/feishuconnector.egg-info/PKG-INFO` & `feishuconnector-0.1.5/feishuconnector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feishuconnector
-Version: 0.1.4
+Version: 0.1.5
 Summary: connect feishu content franchise
 Home-page: http://www.puyuan.tech
 Author: Changhao Jiang
 Author-email: jch@puyuan.tech
 License: MIT License
 Platform: all
 Classifier: Development Status :: 4 - Beta
@@ -49,8 +49,7 @@
     fc.insert_bitable_records('wikcnlBvPJ8xoTSfVtQwGBkrUWc', 'tblGZPQYMzrwRMeo', records)
 
     # 获取普通表格某range的全部数据，values is a list(rows) of list(cols)
     values = fc.get_sheet_data("wikcnQgBgZCWUx7w6ZpzzLXX3bc", "e792af")
     
     # 在普通表格中追加数据
     fc.append_sheet_data("wikcnQgBgZCWUx7w6ZpzzLXX3bc", "e792af", values)
-
```

### Comparing `feishuconnector-0.1.4/setup.py` & `feishuconnector-0.1.5/setup.py`

 * *Files identical despite different names*

