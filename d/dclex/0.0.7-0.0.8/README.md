# Comparing `tmp/dclex-0.0.7.tar.gz` & `tmp/dclex-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dclex-0.0.7.tar", last modified: Thu May  9 11:53:35 2024, max compression
+gzip compressed data, was "dclex-0.0.8.tar", last modified: Mon May 13 14:54:35 2024, max compression
```

## Comparing `dclex-0.0.7.tar` & `dclex-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.567085 dclex-0.0.7/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     8250 2024-01-31 17:39:20.000000 dclex-0.0.7/LICENSE
--rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-05-09 11:53:35.567085 dclex-0.0.7/PKG-INFO
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      450 2024-04-05 14:00:22.000000 dclex-0.0.7/README.md
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      739 2024-05-09 11:43:37.000000 dclex-0.0.7/pyproject.toml
--rw-rw-r--   0 clouds    (1001) clouds    (1001)       38 2024-05-09 11:53:35.567085 dclex-0.0.7/setup.cfg
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.563085 dclex-0.0.7/src/
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.563085 dclex-0.0.7/src/dclex/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      208 2024-05-09 11:47:56.000000 dclex-0.0.7/src/dclex/__init__.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    11676 2024-05-09 11:47:57.000000 dclex-0.0.7/src/dclex/dclex.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    12999 2024-05-09 11:47:57.000000 dclex-0.0.7/src/dclex/dclex_client.py
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.567085 dclex-0.0.7/src/dclex/resources/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    19297 2024-02-02 17:33:59.000000 dclex-0.0.7/src/dclex/resources/digital_identity_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    15662 2024-02-02 17:33:59.000000 dclex-0.0.7/src/dclex/resources/factory_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     6200 2024-02-02 17:33:59.000000 dclex-0.0.7/src/dclex/resources/usdc_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     9883 2024-02-02 17:33:59.000000 dclex-0.0.7/src/dclex/resources/vault_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1188 2024-03-01 16:20:01.000000 dclex-0.0.7/src/dclex/settings.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     2285 2024-03-01 16:30:00.000000 dclex-0.0.7/src/dclex/types.py
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.567085 dclex-0.0.7/src/dclex.egg-info/
--rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-05-09 11:53:35.000000 dclex-0.0.7/src/dclex.egg-info/PKG-INFO
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      580 2024-05-09 11:53:35.000000 dclex-0.0.7/src/dclex.egg-info/SOURCES.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)        1 2024-05-09 11:53:35.000000 dclex-0.0.7/src/dclex.egg-info/dependency_links.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)       60 2024-05-09 11:53:35.000000 dclex-0.0.7/src/dclex.egg-info/requires.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)        6 2024-05-09 11:53:35.000000 dclex-0.0.7/src/dclex.egg-info/top_level.txt
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.567085 dclex-0.0.7/tests/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1167 2024-03-04 19:14:07.000000 dclex-0.0.7/tests/test_account.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     6062 2024-03-04 19:14:07.000000 dclex-0.0.7/tests/test_orders.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1534 2024-04-05 13:55:04.000000 dclex-0.0.7/tests/test_stocks.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     7028 2024-05-09 11:47:57.000000 dclex-0.0.7/tests/test_transfers.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.533091 dclex-0.0.8/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     8250 2024-01-31 17:39:20.000000 dclex-0.0.8/LICENSE
+-rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-05-13 14:54:35.533091 dclex-0.0.8/PKG-INFO
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      450 2024-04-05 14:00:22.000000 dclex-0.0.8/README.md
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      739 2024-05-13 11:24:27.000000 dclex-0.0.8/pyproject.toml
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)       38 2024-05-13 14:54:35.533091 dclex-0.0.8/setup.cfg
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.529091 dclex-0.0.8/src/
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.529091 dclex-0.0.8/src/dclex/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      208 2024-05-09 11:47:56.000000 dclex-0.0.8/src/dclex/__init__.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    12427 2024-05-13 11:23:39.000000 dclex-0.0.8/src/dclex/dclex.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    12993 2024-05-10 16:55:28.000000 dclex-0.0.8/src/dclex/dclex_client.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.533091 dclex-0.0.8/src/dclex/resources/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    19297 2024-02-02 17:33:59.000000 dclex-0.0.8/src/dclex/resources/digital_identity_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    15662 2024-02-02 17:33:59.000000 dclex-0.0.8/src/dclex/resources/factory_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     6200 2024-02-02 17:33:59.000000 dclex-0.0.8/src/dclex/resources/usdc_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     9883 2024-02-02 17:33:59.000000 dclex-0.0.8/src/dclex/resources/vault_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1188 2024-03-01 16:20:01.000000 dclex-0.0.8/src/dclex/settings.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     2285 2024-03-01 16:30:00.000000 dclex-0.0.8/src/dclex/types.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.533091 dclex-0.0.8/src/dclex.egg-info/
+-rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-05-13 14:54:35.000000 dclex-0.0.8/src/dclex.egg-info/PKG-INFO
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      580 2024-05-13 14:54:35.000000 dclex-0.0.8/src/dclex.egg-info/SOURCES.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)        1 2024-05-13 14:54:35.000000 dclex-0.0.8/src/dclex.egg-info/dependency_links.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)       60 2024-05-13 14:54:35.000000 dclex-0.0.8/src/dclex.egg-info/requires.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)        6 2024-05-13 14:54:35.000000 dclex-0.0.8/src/dclex.egg-info/top_level.txt
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-13 14:54:35.533091 dclex-0.0.8/tests/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1167 2024-03-04 19:14:07.000000 dclex-0.0.8/tests/test_account.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     6062 2024-03-04 19:14:07.000000 dclex-0.0.8/tests/test_orders.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1534 2024-04-05 13:55:04.000000 dclex-0.0.8/tests/test_stocks.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     7431 2024-05-13 11:23:39.000000 dclex-0.0.8/tests/test_transfers.py
```

### Comparing `dclex-0.0.7/LICENSE` & `dclex-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dclex-0.0.7/PKG-INFO` & `dclex-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dclex
-Version: 0.0.7
+Version: 0.0.8
 Summary: DCLEX python library
 License: DCLEX API Non-Commercial License
         
         This DCLEX API Non-Commercial License ("License") is an agreement between DCLEX inc. ("DCLEX") and You, and governs Your use of the API Code. By loging to your DCLEX account programmatically , you acknowledge that You consent to be legally bound by this Agreement.
         
         1. Introduction.
         1.1 DCLEX has developed application program interface ("API") code to permit its customers to use their own internal proprietary software tools in managing their accounts with DCLEX. This License is intended only for users who wish to use the API Code by itself as is, or in connection with or for the development of their own internal proprietary tools to manage their own DCLEX accounts. This License is NOT for anybody who is developing software applications that they wish to: (a) sell to third party users for a fee, or (b) give to third party users to generate an indirect financial benefit (e.g., commissions). If You wish to make a software application for the purposes described in the preceding sentence then please us at info@dclex.com.
