# Comparing `tmp/backpack_exchange_sdk-0.3.1.tar.gz` & `tmp/backpack_exchange_sdk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backpack_exchange_sdk-0.3.1.tar", last modified: Tue Apr  2 16:14:22 2024, max compression
+gzip compressed data, was "backpack_exchange_sdk-0.3.2.tar", last modified: Mon May 13 15:19:42 2024, max compression
```

## Comparing `backpack_exchange_sdk-0.3.1.tar` & `backpack_exchange_sdk-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:14:22.146412 backpack_exchange_sdk-0.3.1/
--rw-r--r--   0 solomeowl   (501) staff       (20)     1066 2024-03-08 15:43:17.000000 backpack_exchange_sdk-0.3.1/LICENSE
--rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 16:14:22.146150 backpack_exchange_sdk-0.3.1/PKG-INFO
--rw-r--r--   0 solomeowl   (501) staff       (20)     2119 2024-04-02 15:44:43.000000 backpack_exchange_sdk-0.3.1/README.md
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:14:22.141143 backpack_exchange_sdk-0.3.1/backpack_exchange_sdk/
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:07:47.000000 backpack_exchange_sdk-0.3.1/backpack_exchange_sdk/__init__.py
--rw-r--r--   0 solomeowl   (501) staff       (20)     9392 2024-04-02 16:13:12.000000 backpack_exchange_sdk-0.3.1/backpack_exchange_sdk/authenticated.py
--rw-r--r--   0 solomeowl   (501) staff       (20)     3754 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.3.1/backpack_exchange_sdk/public.py
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:14:22.145850 backpack_exchange_sdk-0.3.1/backpack_exchange_sdk.egg-info/
--rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 16:14:22.000000 backpack_exchange_sdk-0.3.1/backpack_exchange_sdk.egg-info/PKG-INFO
--rw-r--r--   0 solomeowl   (501) staff       (20)      423 2024-04-02 16:14:22.000000 backpack_exchange_sdk-0.3.1/backpack_exchange_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 solomeowl   (501) staff       (20)        1 2024-04-02 16:14:22.000000 backpack_exchange_sdk-0.3.1/backpack_exchange_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 solomeowl   (501) staff       (20)       28 2024-04-02 16:14:22.000000 backpack_exchange_sdk-0.3.1/backpack_exchange_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:14:22.145289 backpack_exchange_sdk-0.3.1/enums/
--rw-r--r--   0 solomeowl   (501) staff       (20)      368 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.3.1/enums/RequestEnums.py
--rw-r--r--   0 solomeowl   (501) staff       (20)      248 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.3.1/enums/ResponseEnums.py
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:07:48.000000 backpack_exchange_sdk-0.3.1/enums/__init__.py
--rw-r--r--   0 solomeowl   (501) staff       (20)       38 2024-04-02 16:14:22.146467 backpack_exchange_sdk-0.3.1/setup.cfg
--rw-r--r--   0 solomeowl   (501) staff       (20)      533 2024-04-02 16:14:04.000000 backpack_exchange_sdk-0.3.1/setup.py
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:14:22.145640 backpack_exchange_sdk-0.3.1/tests/
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.3.1/tests/test_authenticated.py
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.3.1/tests/test_public.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-05-13 15:19:42.846933 backpack_exchange_sdk-0.3.2/
+-rw-r--r--   0 solomeowl   (501) staff       (20)     1066 2024-03-08 15:43:17.000000 backpack_exchange_sdk-0.3.2/LICENSE
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-05-13 15:19:42.846644 backpack_exchange_sdk-0.3.2/PKG-INFO
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2119 2024-04-02 15:44:43.000000 backpack_exchange_sdk-0.3.2/README.md
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-05-13 15:19:42.844367 backpack_exchange_sdk-0.3.2/backpack_exchange_sdk/
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:07:47.000000 backpack_exchange_sdk-0.3.2/backpack_exchange_sdk/__init__.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)     9764 2024-05-13 15:15:13.000000 backpack_exchange_sdk-0.3.2/backpack_exchange_sdk/authenticated.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)     3754 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.3.2/backpack_exchange_sdk/public.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-05-13 15:19:42.846369 backpack_exchange_sdk-0.3.2/backpack_exchange_sdk.egg-info/
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-05-13 15:19:42.000000 backpack_exchange_sdk-0.3.2/backpack_exchange_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 solomeowl   (501) staff       (20)      423 2024-05-13 15:19:42.000000 backpack_exchange_sdk-0.3.2/backpack_exchange_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 solomeowl   (501) staff       (20)        1 2024-05-13 15:19:42.000000 backpack_exchange_sdk-0.3.2/backpack_exchange_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 solomeowl   (501) staff       (20)       28 2024-05-13 15:19:42.000000 backpack_exchange_sdk-0.3.2/backpack_exchange_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-05-13 15:19:42.845932 backpack_exchange_sdk-0.3.2/enums/
+-rw-r--r--   0 solomeowl   (501) staff       (20)      368 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.3.2/enums/RequestEnums.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)      248 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.3.2/enums/ResponseEnums.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:24:21.000000 backpack_exchange_sdk-0.3.2/enums/__init__.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)       38 2024-05-13 15:19:42.846990 backpack_exchange_sdk-0.3.2/setup.cfg
+-rw-r--r--   0 solomeowl   (501) staff       (20)      533 2024-05-13 15:18:58.000000 backpack_exchange_sdk-0.3.2/setup.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-05-13 15:19:42.846186 backpack_exchange_sdk-0.3.2/tests/
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.3.2/tests/test_authenticated.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.3.2/tests/test_public.py
```

### Comparing `backpack_exchange_sdk-0.3.1/LICENSE` & `backpack_exchange_sdk-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.3.1/PKG-INFO` & `backpack_exchange_sdk-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpack_exchange_sdk
-Version: 0.3.1
+Version: 0.3.2
 Summary: A simple SDK for backpack exchange
 Home-page: https://github.com/solomeowl/backpack_exchange_sdk
 Author: solomeowl
 Author-email: j19940430@gmail.com
 Project-URL: Source, https://github.com/solomeowl/backpack_exchange_sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `backpack_exchange_sdk-0.3.1/README.md` & `backpack_exchange_sdk-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.3.1/backpack_exchange_sdk/authenticated.py` & `backpack_exchange_sdk-0.3.2/backpack_exchange_sdk/authenticated.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,33 +66,41 @@
     def get_balances(self):
         """
         Retrieves account balances and the state of the balances (locked or available).
         Locked assets are those that are currently in an open order.
         """
         return self._send_request('GET', 'api/v1/capital', 'balanceQuery')
 
