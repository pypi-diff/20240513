# Comparing `tmp/mm_sdk-0.1.378.tar.gz` & `tmp/mm_sdk-0.1.379.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mm_sdk-0.1.378.tar", max compression
+gzip compressed data, was "mm_sdk-0.1.379.tar", max compression
```

## Comparing `mm_sdk-0.1.378.tar` & `mm_sdk-0.1.379.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      943 2024-05-13 06:08:58.323801 mm_sdk-0.1.378/pyproject.toml
--rw-r--r--   0        0        0     1615 2023-10-11 20:26:52.000000 mm_sdk-0.1.378/sdk/__init__.py
--rw-r--r--   0        0        0     3260 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/admitad.py
--rw-r--r--   0        0        0     3235 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/analytics.py
--rw-r--r--   0        0        0      770 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/barcode_recognizer.py
--rw-r--r--   0        0        0      251 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/base.py
--rw-r--r--   0        0        0     3961 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/cash_register.py
--rw-r--r--   0        0        0      644 2023-10-11 20:26:52.000000 mm_sdk-0.1.378/sdk/click_again.py
--rw-r--r--   0        0        0     8565 2023-10-11 20:26:52.000000 mm_sdk-0.1.378/sdk/client.py
--rw-r--r--   0        0        0      714 2023-11-27 11:49:05.000000 mm_sdk-0.1.378/sdk/cryptopro.py
--rw-r--r--   0        0        0     2504 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/elk.py
--rw-r--r--   0        0        0     1661 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/face_detector.py
--rw-r--r--   0        0        0     4583 2024-05-13 06:04:00.000000 mm_sdk-0.1.378/sdk/gift.py
--rw-r--r--   0        0        0    20030 2024-05-13 06:04:00.000000 mm_sdk-0.1.378/sdk/gigtest.py
--rw-r--r--   0        0        0        0 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/mis/__init__.py
--rw-r--r--   0        0        0     3449 2023-11-27 11:49:05.000000 mm_sdk-0.1.378/sdk/mis/client.py
--rw-r--r--   0        0        0     3471 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/mis/crm.py
--rw-r--r--   0        0        0     3322 2023-10-11 20:26:52.000000 mm_sdk-0.1.378/sdk/mis/lab.py
--rw-r--r--   0        0        0     3630 2023-10-11 20:26:52.000000 mm_sdk-0.1.378/sdk/mis/lmk.py
--rw-r--r--   0        0        0     5188 2024-03-12 13:14:37.000000 mm_sdk-0.1.378/sdk/mis/mobil.py
--rw-r--r--   0        0        0      620 2023-11-27 11:49:05.000000 mm_sdk-0.1.378/sdk/mis/samd.py
--rw-r--r--   0        0        0     1295 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/mis/standalone.py
--rw-r--r--   0        0        0      577 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/mis/widgets.py
--rw-r--r--   0        0        0     4158 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/mobile_backend.py
--rw-r--r--   0        0        0      858 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/notemaster.py
--rw-r--r--   0        0        0     2878 2023-06-21 19:57:19.000000 mm_sdk-0.1.378/sdk/notification.py
--rw-r--r--   0        0        0     2607 2024-05-13 06:04:00.000000 mm_sdk-0.1.378/sdk/nsirosminzdrav.py
--rw-r--r--   0        0        0     5311 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/personal.py
--rw-r--r--   0        0        0    17080 2023-10-11 20:26:52.000000 mm_sdk-0.1.378/sdk/pre_record.py
--rw-r--r--   0        0        0     1740 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/prodoctorov.py
--rw-r--r--   0        0        0     1738 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/reestr.py
--rw-r--r--   0        0        0     1343 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/roistat.py
--rw-r--r--   0        0        0     4377 2024-05-13 06:04:00.000000 mm_sdk-0.1.378/sdk/samd.py
--rw-r--r--   0        0        0      961 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/site_mobilmed.py
--rw-r--r--   0        0        0      687 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/sms.py
--rw-r--r--   0        0        0        0 2023-10-11 20:26:52.000000 mm_sdk-0.1.378/sdk/utils/__init__.py
--rw-r--r--   0        0        0      511 2023-10-11 20:26:52.000000 mm_sdk-0.1.378/sdk/utils/django_request_id.py
--rw-r--r--   0        0        0     5349 2023-01-25 15:15:32.000000 mm_sdk-0.1.378/sdk/yandex_courier.py
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 mm_sdk-0.1.378/setup.py
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 mm_sdk-0.1.378/PKG-INFO
+-rw-r--r--   0        0        0      943 2024-05-13 06:46:06.999925 mm_sdk-0.1.379/pyproject.toml
+-rw-r--r--   0        0        0     1615 2023-10-11 20:26:52.000000 mm_sdk-0.1.379/sdk/__init__.py
+-rw-r--r--   0        0        0     3260 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/admitad.py
+-rw-r--r--   0        0        0     3235 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/analytics.py
+-rw-r--r--   0        0        0      770 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/barcode_recognizer.py
+-rw-r--r--   0        0        0      251 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/base.py
+-rw-r--r--   0        0        0     3961 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/cash_register.py
+-rw-r--r--   0        0        0      644 2023-10-11 20:26:52.000000 mm_sdk-0.1.379/sdk/click_again.py
+-rw-r--r--   0        0        0     8565 2023-10-11 20:26:52.000000 mm_sdk-0.1.379/sdk/client.py
+-rw-r--r--   0        0        0      714 2023-11-27 11:49:05.000000 mm_sdk-0.1.379/sdk/cryptopro.py
+-rw-r--r--   0        0        0     2504 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/elk.py
+-rw-r--r--   0        0        0     1661 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/face_detector.py
+-rw-r--r--   0        0        0     4970 2024-05-13 06:42:54.000000 mm_sdk-0.1.379/sdk/gift.py
+-rw-r--r--   0        0        0    20030 2024-05-13 06:04:00.000000 mm_sdk-0.1.379/sdk/gigtest.py
+-rw-r--r--   0        0        0        0 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/mis/__init__.py
+-rw-r--r--   0        0        0     3449 2023-11-27 11:49:05.000000 mm_sdk-0.1.379/sdk/mis/client.py
+-rw-r--r--   0        0        0     3471 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/mis/crm.py
+-rw-r--r--   0        0        0     3322 2023-10-11 20:26:52.000000 mm_sdk-0.1.379/sdk/mis/lab.py
+-rw-r--r--   0        0        0     3630 2023-10-11 20:26:52.000000 mm_sdk-0.1.379/sdk/mis/lmk.py
+-rw-r--r--   0        0        0     5188 2024-03-12 13:14:37.000000 mm_sdk-0.1.379/sdk/mis/mobil.py
+-rw-r--r--   0        0        0      620 2023-11-27 11:49:05.000000 mm_sdk-0.1.379/sdk/mis/samd.py
+-rw-r--r--   0        0        0     1295 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/mis/standalone.py
+-rw-r--r--   0        0        0      577 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/mis/widgets.py
+-rw-r--r--   0        0        0     4158 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/mobile_backend.py
+-rw-r--r--   0        0        0      858 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/notemaster.py
+-rw-r--r--   0        0        0     2878 2023-06-21 19:57:19.000000 mm_sdk-0.1.379/sdk/notification.py
+-rw-r--r--   0        0        0     2607 2024-05-13 06:04:00.000000 mm_sdk-0.1.379/sdk/nsirosminzdrav.py
+-rw-r--r--   0        0        0     5311 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/personal.py
+-rw-r--r--   0        0        0    17080 2023-10-11 20:26:52.000000 mm_sdk-0.1.379/sdk/pre_record.py
+-rw-r--r--   0        0        0     1740 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/prodoctorov.py
+-rw-r--r--   0        0        0     1738 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/reestr.py
+-rw-r--r--   0        0        0     1343 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/roistat.py
+-rw-r--r--   0        0        0     4377 2024-05-13 06:04:00.000000 mm_sdk-0.1.379/sdk/samd.py
+-rw-r--r--   0        0        0      961 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/site_mobilmed.py
+-rw-r--r--   0        0        0      687 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/sms.py
+-rw-r--r--   0        0        0        0 2023-10-11 20:26:52.000000 mm_sdk-0.1.379/sdk/utils/__init__.py
+-rw-r--r--   0        0        0      511 2023-10-11 20:26:52.000000 mm_sdk-0.1.379/sdk/utils/django_request_id.py
+-rw-r--r--   0        0        0     5349 2023-01-25 15:15:32.000000 mm_sdk-0.1.379/sdk/yandex_courier.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 mm_sdk-0.1.379/setup.py
+-rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 mm_sdk-0.1.379/PKG-INFO
```

### Comparing `mm_sdk-0.1.378/pyproject.toml` & `mm_sdk-0.1.379/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mm-sdk"
-version = "0.1.378"
+version = "0.1.379"
 description = ""
 authors = ["dyus <dyuuus@gmail.com>"]
 packages = [
     { include = "sdk" },
 ]
 
 [build-system]