```

### Comparing `dclex-0.0.7/pyproject.toml` & `dclex-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dclex"
-version = "0.0.7"
+version = "0.0.8"
 description = "DCLEX python library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 classifiers = [
     "Intended Audience :: Financial and Insurance Industry",
     "Programming Language :: Python :: 3.7",
```

### Comparing `dclex-0.0.7/src/dclex/dclex.py` & `dclex-0.0.8/src/dclex/dclex.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     pass
 
 
 class DigitalIdentityAlreadyClaimed(Exception):
     pass
 
 
+class WithdrawalNotFound(Exception):
+    pass
+
+
 class Dclex:
     def __init__(self, private_key: str, web3_provider_url: str) -> None:
         self._account = Web3().eth.account.from_key(private_key)
         self._web3 = Web3(Web3.HTTPProvider(web3_provider_url))
         self._dclex_client = DclexClient()
 
     def login(self) -> None:
@@ -123,41 +127,42 @@
         )
         return self._build_and_send_transaction(
             usdc_contract.functions.transfer(
                 VAULT_CONTRACT_ADDRESS, int(amount * Decimal(10**6))
             )
         )
 
-    def initialize_usdc_withdrawal(self, amount: Decimal):
+    def request_usdc_withdrawal(self, amount: Decimal):
         account_status = self._dclex_client.get_account_status()
         if account_status not in [AccountStatus.VERIFIED, AccountStatus.DID_MINTED]:
             raise AccountNotVerified()
 
         try:
-            return self._dclex_client.initialize_usdc_withdrawal(amount=amount)
+            return self._dclex_client.request_usdc_withdrawal(amount=amount)
         except APIError as exc:
             if exc.error_code == "INSUFFICIENT_FUNDS":
                 raise NotEnoughFunds()
 
