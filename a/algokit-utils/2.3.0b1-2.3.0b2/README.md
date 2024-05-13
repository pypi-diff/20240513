# Comparing `tmp/algokit_utils-2.3.0b1-py3-none-any.whl.zip` & `tmp/algokit_utils-2.3.0b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 58581 bytes, number of entries: 24
+Zip file size: 58630 bytes, number of entries: 24
 -rw-r--r--  2.0 unx     4963 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx    10732 b- defN 80-Jan-01 00:00 algokit_utils/_debugging.py
 -rw-r--r--  2.0 unx     6786 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
--rw-r--r--  2.0 unx     5947 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
+-rw-r--r--  2.0 unx     6021 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    59092 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx     7216 b- defN 80-Jan-01 00:00 algokit_utils/asset.py
 -rw-r--r--  2.0 unx     8015 b- defN 80-Jan-01 00:00 algokit_utils/beta/account_manager.py
 -rw-r--r--  2.0 unx    12649 b- defN 80-Jan-01 00:00 algokit_utils/beta/algorand_client.py
 -rw-r--r--  2.0 unx     3117 b- defN 80-Jan-01 00:00 algokit_utils/beta/client_manager.py
@@ -15,12 +15,12 @@
 -rw-r--r--  2.0 unx     4279 b- defN 80-Jan-01 00:00 algokit_utils/config.py
 -rw-r--r--  2.0 unx    35110 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     5584 b- defN 80-Jan-01 00:00 algokit_utils/dispenser_api.py
 -rw-r--r--  2.0 unx     2617 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx    12803 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     5929 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-2.3.0b1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2207 b- defN 80-Jan-01 00:00 algokit_utils-2.3.0b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-2.3.0b1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2044 b- defN 16-Jan-01 00:00 algokit_utils-2.3.0b1.dist-info/RECORD
-24 files, 234523 bytes uncompressed, 55275 bytes compressed:  76.4%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-2.3.0b2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2207 b- defN 80-Jan-01 00:00 algokit_utils-2.3.0b2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-2.3.0b2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2044 b- defN 16-Jan-01 00:00 algokit_utils-2.3.0b2.dist-info/RECORD
+24 files, 234597 bytes uncompressed, 55324 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-2.3.0b1.dist-info/LICENSE
+Filename: algokit_utils-2.3.0b2.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-2.3.0b1.dist-info/METADATA
+Filename: algokit_utils-2.3.0b2.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-2.3.0b1.dist-info/WHEEL
+Filename: algokit_utils-2.3.0b2.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-2.3.0b1.dist-info/RECORD
+Filename: algokit_utils-2.3.0b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/_transfer.py

```diff
@@ -82,15 +82,15 @@
 
 def transfer(client: "AlgodClient", parameters: TransferParameters) -> PaymentTxn:
     """Transfer µALGOs between accounts"""
 
     params = parameters
     params.suggested_params = parameters.suggested_params or client.suggested_params()
     from_account = params.from_account
-    sender = address_from_private_key(from_account.private_key)  # type: ignore[no-untyped-call]
+    sender = _get_address(from_account)
     transaction = PaymentTxn(
         sender=sender,
         receiver=params.to_address,
         amt=params.micro_algos,
         note=params.note.encode("utf-8") if isinstance(params.note, str) else params.note,
         sp=params.suggested_params,
     )  # type: ignore[no-untyped-call]
@@ -101,15 +101,15 @@
 
 
 def transfer_asset(client: "AlgodClient", parameters: TransferAssetParameters) -> AssetTransferTxn:
     """Transfer assets between accounts"""
 
     params = parameters
     params.suggested_params = parameters.suggested_params or client.suggested_params()
-    sender = address_from_private_key(parameters.from_account.private_key)  # type: ignore[no-untyped-call]
+    sender = _get_address(parameters.from_account)
     suggested_params = parameters.suggested_params or client.suggested_params()
     xfer_txn = AssetTransferTxn(
         sp=suggested_params,
         sender=sender,
         receiver=params.to_address,
         close_assets_to=None,
         revocation_target=params.clawback_from,
@@ -135,13 +135,18 @@
     if parameters.suggested_params is not None and not parameters.suggested_params.flat_fee:
         _check_fee(transaction, parameters.max_fee_micro_algos)
 
     signed_transaction = transaction.sign(parameters.from_account.private_key)  # type: ignore[no-untyped-call]
     client.send_transaction(signed_transaction)
 
     txid = transaction.get_txid()  # type: ignore[no-untyped-call]
-    logger.debug(
-        f"Sent transaction {txid} type={transaction.type} from "
-        f"{address_from_private_key(parameters.from_account.private_key)}"  # type: ignore[no-untyped-call]
-    )
+    logger.debug(f"Sent transaction {txid} type={transaction.type} from {_get_address(parameters.from_account)}")
 
     return transaction
+
+
+def _get_address(account: Account | AccountTransactionSigner) -> str:
+    if type(account) is Account:
+        return account.address
+    else:
+        address = address_from_private_key(account.private_key)  # type: ignore[no-untyped-call]
+        return str(address)
```