-    def get_deposits(self, limit: int = 100, offset: int = 0):
+    def get_deposits(self, fromTimestamp: int = False, toTimestamp: int = False, limit: int = 100, offset: int = 0):
         """
         Retrieves deposit history.
         """
         params = {'limit': limit, 'offset': offset}
+        if fromTimestamp:
+            params['from'] = fromTimestamp
+        if toTimestamp:
+            params['to'] = toTimestamp
         return self._send_request('GET', 'wapi/v1/capital/deposits', 'depositQueryAll', params)
 
     def get_deposit_address(self, blockchain_name: str):
         """
         Retrieves the user specific deposit address if the user were to deposit on the specified blockchain.
         """
         params = {'blockchain': blockchain_name}
         return self._send_request('GET', 'wapi/v1/capital/deposit/address', 'depositAddressQuery', params)
 
-    def get_withdrawals(self, limit: int = 100, offset: int = 0):
+    def get_withdrawals(self, fromTimestamp: int = False, toTimestamp: int = False, limit: int = 100, offset: int = 0):
         """
         Retrieves withdrawal history.
         """
         params = {'limit': limit, 'offset': offset}
+        if fromTimestamp:
+            params['from'] = fromTimestamp
+        if toTimestamp:
+            params['to'] = toTimestamp
         return self._send_request('GET', 'wapi/v1/capital/withdrawals', 'withdrawalQueryAll', params)
 
     def request_withdrawal(self, address: str,
                            blockchain: str,
                            quantity: str,
                            symbol: str,
                            client_id: str = None,
```

### Comparing `backpack_exchange_sdk-0.3.1/backpack_exchange_sdk/public.py` & `backpack_exchange_sdk-0.3.2/backpack_exchange_sdk/public.py`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.3.1/backpack_exchange_sdk.egg-info/PKG-INFO` & `backpack_exchange_sdk-0.3.2/backpack_exchange_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpack_exchange_sdk
-Version: 0.3.1
+Version: 0.3.2
 Summary: A simple SDK for backpack exchange
 Home-page: https://github.com/solomeowl/backpack_exchange_sdk
 Author: solomeowl
 Author-email: j19940430@gmail.com
 Project-URL: Source, https://github.com/solomeowl/backpack_exchange_sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `backpack_exchange_sdk-0.3.1/setup.py` & `backpack_exchange_sdk-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="backpack_exchange_sdk",
-    version="0.3.1",
+    version="0.3.2",
     author="solomeowl",
     author_email="j19940430@gmail.com",
     description="A simple SDK for backpack exchange",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/solomeowl/backpack_exchange_sdk",
     project_urls={
```