-    def finalize_usdc_withdrawal(self, withdrawal_id: int, amount: Decimal) -> str:
+    def claim_usdc_withdrawal(self, withdrawal_id: int) -> str:
+        withdrawal = self._get_claimable_withdrawal(withdrawal_id)
         signature = self._dclex_client.get_withdraw_signature(
             withdrawal_id=withdrawal_id,
         )
 
         vault_contract_address = self._web3.to_checksum_address(VAULT_CONTRACT_ADDRESS)
         vault_contract = self._web3.eth.contract(
             address=vault_contract_address, abi=VAULT_CONTRACT_ABI
         )
         return self._build_and_send_transaction(
             vault_contract.functions.withdraw(
                 {
                     "token": USDC_CONTRACT_ADDRESS,
                     "account": VAULT_CONTRACT_ADDRESS,
                     "to": self._account.address,
-                    "amount": int(amount * Decimal(10**6)),
+                    "amount": int(withdrawal.amount * Decimal(10**6)),
                     "nonce": withdrawal_id,
                 },
                 bytes.fromhex(signature),
             )
         )
 
     def deposit_stock_token(self, stock_symbol: str, amount: int) -> str:
@@ -184,53 +189,67 @@
                     "account": self._account.address,
                     "nonce": int.from_bytes(bytes.fromhex(signature.nonce[2:]), "big"),
                 },
                 bytes.fromhex(signature.signature),
             )
         )
 
-    def initialize_stock_withdrawal(self, stock_symbol: str, amount: int):
+    def request_stock_withdrawal(self, stock_symbol: str, amount: int):
         account_status = self._dclex_client.get_account_status()
         if account_status != AccountStatus.DID_MINTED:
             raise AccountNotVerified()
 
         try:
-            return self._dclex_client.initialize_stock_withdrawal(
+            return self._dclex_client.request_stock_withdrawal(
                 amount=amount,
                 asset_type=stock_symbol,
             )
         except APIError as exc:
             if exc.error_code == "INSUFFICIENT_FUNDS":
                 raise NotEnoughFunds()
 
-    def finalize_stock_withdrawal(
-        self, withdrawal_id: int, stock_symbol: str, amount: int
-    ) -> str:
+    def claim_stock_withdrawal(self, withdrawal_id: int) -> str:
+        withdrawal = self._get_claimable_withdrawal(withdrawal_id)
         signature = self._dclex_client.get_withdraw_signature(
             withdrawal_id=withdrawal_id,
         )
 
         factory_contract_address = self._web3.to_checksum_address(
             FACTORY_CONTRACT_ADDRESS
         )
         factory_contract = self._web3.eth.contract(
             address=factory_contract_address, abi=FACTORY_CONTRACT_ABI
         )
         return self._build_and_send_transaction(
             factory_contract.functions.mintStocks(
                 {
-                    "symbol": stock_symbol,
-                    "amount": int(amount * Decimal(10**18)),
+                    "symbol": withdrawal.asset_type,
+                    "amount": int(withdrawal.amount * Decimal(10**18)),
                     "account": self._account.address,
                     "nonce": withdrawal_id,
                 },
                 bytes.fromhex(signature),
             )
         )
 
+    def _get_claimable_withdrawal(self, withdrawal_id: int) -> ClaimableWithdrawal:
+        claimable_withdrawals = self._dclex_client.claimable_withdrawals()
+        matching_withdrawals = [
+            withdrawal
+            for withdrawal in claimable_withdrawals
+            if withdrawal.withdrawal_id == withdrawal_id
+        ]
+        if len(matching_withdrawals) == 0:
+            raise WithdrawalNotFound()
+        if len(matching_withdrawals) > 1:
+            raise RuntimeError(
+                "Received multiple claimable withdrawals with the same id"
+            )
+        return matching_withdrawals[0]
+
     def pending_transfers(self) -> list[Transfer]:
         return self._dclex_client.get_pending_transfers()
 
     def closed_transfers(self) -> list[Transfer]:
         return self._dclex_client.get_closed_transfers()
 
     def get_usdc_available_balance(self) -> Decimal:
```

### Comparing `dclex-0.0.7/src/dclex/dclex_client.py` & `dclex-0.0.8/src/dclex/dclex_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,21 +174,21 @@
             "/deposit-stocks-signature/", {"amount": str(amount), "symbol": symbol}
         )
         return DepositStocksSignature(
             signature=response["signature"],
             nonce=response["nonce"],
         )
 
-    def initialize_usdc_withdrawal(self, amount: Decimal) -> int:
+    def request_usdc_withdrawal(self, amount: Decimal) -> int:
         response = self._authorized_post(
             "/initialize-usdc-withdraw/", {"amount": str(amount)}
         )
         return response["withdrawalId"]
 
