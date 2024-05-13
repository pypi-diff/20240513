# Comparing `tmp/vitya-0.20.4.tar.gz` & `tmp/vitya-0.20.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vitya-0.20.4.tar", last modified: Mon Apr 22 13:13:46 2024, max compression
+gzip compressed data, was "dist/vitya-0.20.5.tar", last modified: Mon May 13 13:05:37 2024, max compression
```

## Comparing `vitya-0.20.4.tar` & `vitya-0.20.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:13:46.000000 vitya-0.20.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 13:13:39.000000 vitya-0.20.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-22 13:13:46.000000 vitya-0.20.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-22 13:13:39.000000 vitya-0.20.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-22 13:13:39.000000 vitya-0.20.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:13:46.000000 vitya-0.20.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-22 13:13:39.000000 vitya-0.20.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:13:46.000000 vitya-0.20.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-22 13:13:39.000000 vitya-0.20.4/tests/test_error_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-22 13:13:39.000000 vitya-0.20.4/tests/test_vitya.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:13:46.000000 vitya-0.20.4/vitya/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/error_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/errors_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:13:46.000000 vitya-0.20.4/vitya/payment_order/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/payment_order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/payment_order/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    35446 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/payment_order/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/payment_order/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:13:46.000000 vitya-0.20.4/vitya/payment_order/payments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/payment_order/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/payment_order/payments/checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18973 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/payment_order/payments/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/payment_order/payments/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/payment_order/payments/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/payment_order/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/pydantic_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/typing_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-22 13:13:39.000000 vitya-0.20.4/vitya/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:13:46.000000 vitya-0.20.4/vitya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-22 13:13:46.000000 vitya-0.20.4/vitya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 13:13:46.000000 vitya-0.20.4/vitya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:13:46.000000 vitya-0.20.4/vitya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 13:13:46.000000 vitya-0.20.4/vitya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:37.000000 vitya-0.20.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 13:05:31.000000 vitya-0.20.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-13 13:05:37.000000 vitya-0.20.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-13 13:05:31.000000 vitya-0.20.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-13 13:05:31.000000 vitya-0.20.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:05:37.000000 vitya-0.20.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-13 13:05:31.000000 vitya-0.20.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:37.000000 vitya-0.20.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-13 13:05:31.000000 vitya-0.20.5/tests/test_error_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-13 13:05:31.000000 vitya-0.20.5/tests/test_vitya.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:37.000000 vitya-0.20.5/vitya/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/error_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/errors_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:37.000000 vitya-0.20.5/vitya/payment_order/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/payment_order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/payment_order/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35446 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/payment_order/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/payment_order/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:37.000000 vitya-0.20.5/vitya/payment_order/payments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/payment_order/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18070 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/payment_order/payments/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19286 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/payment_order/payments/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/payment_order/payments/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/payment_order/payments/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/payment_order/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/pydantic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/typing_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-13 13:05:31.000000 vitya-0.20.5/vitya/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:37.000000 vitya-0.20.5/vitya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-13 13:05:37.000000 vitya-0.20.5/vitya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-13 13:05:37.000000 vitya-0.20.5/vitya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:05:37.000000 vitya-0.20.5/vitya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 13:05:37.000000 vitya-0.20.5/vitya.egg-info/top_level.txt
```

### Comparing `vitya-0.20.4/LICENSE` & `vitya-0.20.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/PKG-INFO` & `vitya-0.20.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.20.4
+Version: 0.20.5
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.20.4/README.md` & `vitya-0.20.5/README.md`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/setup.py` & `vitya-0.20.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='vitya',
-    version='0.20.4',
+    version='0.20.5',
     author='hicebank.ru',
     author_email='inyutin@hicebank.ru',
     description='Validators for different russian banking values',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/hicebank/vitya',
     packages=setuptools.find_packages(),
```

### Comparing `vitya-0.20.4/tests/test_error_description.py` & `vitya-0.20.5/tests/test_error_description.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/tests/test_vitya.py` & `vitya-0.20.5/tests/test_vitya.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya/error_description.py` & `vitya-0.20.5/vitya/error_description.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya/errors.py` & `vitya-0.20.5/vitya/errors.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya/errors_base.py` & `vitya-0.20.5/vitya/errors_base.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya/payment_order/enums.py` & `vitya-0.20.5/vitya/payment_order/enums.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya/payment_order/errors.py` & `vitya-0.20.5/vitya/payment_order/errors.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya/payment_order/fields.py` & `vitya-0.20.5/vitya/payment_order/fields.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya/payment_order/payments/checkers.py` & `vitya-0.20.5/vitya/payment_order/payments/checkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     check_document_date_with_reason,
     check_document_number,
     check_oktmo,
     check_oktmo_with_payer_status,
     check_oktmo_with_receiver_account_number,
     check_operation_kind,
     check_payer_inn,
+    check_payer_inn_with_uin_and_receiver_account,
     check_payer_kpp,
     check_payer_status,
     check_payment_type_and_for_third_person,
     check_purpose,
     check_purpose_for_third_person,
     check_reason,
     check_receiver_account,
