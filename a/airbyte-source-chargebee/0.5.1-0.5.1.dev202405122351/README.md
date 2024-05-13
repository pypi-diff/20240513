# Comparing `tmp/airbyte_source_chargebee-0.5.1.tar.gz` & `tmp/airbyte_source_chargebee-0.5.1.dev202405122351.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_chargebee-0.5.1.tar", max compression
+gzip compressed data, was "airbyte_source_chargebee-0.5.1.dev202405122351.tar", max compression
```

## Comparing `airbyte_source_chargebee-0.5.1.tar` & `airbyte_source_chargebee-0.5.1.dev202405122351.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     4562 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/README.md
--rw-r--r--   0        0        0      782 2024-05-10 10:43:37.223538 airbyte_source_chargebee-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      130 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/__init__.py
--rw-r--r--   0        0        0     6489 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/components.py
--rw-r--r--   0        0        0    14973 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/manifest.yaml
--rw-r--r--   0        0        0      239 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/run.py
--rw-r--r--   0        0        0     6678 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/addon.json
--rw-r--r--   0        0        0     2220 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/attached_item.json
--rw-r--r--   0        0        0     1364 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/comment.json
--rw-r--r--   0        0        0     1746 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/contact.json
--rw-r--r--   0        0        0     5624 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/coupon.json
--rw-r--r--   0        0        0    22604 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/credit_note.json
--rw-r--r--   0        0        0    17613 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/customer.json
--rw-r--r--   0        0        0     3297 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/differential_price.json
--rw-r--r--   0        0        0     2017 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/event.json
--rw-r--r--   0        0        0     4023 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/gift.json
--rw-r--r--   0        0        0     2224 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/hosted_page.json
--rw-r--r--   0        0        0    30727 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/invoice.json
--rw-r--r--   0        0        0     3510 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/item.json
--rw-r--r--   0        0        0     1278 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/item_family.json
--rw-r--r--   0        0        0     7361 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/item_price.json
--rw-r--r--   0        0        0    20267 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/order.json
--rw-r--r--   0        0        0     8208 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/payment_source.json
--rw-r--r--   0        0        0     9798 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/plan.json
--rw-r--r--   0        0        0     2039 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/promotional_credit.json
--rw-r--r--   0        0        0    13207 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/quote.json
--rw-r--r--   0        0        0     7310 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/quote_line_group.json
--rw-r--r--   0        0        0      328 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/shared/_definitions.json
--rw-r--r--   0        0        0     1285 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/site_migration_detail.json
--rw-r--r--   0        0        0    28215 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/subscription.json
--rw-r--r--   0        0        0     9683 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/transaction.json
--rw-r--r--   0        0        0     4615 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/unbilled_charge.json
--rw-r--r--   0        0        0     2340 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/schemas/virtual_bank_account.json
--rw-r--r--   0        0        0      478 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/source.py
--rw-r--r--   0        0        0     1474 2024-05-10 09:50:12.000000 airbyte_source_chargebee-0.5.1/source_chargebee/spec.yaml
--rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 airbyte_source_chargebee-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     4562 2024-05-12 23:48:40.463544 airbyte_source_chargebee-0.5.1.dev202405122351/README.md
+-rw-r--r--   0        0        0      798 2024-05-12 23:52:00.516745 airbyte_source_chargebee-0.5.1.dev202405122351/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/__init__.py
+-rw-r--r--   0        0        0     6489 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/components.py
+-rw-r--r--   0        0        0    14973 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/run.py
+-rw-r--r--   0        0        0     6678 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/addon.json
+-rw-r--r--   0        0        0     2220 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/attached_item.json
+-rw-r--r--   0        0        0     1364 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/comment.json
+-rw-r--r--   0        0        0     1746 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/contact.json
+-rw-r--r--   0        0        0     5624 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/coupon.json
+-rw-r--r--   0        0        0    22604 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/credit_note.json
+-rw-r--r--   0        0        0    17613 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/customer.json
+-rw-r--r--   0        0        0     3297 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/differential_price.json
+-rw-r--r--   0        0        0     2017 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/event.json
+-rw-r--r--   0        0        0     4023 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/gift.json
+-rw-r--r--   0        0        0     2224 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/hosted_page.json
+-rw-r--r--   0        0        0    30727 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/invoice.json
+-rw-r--r--   0        0        0     3510 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/item.json
+-rw-r--r--   0        0        0     1278 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/item_family.json
+-rw-r--r--   0        0        0     7361 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/item_price.json
+-rw-r--r--   0        0        0    20267 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/order.json
+-rw-r--r--   0        0        0     8208 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/payment_source.json
+-rw-r--r--   0        0        0     9798 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/plan.json
+-rw-r--r--   0        0        0     2039 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/promotional_credit.json
+-rw-r--r--   0        0        0    13207 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/quote.json
+-rw-r--r--   0        0        0     7310 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/quote_line_group.json
+-rw-r--r--   0        0        0      328 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/shared/_definitions.json
+-rw-r--r--   0        0        0     1285 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/site_migration_detail.json
+-rw-r--r--   0        0        0    28215 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/subscription.json
+-rw-r--r--   0        0        0     9683 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/transaction.json
+-rw-r--r--   0        0        0     4615 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/unbilled_charge.json
+-rw-r--r--   0        0        0     2340 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/virtual_bank_account.json
+-rw-r--r--   0        0        0      478 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/source.py
+-rw-r--r--   0        0        0     1474 2024-05-12 23:48:40.467544 airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/spec.yaml
+-rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 airbyte_source_chargebee-0.5.1.dev202405122351/PKG-INFO
```

### Comparing `airbyte_source_chargebee-0.5.1/README.md` & `airbyte_source_chargebee-0.5.1.dev202405122351/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/pyproject.toml` & `airbyte_source_chargebee-0.5.1.dev202405122351/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.5.1"
+version = "0.5.1.dev202405122351"
 name = "airbyte-source-chargebee"
 description = "Source implementation for Chargebee."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/components.py` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/manifest.yaml` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/addon.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/addon.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/attached_item.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/attached_item.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/comment.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/comment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/contact.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/contact.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/coupon.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/coupon.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/credit_note.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/credit_note.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/customer.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/customer.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/differential_price.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/differential_price.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/event.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/event.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/gift.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/gift.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/hosted_page.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/hosted_page.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/invoice.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/invoice.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/item.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/item.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/item_family.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/item_family.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/item_price.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/item_price.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/order.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/order.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/payment_source.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/payment_source.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/plan.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/plan.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/promotional_credit.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/promotional_credit.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/quote.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/quote.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/quote_line_group.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/quote_line_group.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/site_migration_detail.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/site_migration_detail.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/subscription.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/subscription.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/transaction.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/transaction.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/unbilled_charge.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/unbilled_charge.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/schemas/virtual_bank_account.json` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/schemas/virtual_bank_account.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/source_chargebee/spec.yaml` & `airbyte_source_chargebee-0.5.1.dev202405122351/source_chargebee/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_chargebee-0.5.1/PKG-INFO` & `airbyte_source_chargebee-0.5.1.dev202405122351/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-chargebee
-Version: 0.5.1
+Version: 0.5.1.dev202405122351
 Summary: Source implementation for Chargebee.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