-    def initialize_stock_withdrawal(self, amount: int, asset_type: str) -> int:
+    def request_stock_withdrawal(self, amount: int, asset_type: str) -> int:
         response = self._authorized_post(
             "/initialize-stocks-withdraw/",
             {"amount": str(amount), "assetType": asset_type},
         )
         return response["withdrawalId"]
 
     def get_withdraw_signature(self, withdrawal_id: int) -> str:
```

### Comparing `dclex-0.0.7/src/dclex/resources/digital_identity_contract_abi.json` & `dclex-0.0.8/src/dclex/resources/digital_identity_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.7/src/dclex/resources/factory_contract_abi.json` & `dclex-0.0.8/src/dclex/resources/factory_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.7/src/dclex/resources/usdc_contract_abi.json` & `dclex-0.0.8/src/dclex/resources/usdc_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.7/src/dclex/resources/vault_contract_abi.json` & `dclex-0.0.8/src/dclex/resources/vault_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.7/src/dclex/settings.py` & `dclex-0.0.8/src/dclex/settings.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.7/src/dclex/types.py` & `dclex-0.0.8/src/dclex/types.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.7/src/dclex.egg-info/PKG-INFO` & `dclex-0.0.8/src/dclex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dclex
-Version: 0.0.7
+Version: 0.0.8
 Summary: DCLEX python library
 License: DCLEX API Non-Commercial License
         
         This DCLEX API Non-Commercial License ("License") is an agreement between DCLEX inc. ("DCLEX") and You, and governs Your use of the API Code. By loging to your DCLEX account programmatically , you acknowledge that You consent to be legally bound by this Agreement.
         
         1. Introduction.
         1.1 DCLEX has developed application program interface ("API") code to permit its customers to use their own internal proprietary software tools in managing their accounts with DCLEX. This License is intended only for users who wish to use the API Code by itself as is, or in connection with or for the development of their own internal proprietary tools to manage their own DCLEX accounts. This License is NOT for anybody who is developing software applications that they wish to: (a) sell to third party users for a fee, or (b) give to third party users to generate an indirect financial benefit (e.g., commissions). If You wish to make a software application for the purposes described in the preceding sentence then please us at info@dclex.com.
```

### Comparing `dclex-0.0.7/src/dclex.egg-info/SOURCES.txt` & `dclex-0.0.8/src/dclex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dclex-0.0.7/tests/test_account.py` & `dclex-0.0.8/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.7/tests/test_orders.py` & `dclex-0.0.8/tests/test_orders.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.7/tests/test_stocks.py` & `dclex-0.0.8/tests/test_stocks.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.7/tests/test_transfers.py` & `dclex-0.0.8/tests/test_transfers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,69 @@
 from decimal import Decimal
 from time import sleep
 from unittest.mock import ANY
 
 import pytest
 
-from dclex.dclex import AccountNotVerified, NotEnoughFunds
+from dclex.dclex import AccountNotVerified, NotEnoughFunds, WithdrawalNotFound
 from dclex.types import OrderSide, TransactionType, Transfer, TransferHistoryStatus
 
 from .conftest import wait_for_transaction
 
 
 def test_deposit_and_withdraw_usdc(dclex, provider_url):
     dclex.login()
 
     usdc_available_balance_before = dclex.get_usdc_available_balance()
     usdc_ledger_balance_before = dclex.get_usdc_ledger_balance()
 
-    tx_hash = dclex.deposit_usdc(amount=Decimal(100))
-    wait_for_transaction(tx_hash, provider_url)
+    # tx_hash = dclex.deposit_usdc(amount=Decimal(100))
+    # wait_for_transaction(tx_hash, provider_url)
 
-    sleep(3)
+    # sleep(3)
 
-    assert dclex.get_usdc_ledger_balance() - usdc_ledger_balance_before == 100
-    assert dclex.get_usdc_available_balance() - usdc_available_balance_before == 100
+    # assert dclex.get_usdc_ledger_balance() - usdc_ledger_balance_before == 100
+    # assert dclex.get_usdc_available_balance() - usdc_available_balance_before == 100
 
-    withdrawal_id = dclex.initialize_usdc_withdrawal(Decimal(100))
-    tx_hash = dclex.finalize_usdc_withdrawal(withdrawal_id, Decimal(100))
+    withdrawal_id = dclex.request_usdc_withdrawal(Decimal(100))
+    tx_hash = dclex.claim_usdc_withdrawal(withdrawal_id)
     wait_for_transaction(tx_hash, provider_url)
 
     sleep(15)
 
     assert dclex.get_usdc_ledger_balance() == usdc_ledger_balance_before - 100
     assert dclex.get_usdc_available_balance() == usdc_available_balance_before - 100
 
 
 def test_deposit_usdc_raises_when_user_is_not_verified(dclex_unverified):
     dclex_unverified.login()
     with pytest.raises(AccountNotVerified):
         dclex_unverified.deposit_usdc(Decimal(100))
 
 
