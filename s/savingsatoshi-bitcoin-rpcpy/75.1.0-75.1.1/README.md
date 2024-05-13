# Comparing `tmp/savingsatoshi_bitcoin_rpcpy-75.1.0.tar.gz` & `tmp/savingsatoshi_bitcoin_rpcpy-75.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "savingsatoshi_bitcoin_rpcpy-75.1.0.tar", max compression
+gzip compressed data, was "savingsatoshi_bitcoin_rpcpy-75.1.1.tar", max compression
```

## Comparing `savingsatoshi_bitcoin_rpcpy-75.1.0.tar` & `savingsatoshi_bitcoin_rpcpy-75.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-04-17 16:06:23.379599 savingsatoshi_bitcoin_rpcpy-75.1.0/bitcoin_rpcpy/__init__.py
--rw-r--r--   0        0        0     2338 2024-04-17 16:33:18.778777 savingsatoshi_bitcoin_rpcpy-75.1.0/bitcoin_rpcpy/bitcoin_rpc.py
--rw-r--r--   0        0        0  5896269 2024-04-17 16:26:51.840678 savingsatoshi_bitcoin_rpcpy-75.1.0/bitcoin_rpcpy/chainstate.json
--rw-r--r--   0        0        0      378 2024-04-17 16:59:00.348409 savingsatoshi_bitcoin_rpcpy-75.1.0/pyproject.toml
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 savingsatoshi_bitcoin_rpcpy-75.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-17 16:06:23.379599 savingsatoshi_bitcoin_rpcpy-75.1.1/bitcoin_rpcpy/__init__.py
+-rw-r--r--   0        0        0     2336 2024-05-13 16:23:27.273401 savingsatoshi_bitcoin_rpcpy-75.1.1/bitcoin_rpcpy/bitcoin_rpc.py
+-rw-r--r--   0        0        0  5896269 2024-04-17 16:26:51.840678 savingsatoshi_bitcoin_rpcpy-75.1.1/bitcoin_rpcpy/chainstate.json
+-rw-r--r--   0        0        0      378 2024-05-13 16:23:50.685481 savingsatoshi_bitcoin_rpcpy-75.1.1/pyproject.toml
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 savingsatoshi_bitcoin_rpcpy-75.1.1/PKG-INFO
```

### Comparing `savingsatoshi_bitcoin_rpcpy-75.1.0/bitcoin_rpcpy/bitcoin_rpc.py` & `savingsatoshi_bitcoin_rpcpy-75.1.1/bitcoin_rpcpy/bitcoin_rpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from pathlib import Path
 
 class Bitcoin:
     def __init__(self):
         with open(f"{'chainstate.json'}", "r") as file:
             self.state = load(file)
 
-    @staticmethod
-    def rpc(method=None, params=None):
-        self = Bitcoin()
+    def rpc(self, method=None, params=None):
+        self = self = type(self)()
         if not method:
             raise Exception("First argument 'method' is required.\nExecute `rpc('help')` for help")
         if hasattr(self, method):
             func = getattr(self, method)
             if params:
                 return func(params)
             else:
```

### Comparing `savingsatoshi_bitcoin_rpcpy-75.1.0/bitcoin_rpcpy/chainstate.json` & `savingsatoshi_bitcoin_rpcpy-75.1.1/bitcoin_rpcpy/chainstate.json`

 * *Files identical despite different names*

