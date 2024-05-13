# Comparing `tmp/alibabacloud_linkedmall20230930-2.2.1.tar.gz` & `tmp/alibabacloud_linkedmall20230930-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_linkedmall20230930-2.2.1.tar", last modified: Tue May  7 05:58:35 2024, max compression
+gzip compressed data, was "dist/alibabacloud_linkedmall20230930-2.2.2.tar", last modified: Mon May 13 07:25:28 2024, max compression
```

## Comparing `alibabacloud_linkedmall20230930-2.2.1.tar` & `alibabacloud_linkedmall20230930-2.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/
--rw-r--r--   0 root         (0) root         (0)      662 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2450 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1123 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1208 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/__init__.py
--rw-r--r--   0 root         (0) root         (0)    83946 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/client.py
--rw-r--r--   0 root         (0) root         (0)   161626 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2450 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    83946 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930/client.py
+-rw-r--r--   0 root         (0) root         (0)   163099 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2024-05-13 07:25:28.000000 alibabacloud_linkedmall20230930-2.2.2/setup.py
```

### Comparing `alibabacloud_linkedmall20230930-2.2.1/ChangeLog.md` & `alibabacloud_linkedmall20230930-2.2.2/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-05-07 Version: 2.2.1
+- Generated python 2023-09-30 for linkedmall.
+
 2024-04-17 Version: 2.2.0
 - Support API SplitPurchaseOrder.
 
 
 2024-04-12 Version: 2.1.4
 - Generated python 2023-09-30 for linkedmall.
```

### Comparing `alibabacloud_linkedmall20230930-2.2.1/LICENSE` & `alibabacloud_linkedmall20230930-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.2.1/PKG-INFO` & `alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_linkedmall20230930
-Version: 2.2.1
+Name: alibabacloud-linkedmall20230930
+Version: 2.2.2
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930-2.2.1/README-CN.md` & `alibabacloud_linkedmall20230930-2.2.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.2.1/README.md` & `alibabacloud_linkedmall20230930-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/client.py` & `alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/models.py` & `alibabacloud_linkedmall20230930-2.2.2/alibabacloud_linkedmall20230930/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1623,14 +1623,47 @@
         if m.get('productList') is not None:
             for k in m.get('productList'):
                 temp_model = OrderProductResult()
                 self.product_list.append(temp_model.from_map(k))
         return self
 
 
+class ProductExtendProperty(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
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
+        if self.key is not None:
+            result['key'] = self.key
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('key') is not None:
+            self.key = m.get('key')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        return self
+
+
 class ProductSpecValue(TeaModel):
     def __init__(
         self,
         value: str = None,
         value_id: int = None,
     ):
         self.value = value
@@ -1921,14 +1954,15 @@
         self,
         brand_name: str = None,
         can_sell: bool = None,
         category_chain: List[Category] = None,
         category_leaf_id: int = None,
         desc_path: str = None,
         division_code: str = None,
+        extend_properties: List[ProductExtendProperty] = None,
         fuzzy_quantity: str = None,
         images: List[str] = None,
         pic_url: str = None,
         product_id: str = None,
         product_specs: List[ProductSpec] = None,
         product_status: str = None,
         product_type: str = None,
@@ -1944,14 +1978,15 @@
     ):
         self.brand_name = brand_name
         self.can_sell = can_sell
         self.category_chain = category_chain
         self.category_leaf_id = category_leaf_id
         self.desc_path = desc_path
         self.division_code = division_code
+        self.extend_properties = extend_properties
         self.fuzzy_quantity = fuzzy_quantity
         self.images = images
         self.pic_url = pic_url
         self.product_id = product_id
         self.product_specs = product_specs
         self.product_status = product_status
         self.product_type = product_type
@@ -1966,14 +2001,18 @@
         self.title = title
 
     def validate(self):
         if self.category_chain:
             for k in self.category_chain:
                 if k:
                     k.validate()
+        if self.extend_properties:
+            for k in self.extend_properties:
+                if k:
+                    k.validate()
         if self.product_specs:
             for k in self.product_specs:
                 if k:
                     k.validate()
         if self.properties:
             for k in self.properties:
                 if k:
@@ -1999,14 +2038,18 @@
                 result['categoryChain'].append(k.to_map() if k else None)
         if self.category_leaf_id is not None:
             result['categoryLeafId'] = self.category_leaf_id
         if self.desc_path is not None:
             result['descPath'] = self.desc_path
         if self.division_code is not None:
             result['divisionCode'] = self.division_code
+        result['extendProperties'] = []
+        if self.extend_properties is not None:
+            for k in self.extend_properties:
+                result['extendProperties'].append(k.to_map() if k else None)
         if self.fuzzy_quantity is not None:
             result['fuzzyQuantity'] = self.fuzzy_quantity
         if self.images is not None:
             result['images'] = self.images
         if self.pic_url is not None:
             result['picUrl'] = self.pic_url
         if self.product_id is not None:
@@ -2056,14 +2099,19 @@
                 self.category_chain.append(temp_model.from_map(k))
         if m.get('categoryLeafId') is not None:
             self.category_leaf_id = m.get('categoryLeafId')
         if m.get('descPath') is not None:
             self.desc_path = m.get('descPath')
         if m.get('divisionCode') is not None:
             self.division_code = m.get('divisionCode')
+        self.extend_properties = []
+        if m.get('extendProperties') is not None:
+            for k in m.get('extendProperties'):
+                temp_model = ProductExtendProperty()
+                self.extend_properties.append(temp_model.from_map(k))
         if m.get('fuzzyQuantity') is not None:
             self.fuzzy_quantity = m.get('fuzzyQuantity')
         if m.get('images') is not None:
             self.images = m.get('images')
         if m.get('picUrl') is not None:
             self.pic_url = m.get('picUrl')
         if m.get('productId') is not None:
```

### Comparing `alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/PKG-INFO` & `alibabacloud_linkedmall20230930-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-linkedmall20230930
-Version: 2.2.1
+Name: alibabacloud_linkedmall20230930
+Version: 2.2.2
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930-2.2.1/setup.py` & `alibabacloud_linkedmall20230930-2.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_linkedmall20230930.
 
-Created on 07/05/2024
+Created on 13/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_linkedmall20230930"
 NAME = "alibabacloud_linkedmall20230930" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud linkedmall (20230930) SDK Library for Python"
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