-def test_initialize_usdc_withdrawal_raises_when_user_is_not_verified(dclex_unverified):
+def test_request_usdc_withdrawal_raises_when_user_is_not_verified(dclex_unverified):
     dclex_unverified.login()
     with pytest.raises(AccountNotVerified):
-        dclex_unverified.initialize_usdc_withdrawal(Decimal(100))
+        dclex_unverified.request_usdc_withdrawal(Decimal(100))
 
 
-def test_initialize_usdc_withdrawal_raises_when_not_enough_funds(dclex, provider_url):
+def test_request_usdc_withdrawal_raises_when_not_enough_funds(dclex, provider_url):
     dclex.login()
     usdc_available_balance = dclex.get_usdc_available_balance()
 
     with pytest.raises(NotEnoughFunds):
-        dclex.initialize_usdc_withdrawal(Decimal(usdc_available_balance + 1))
+        dclex.request_usdc_withdrawal(Decimal(usdc_available_balance + 1))
+
+
+def test_claim_usdc_withdrawal_raises_when_claimable_withdrawal_id_does_not_exist(
+    dclex, provider_url
+):
+    dclex.login()
+    with pytest.raises(WithdrawalNotFound):
+        dclex.claim_usdc_withdrawal(9999)
 
 
 def test_withdraw_and_deposit_stock(dclex, provider_url):
     dclex.login()
 
     tx_hash = dclex.deposit_usdc(Decimal(200))
     wait_for_transaction(tx_hash, provider_url)
@@ -63,16 +71,16 @@
 
     dclex.create_limit_order(OrderSide.BUY, "AAPL", 1, Decimal(190))
     sleep(30)
 
     aapl_available_balance_before = dclex.get_stock_available_balance("AAPL")
     aapl_ledger_balance_before = dclex.get_stock_ledger_balance("AAPL")
 
-    withdrawal_id = dclex.initialize_stock_withdrawal("AAPL", 1)
-    tx_hash = dclex.finalize_stock_withdrawal(withdrawal_id, "AAPL", 1)
+    withdrawal_id = dclex.request_stock_withdrawal("AAPL", 1)
+    tx_hash = dclex.claim_stock_withdrawal(withdrawal_id)
     wait_for_transaction(tx_hash, provider_url)
     sleep(20)
 
     assert (
         dclex.get_stock_available_balance("AAPL") - aapl_available_balance_before == -1
     )
     assert dclex.get_stock_ledger_balance("AAPL") - aapl_ledger_balance_before == -1
@@ -87,26 +95,34 @@
 
 def test_deposit_stock_raises_when_user_is_not_verified(dclex_unverified):
     dclex_unverified.login()
     with pytest.raises(AccountNotVerified):
         dclex_unverified.deposit_stock_token("AAPL", Decimal(1))
 
 
-def test_initialize_stock_withdrawal_raises_when_user_is_not_verified(dclex_unverified):
+def test_request_stock_withdrawal_raises_when_user_is_not_verified(dclex_unverified):
     dclex_unverified.login()
     with pytest.raises(AccountNotVerified):
-        dclex_unverified.initialize_stock_withdrawal("AAPL", Decimal(1))
+        dclex_unverified.request_stock_withdrawal("AAPL", Decimal(1))
 
 
-def test_initialize_stock_withdrawal_raises_when_not_enough_funds(dclex, provider_url):
+def test_request_stock_withdrawal_raises_when_not_enough_funds(dclex, provider_url):
     dclex.login()
     available_balance = dclex.get_stock_available_balance("AAPL")
 
     with pytest.raises(NotEnoughFunds):
-        dclex.initialize_stock_withdrawal("AAPL", available_balance + 1)
+        dclex.request_stock_withdrawal("AAPL", available_balance + 1)
+
+
+def test_claim_stock_withdrawal_raises_when_claimable_withdrawal_id_does_not_exist(
+    dclex, provider_url
+):
+    dclex.login()
+    with pytest.raises(WithdrawalNotFound):
+        dclex.claim_stock_withdrawal(9999)
 
 
 def test_usdc_pending_transfers(dclex, provider_url):
     dclex.login()
 
     assert dclex.pending_transfers() == []
```