```

### Comparing `mm_sdk-0.1.378/sdk/__init__.py` & `mm_sdk-0.1.379/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/admitad.py` & `mm_sdk-0.1.379/sdk/admitad.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/analytics.py` & `mm_sdk-0.1.379/sdk/analytics.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/barcode_recognizer.py` & `mm_sdk-0.1.379/sdk/barcode_recognizer.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/cash_register.py` & `mm_sdk-0.1.379/sdk/cash_register.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/click_again.py` & `mm_sdk-0.1.379/sdk/click_again.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/client.py` & `mm_sdk-0.1.379/sdk/client.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/cryptopro.py` & `mm_sdk-0.1.379/sdk/cryptopro.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/elk.py` & `mm_sdk-0.1.379/sdk/elk.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/face_detector.py` & `mm_sdk-0.1.379/sdk/face_detector.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/gift.py` & `mm_sdk-0.1.379/sdk/gift.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import math
 
 from enum import Enum
 from typing import List, Optional
 
 from pydantic import BaseModel, Field, HttpUrl
 
 from .client import SDKClient, SDKResponse
@@ -75,14 +76,21 @@
     is_promo: bool
     is_first_time: bool
     min_cost: Optional[int]
 
     class Config:
         use_enum_values = True
 
+    def get_discount(self, cost: int) -> int:
+        """Округляем до целого числа делящегося на 5 в сторону клиента,
+        по указанию от Леши Пермякова"""
+        if self.amount_type == AmountType.percent:
+            return math.ceil(cost * self.amount / 100 / 5) * 5
+        return self.amount
+
 
 class GiftError(BaseModel):
     code: str
     message: str
 
 
 class GiftCodeCheckResponse(GiftCodeResponse):