@@ -129,32 +130,51 @@
 
 
 class PayerINNChecker(BaseChecker):
     def __init__(
         self,
         payer_inn: Optional[PayerINN],
         payer_status: Optional[PayerStatus],
-        receiver_account: Optional[ReceiverAccountNumber],
-        uin: Optional[UIN],
         for_third_person: ForThirdPerson,
         payment_type: PaymentType
     ) -> None:
         self.payer_inn = payer_inn
         self.payer_status = payer_status
         self.for_third_person = for_third_person
         self.payment_type = payment_type
-        self.receiver_account = receiver_account
-        self.uin = uin
 
     def check(self) -> None:
         check_payer_inn(
             value=self.payer_inn,
             payment_type=self.payment_type,
             payer_status=self.payer_status,
             for_third_person=self.for_third_person,
+        )
+
+
+class PayerINNWithUinAndReceiverAccountChecker(BaseChecker):
+    def __init__(
+        self,
+        payer_inn: Optional[PayerINN],
+        payer_status: Optional[PayerStatus],
+        receiver_account: Optional[ReceiverAccountNumber],
+        uin: Optional[UIN],
+        payment_type: PaymentType
+    ) -> None:
+        self.payer_inn = payer_inn
+        self.payer_status = payer_status
+        self.payment_type = payment_type
+        self.receiver_account = receiver_account
+        self.uin = uin
+
+    def check(self) -> None:
+        check_payer_inn_with_uin_and_receiver_account(
+            value=self.payer_inn,
+            payment_type=self.payment_type,
+            payer_status=self.payer_status,
             receiver_account=self.receiver_account,
             uin=self.uin,
         )
 
 
 class UINChecker(BaseChecker):
     def __init__(
@@ -446,14 +466,15 @@
     __extra_wired_checkers__: ClassVar[Sequence[WiredChecker]] = []
     __auto_checkers__: ClassVar[Sequence[Type[BaseChecker]]] = [
         ReceiverAccountChecker,
         ReceiverAccountCheckerWithPaymentType,
         ReceiverAccountCheckerWithPaymentTypeAndPayerStatus,
         OperationKindChecker,
         PayerINNChecker,
+        PayerINNWithUinAndReceiverAccountChecker,
         UINChecker,
         PurposeChecker,
         ReceiverINNChecker,
         PayerStatusChecker,
         PaymentTypeAndForThirdPersonChecker,
         ForThirdPersonAndPurposeChecker,
         PayerKPPChecker,
```

### Comparing `vitya-0.20.4/vitya/payment_order/payments/checks.py` & `vitya-0.20.5/vitya/payment_order/payments/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,32 +230,23 @@
     return value
 
 
 def check_payer_inn(
     value: Optional[PayerINN],
     payment_type: PaymentType,
     payer_status: Optional[PayerStatus],
-    receiver_account: Optional[ReceiverAccountNumber],
-    uin: Optional[UIN],
     for_third_person: ForThirdPerson,
 ) -> Optional[PayerINN]:
     if not payment_type.is_budget:
         return value
 
     if value is None:
         if payment_type == PaymentType.BUDGET_OTHER:
             return None
-        elif (
-            payment_type == PaymentType.FNS
-            and payer_status == '13'
-            and receiver_account is not None
-            and receiver_account.startswith('03100')
-            and uin is not None
-            and len(uin) in [20, 25]
-        ):
+        elif payment_type == PaymentType.FNS:
             return None
         elif payment_type == PaymentType.CUSTOMS and payer_status == '30':
             return None
         raise PayerINNValidationEmptyNotAllowedError
 
     if payment_type == PaymentType.CUSTOMS:
         if payer_status == '06' and for_third_person and len(value) != 10:
@@ -266,14 +257,34 @@
 
     if value.startswith('00'):
         raise PayerINNValidationStartWithZerosError
 
     return value
 
 
+def check_payer_inn_with_uin_and_receiver_account(
+    value: Optional[PayerINN],
+    payment_type: PaymentType,
+    payer_status: Optional[PayerStatus],
+    receiver_account: Optional[ReceiverAccountNumber],
+    uin: Optional[UIN],
+) -> Optional[PayerINN]:
+    if value is None and payment_type == PaymentType.FNS:
+        if not (
+            payer_status == '13'
+            and receiver_account is not None
+            and receiver_account.startswith('03100')
+            and uin is not None
+            and len(uin) in [20, 25]
+        ):
+            raise PayerINNValidationEmptyNotAllowedError
+
+    return None
+
+
 def check_receiver_inn(
     value: Optional[ReceiverINN],
     payment_type: PaymentType,
 ) -> Optional[ReceiverINN]:
     if payment_type in [
         PaymentType.CUSTOMS,
         PaymentType.FNS,
```

### Comparing `vitya-0.20.4/vitya/payment_order/payments/constants.py` & `vitya-0.20.5/vitya/payment_order/payments/constants.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya/payment_order/payments/tools.py` & `vitya-0.20.5/vitya/payment_order/payments/tools.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya/payment_order/validators.py` & `vitya-0.20.5/vitya/payment_order/validators.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya/pydantic_fields.py` & `vitya-0.20.5/vitya/pydantic_fields.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya/validators.py` & `vitya-0.20.5/vitya/validators.py`

 * *Files identical despite different names*

### Comparing `vitya-0.20.4/vitya.egg-info/PKG-INFO` & `vitya-0.20.5/vitya.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.20.4
+Version: 0.20.5
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.20.4/vitya.egg-info/SOURCES.txt` & `vitya-0.20.5/vitya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