## Comparing `algokit_utils-2.3.0b1.dist-info/LICENSE` & `algokit_utils-2.3.0b2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-2.3.0b1.dist-info/METADATA` & `algokit_utils-2.3.0b2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 2.3.0b1
+Version: 2.3.0b2
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-2.3.0b1.dist-info/RECORD` & `algokit_utils-2.3.0b2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 algokit_utils/__init__.py,sha256=yeufbE_5wjRILZs_10UD5B3_sjdwAfPXskdFKskzXhg,4963
 algokit_utils/_debugging.py,sha256=4UC5NZGqxF32y742TUB34rX9kWaObXCCPOs-lbkQjGQ,10732
 algokit_utils/_ensure_funded.py,sha256=ZdEdUB43QGIQrg7cSSgNrDmWaLSUhli9x9I6juwKfgo,6786
-algokit_utils/_transfer.py,sha256=CyXGOR_Zy-2crQhk-78uUbB8Sj_ZeTzxPwOAHU7wwno,5947
+algokit_utils/_transfer.py,sha256=R9q8RoMHiwtqcwQjuGHEluMxIzmYqAsI5WrTsQd24Ds,6021
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
 algokit_utils/application_client.py,sha256=qylA2aI4Ecs532bIs6fyc6FgLnWey9PBzZBZW_jnYtk,59092
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/asset.py,sha256=jsc7T1dH9HZA3Yve2gRLObwUlK6xLDoQz0NxLLnqaGs,7216
 algokit_utils/beta/account_manager.py,sha256=dSb-jpBAWRfmKFYzG6T8t5vkh6ysX2NkZXl5UcZY5WA,8015
 algokit_utils/beta/algorand_client.py,sha256=y1CYYn_ADwgOLTVID9BFMvdubDgKqUfx9R6XH3PrzsA,12649
 algokit_utils/beta/client_manager.py,sha256=rW58VVBdYAV_5QwXNyt3VMP8NGon_IRhq1Dr35Mp31g,3117
@@ -14,11 +14,11 @@
 algokit_utils/config.py,sha256=oY3o1kPzVPRiQH--f4HzrMMNPojT078CSudqS9WQaEc,4279
 algokit_utils/deploy.py,sha256=BxIFPtZd1lO8o_JmQQDIKk0O93E_bE-ZzglEWXwbefw,35110
 algokit_utils/dispenser_api.py,sha256=BpwEhKDig6qz54wbO-htG8hmLxFIrvdzXpESUb7Y1zw,5584
 algokit_utils/logic_error.py,sha256=YeE70qHZ6WBeoKCXqnto3uBg8R4ODXiNZkLmfEmASQo,2617
 algokit_utils/models.py,sha256=iJUiV6eLq5N_FKki4X5ll5rYQslU_wSPiSTtl61Z1CI,12803
 algokit_utils/network_clients.py,sha256=O4nJ3ECms4hFbuB1X64nzTMNOfK1Uj2oyjKxeieri-g,5929
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-2.3.0b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-2.3.0b1.dist-info/METADATA,sha256=dybj019jKMUl-xvnqX0pKgaKzNT2snOiY_APCekP21Q,2207
-algokit_utils-2.3.0b1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-algokit_utils-2.3.0b1.dist-info/RECORD,,
+algokit_utils-2.3.0b2.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-2.3.0b2.dist-info/METADATA,sha256=o9prEi5x37Ryru-KqugNKOsQ3nQYLAeI7_TpzDpKrDE,2207
+algokit_utils-2.3.0b2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+algokit_utils-2.3.0b2.dist-info/RECORD,,
```