```

### Comparing `mm_sdk-0.1.378/sdk/gigtest.py` & `mm_sdk-0.1.379/sdk/gigtest.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/mis/client.py` & `mm_sdk-0.1.379/sdk/mis/client.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/mis/crm.py` & `mm_sdk-0.1.379/sdk/mis/crm.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/mis/lab.py` & `mm_sdk-0.1.379/sdk/mis/lab.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/mis/lmk.py` & `mm_sdk-0.1.379/sdk/mis/lmk.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/mis/mobil.py` & `mm_sdk-0.1.379/sdk/mis/mobil.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/mis/samd.py` & `mm_sdk-0.1.379/sdk/mis/samd.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/mis/standalone.py` & `mm_sdk-0.1.379/sdk/mis/standalone.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/mis/widgets.py` & `mm_sdk-0.1.379/sdk/mis/widgets.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/mobile_backend.py` & `mm_sdk-0.1.379/sdk/mobile_backend.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/notemaster.py` & `mm_sdk-0.1.379/sdk/notemaster.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/notification.py` & `mm_sdk-0.1.379/sdk/notification.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/nsirosminzdrav.py` & `mm_sdk-0.1.379/sdk/nsirosminzdrav.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/personal.py` & `mm_sdk-0.1.379/sdk/personal.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/pre_record.py` & `mm_sdk-0.1.379/sdk/pre_record.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/prodoctorov.py` & `mm_sdk-0.1.379/sdk/prodoctorov.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/reestr.py` & `mm_sdk-0.1.379/sdk/reestr.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/roistat.py` & `mm_sdk-0.1.379/sdk/roistat.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/samd.py` & `mm_sdk-0.1.379/sdk/samd.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/site_mobilmed.py` & `mm_sdk-0.1.379/sdk/site_mobilmed.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/sms.py` & `mm_sdk-0.1.379/sdk/sms.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/sdk/yandex_courier.py` & `mm_sdk-0.1.379/sdk/yandex_courier.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.378/setup.py` & `mm_sdk-0.1.379/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.23.3,<0.24.0', 'pydantic>=1.7.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'mm-sdk',
-    'version': '0.1.378',
+    'version': '0.1.379',
     'description': '',
     'long_description': 'None',
     'author': 'dyus',
     'author_email': 'dyuuus@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mm_sdk-0.1.378/PKG-INFO` & `mm_sdk-0.1.379/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mm-sdk
-Version: 0.1.378
+Version: 0.1.379
 Summary: 
 Author: dyus
 Author-email: dyuuus@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

