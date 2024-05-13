# Comparing `tmp/stakefish_web3_utils-0.7.1.tar.gz` & `tmp/stakefish_web3_utils-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stakefish_web3_utils-0.7.1.tar", last modified: Wed May  1 14:37:34 2024, max compression
+gzip compressed data, was "stakefish_web3_utils-0.7.4.tar", last modified: Mon May 13 12:34:20 2024, max compression
```

## Comparing `stakefish_web3_utils-0.7.1.tar` & `stakefish_web3_utils-0.7.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 fishy      (501) staff       (20)        0 2024-05-01 14:37:34.242426 stakefish_web3_utils-0.7.1/
--rw-r--r--   0 fishy      (501) staff       (20)     1082 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/LICENSE.md
--rw-r--r--   0 fishy      (501) staff       (20)     1581 2024-05-01 14:37:34.242349 stakefish_web3_utils-0.7.1/PKG-INFO
--rw-r--r--   0 fishy      (501) staff       (20)      810 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/README.rst
--rw-r--r--   0 fishy      (501) staff       (20)      187 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/pyproject.toml
--rw-r--r--   0 fishy      (501) staff       (20)      811 2024-05-01 14:37:34.242816 stakefish_web3_utils-0.7.1/setup.cfg
-drwxr-xr-x   0 fishy      (501) staff       (20)        0 2024-05-01 14:37:34.241898 stakefish_web3_utils-0.7.1/stakefish_web3_utils.egg-info/
--rw-r--r--   0 fishy      (501) staff       (20)     1581 2024-05-01 14:37:34.000000 stakefish_web3_utils-0.7.1/stakefish_web3_utils.egg-info/PKG-INFO
--rw-r--r--   0 fishy      (501) staff       (20)     1186 2024-05-01 14:37:34.000000 stakefish_web3_utils-0.7.1/stakefish_web3_utils.egg-info/SOURCES.txt
--rw-r--r--   0 fishy      (501) staff       (20)        1 2024-05-01 14:37:34.000000 stakefish_web3_utils-0.7.1/stakefish_web3_utils.egg-info/dependency_links.txt
--rw-r--r--   0 fishy      (501) staff       (20)        1 2024-05-01 14:37:34.000000 stakefish_web3_utils-0.7.1/stakefish_web3_utils.egg-info/not-zip-safe
--rw-r--r--   0 fishy      (501) staff       (20)       76 2024-05-01 14:37:34.000000 stakefish_web3_utils-0.7.1/stakefish_web3_utils.egg-info/requires.txt
--rw-r--r--   0 fishy      (501) staff       (20)       11 2024-05-01 14:37:34.000000 stakefish_web3_utils-0.7.1/stakefish_web3_utils.egg-info/top_level.txt
-drwxr-xr-x   0 fishy      (501) staff       (20)        0 2024-05-01 14:37:34.238834 stakefish_web3_utils-0.7.1/tests/
--rw-r--r--   0 fishy      (501) staff       (20)     3412 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_async_beacon.py
--rw-r--r--   0 fishy      (501) staff       (20)      207 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_compute_time_at_slot.py
--rw-r--r--   0 fishy      (501) staff       (20)      269 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_convert_to_standard_notation.py
--rw-r--r--   0 fishy      (501) staff       (20)      635 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_divide_chunks.py
--rw-r--r--   0 fishy      (501) staff       (20)     2964 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_gitlab.py
--rw-r--r--   0 fishy      (501) staff       (20)      320 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_gwei_to_wei.py
--rw-r--r--   0 fishy      (501) staff       (20)      228 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_hash_event_param.py
--rw-r--r--   0 fishy      (501) staff       (20)      256 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_is_null_address.py
--rw-r--r--   0 fishy      (501) staff       (20)     1535 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_load_public_keys_from_files.py
--rw-r--r--   0 fishy      (501) staff       (20)      289 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_normalize_address.py
--rw-r--r--   0 fishy      (501) staff       (20)     4429 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_retryable_eth_module.py
--rw-r--r--   0 fishy      (501) staff       (20)      628 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/tests/test_split_validator_pubkey_bytes.py
-drwxr-xr-x   0 fishy      (501) staff       (20)        0 2024-05-01 14:37:34.241429 stakefish_web3_utils-0.7.1/web3_utils/
--rw-r--r--   0 fishy      (501) staff       (20)        0 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/__init__.py
--rw-r--r--   0 fishy      (501) staff       (20)     3769 2024-05-01 12:18:07.000000 stakefish_web3_utils-0.7.1/web3_utils/async_beacon.py
--rw-r--r--   0 fishy      (501) staff       (20)      343 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/calculate_max_fees.py
--rw-r--r--   0 fishy      (501) staff       (20)      130 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/compute_time_at_slot.py
--rw-r--r--   0 fishy      (501) staff       (20)      168 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/convert_to_standard_notation.py
--rw-r--r--   0 fishy      (501) staff       (20)      284 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/current_utc_timestamp.py
--rw-r--r--   0 fishy      (501) staff       (20)      138 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/divide_chunks.py
--rw-r--r--   0 fishy      (501) staff       (20)     1367 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/gitlab.py
--rw-r--r--   0 fishy      (501) staff       (20)      111 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/gwei_to_wei.py
--rw-r--r--   0 fishy      (501) staff       (20)      126 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/hash_event_param.py
--rw-r--r--   0 fishy      (501) staff       (20)      241 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/is_null_address.py
--rw-r--r--   0 fishy      (501) staff       (20)     1418 2024-05-01 14:11:03.000000 stakefish_web3_utils-0.7.1/web3_utils/load_public_keys_from_files.py
--rw-r--r--   0 fishy      (501) staff       (20)      301 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/normalize_address.py
--rw-r--r--   0 fishy      (501) staff       (20)     3547 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/retryable_eth_module.py
--rw-r--r--   0 fishy      (501) staff       (20)      336 2024-04-11 09:11:47.000000 stakefish_web3_utils-0.7.1/web3_utils/split_validator_pubkey_bytes.py
+drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2024-05-13 12:34:20.617136 stakefish_web3_utils-0.7.4/
+-rw-r--r--   0 stakefish   (502) staff       (20)     1082 2023-01-12 15:11:34.000000 stakefish_web3_utils-0.7.4/LICENSE.md
+-rw-r--r--   0 stakefish   (502) staff       (20)     1581 2024-05-13 12:34:20.616932 stakefish_web3_utils-0.7.4/PKG-INFO
+-rw-r--r--   0 stakefish   (502) staff       (20)      810 2023-01-12 15:11:34.000000 stakefish_web3_utils-0.7.4/README.rst
+-rw-r--r--   0 stakefish   (502) staff       (20)      187 2023-01-04 12:28:25.000000 stakefish_web3_utils-0.7.4/pyproject.toml
+-rw-r--r--   0 stakefish   (502) staff       (20)      811 2024-05-13 12:34:20.617874 stakefish_web3_utils-0.7.4/setup.cfg
+drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2024-05-13 12:34:20.615529 stakefish_web3_utils-0.7.4/stakefish_web3_utils.egg-info/
+-rw-r--r--   0 stakefish   (502) staff       (20)     1581 2024-05-13 12:34:20.000000 stakefish_web3_utils-0.7.4/stakefish_web3_utils.egg-info/PKG-INFO
+-rw-r--r--   0 stakefish   (502) staff       (20)     1186 2024-05-13 12:34:20.000000 stakefish_web3_utils-0.7.4/stakefish_web3_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 stakefish   (502) staff       (20)        1 2024-05-13 12:34:20.000000 stakefish_web3_utils-0.7.4/stakefish_web3_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 stakefish   (502) staff       (20)        1 2024-05-13 12:34:20.000000 stakefish_web3_utils-0.7.4/stakefish_web3_utils.egg-info/not-zip-safe
+-rw-r--r--   0 stakefish   (502) staff       (20)       76 2024-05-13 12:34:20.000000 stakefish_web3_utils-0.7.4/stakefish_web3_utils.egg-info/requires.txt
+-rw-r--r--   0 stakefish   (502) staff       (20)       11 2024-05-13 12:34:20.000000 stakefish_web3_utils-0.7.4/stakefish_web3_utils.egg-info/top_level.txt
+drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2024-05-13 12:34:20.603559 stakefish_web3_utils-0.7.4/tests/
+-rw-r--r--   0 stakefish   (502) staff       (20)     3412 2024-05-13 12:29:32.000000 stakefish_web3_utils-0.7.4/tests/test_async_beacon.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      207 2023-01-12 12:30:57.000000 stakefish_web3_utils-0.7.4/tests/test_compute_time_at_slot.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      269 2023-01-12 12:30:57.000000 stakefish_web3_utils-0.7.4/tests/test_convert_to_standard_notation.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      635 2023-01-04 12:28:25.000000 stakefish_web3_utils-0.7.4/tests/test_divide_chunks.py
+-rw-r--r--   0 stakefish   (502) staff       (20)     2964 2024-05-13 12:24:07.000000 stakefish_web3_utils-0.7.4/tests/test_gitlab.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      320 2023-01-06 17:01:52.000000 stakefish_web3_utils-0.7.4/tests/test_gwei_to_wei.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      228 2023-01-12 12:30:57.000000 stakefish_web3_utils-0.7.4/tests/test_hash_event_param.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      256 2024-05-13 12:24:07.000000 stakefish_web3_utils-0.7.4/tests/test_is_null_address.py
+-rw-r--r--   0 stakefish   (502) staff       (20)     1535 2024-05-13 12:24:07.000000 stakefish_web3_utils-0.7.4/tests/test_load_public_keys_from_files.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      289 2023-01-06 17:01:52.000000 stakefish_web3_utils-0.7.4/tests/test_normalize_address.py
+-rw-r--r--   0 stakefish   (502) staff       (20)     4429 2024-05-13 12:24:07.000000 stakefish_web3_utils-0.7.4/tests/test_retryable_eth_module.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      628 2024-05-13 12:24:07.000000 stakefish_web3_utils-0.7.4/tests/test_split_validator_pubkey_bytes.py
+drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2024-05-13 12:34:20.614494 stakefish_web3_utils-0.7.4/web3_utils/
+-rw-r--r--   0 stakefish   (502) staff       (20)        0 2023-01-04 12:28:25.000000 stakefish_web3_utils-0.7.4/web3_utils/__init__.py
+-rw-r--r--   0 stakefish   (502) staff       (20)     3986 2024-05-13 12:28:38.000000 stakefish_web3_utils-0.7.4/web3_utils/async_beacon.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      343 2023-01-06 17:01:52.000000 stakefish_web3_utils-0.7.4/web3_utils/calculate_max_fees.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      130 2023-01-06 17:01:52.000000 stakefish_web3_utils-0.7.4/web3_utils/compute_time_at_slot.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      168 2023-03-30 10:43:41.000000 stakefish_web3_utils-0.7.4/web3_utils/convert_to_standard_notation.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      284 2023-01-06 17:01:52.000000 stakefish_web3_utils-0.7.4/web3_utils/current_utc_timestamp.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      138 2024-05-13 12:24:07.000000 stakefish_web3_utils-0.7.4/web3_utils/divide_chunks.py
+-rw-r--r--   0 stakefish   (502) staff       (20)     1367 2024-05-13 12:24:07.000000 stakefish_web3_utils-0.7.4/web3_utils/gitlab.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      111 2023-01-06 17:01:52.000000 stakefish_web3_utils-0.7.4/web3_utils/gwei_to_wei.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      126 2023-01-06 17:01:52.000000 stakefish_web3_utils-0.7.4/web3_utils/hash_event_param.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      241 2024-05-13 12:24:07.000000 stakefish_web3_utils-0.7.4/web3_utils/is_null_address.py
+-rw-r--r--   0 stakefish   (502) staff       (20)     1418 2024-05-13 12:24:38.000000 stakefish_web3_utils-0.7.4/web3_utils/load_public_keys_from_files.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      301 2023-01-06 17:01:52.000000 stakefish_web3_utils-0.7.4/web3_utils/normalize_address.py
+-rw-r--r--   0 stakefish   (502) staff       (20)     3547 2024-05-13 12:24:07.000000 stakefish_web3_utils-0.7.4/web3_utils/retryable_eth_module.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      336 2024-05-13 12:24:07.000000 stakefish_web3_utils-0.7.4/web3_utils/split_validator_pubkey_bytes.py
```

### Comparing `stakefish_web3_utils-0.7.1/LICENSE.md` & `stakefish_web3_utils-0.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stakefish_web3_utils-0.7.1/PKG-INFO` & `stakefish_web3_utils-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stakefish-web3-utils
-Version: 0.7.1
+Version: 0.7.4
 Summary: Stakefish’s web3 utils for Python
 Home-page: https://github.com/stakefish/web3-utils
 Author: Michal Baranowski <mbaranovski@stake.fish>, Mateusz Sokola <mateusz@stake.fish>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `stakefish_web3_utils-0.7.1/README.rst` & `stakefish_web3_utils-0.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `stakefish_web3_utils-0.7.1/setup.cfg` & `stakefish_web3_utils-0.7.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = stakefish-web3-utils
-version = 0.7.1
+version = 0.7.4
 description = Stakefish’s web3 utils for Python
 author = Michal Baranowski <mbaranovski@stake.fish>, Mateusz Sokola <mateusz@stake.fish>
 url = https://github.com/stakefish/web3-utils
 long_description = file: README.rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
```

### Comparing `stakefish_web3_utils-0.7.1/stakefish_web3_utils.egg-info/PKG-INFO` & `stakefish_web3_utils-0.7.4/stakefish_web3_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stakefish-web3-utils
-Version: 0.7.1
+Version: 0.7.4
 Summary: Stakefish’s web3 utils for Python
 Home-page: https://github.com/stakefish/web3-utils
 Author: Michal Baranowski <mbaranovski@stake.fish>, Mateusz Sokola <mateusz@stake.fish>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `stakefish_web3_utils-0.7.1/stakefish_web3_utils.egg-info/SOURCES.txt` & `stakefish_web3_utils-0.7.4/stakefish_web3_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stakefish_web3_utils-0.7.1/tests/test_async_beacon.py` & `stakefish_web3_utils-0.7.4/tests/test_async_beacon.py`

 * *Files identical despite different names*

### Comparing `stakefish_web3_utils-0.7.1/tests/test_divide_chunks.py` & `stakefish_web3_utils-0.7.4/tests/test_divide_chunks.py`

 * *Files identical despite different names*

### Comparing `stakefish_web3_utils-0.7.1/tests/test_gitlab.py` & `stakefish_web3_utils-0.7.4/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `stakefish_web3_utils-0.7.1/tests/test_load_public_keys_from_files.py` & `stakefish_web3_utils-0.7.4/tests/test_load_public_keys_from_files.py`

 * *Files identical despite different names*

### Comparing `stakefish_web3_utils-0.7.1/tests/test_retryable_eth_module.py` & `stakefish_web3_utils-0.7.4/tests/test_retryable_eth_module.py`

 * *Files identical despite different names*

### Comparing `stakefish_web3_utils-0.7.1/tests/test_split_validator_pubkey_bytes.py` & `stakefish_web3_utils-0.7.4/tests/test_split_validator_pubkey_bytes.py`

 * *Files identical despite different names*

### Comparing `stakefish_web3_utils-0.7.1/web3_utils/async_beacon.py` & `stakefish_web3_utils-0.7.4/web3_utils/async_beacon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import logging
 from typing import Any, Dict, List, Callable
 
-from requests import HTTPError, ConnectionError
+from requests import HTTPError, ConnectionError, Session
 from tenacity import retry, retry_if_exception, wait_fixed, before_sleep_log, retry_any, retry_if_exception_type, stop_never
 from web3.beacon import Beacon
 
 
 def with_retry(f):
     async def wrapper(*args):
         retry_stop = args[0].retry_stop
@@ -31,14 +31,21 @@
 class AsyncBeacon(Beacon):
     def __init__(self, base_url: str, logger: logging.Logger, retry_stop: Callable or None = None):
         super().__init__(base_url)
         self.retry_stop = retry_stop
         self.logger = logger
         self.cache = {}
 
+    def update_base_url(self, base_url: str):
+        self.base_url = base_url
+        self.session = Session()
+
+    async def get_syncing(self):
+        return await self._run_as_async(super().get_syncing)
+
     async def get_finality_checkpoint(self, state_id: str = "head"):
         return await self._run_as_async(super().get_finality_checkpoint, state_id)
 
     async def get_genesis(self) -> int:
         if "genesis_time" not in self.cache:
             genesis = await self._run_as_async(super().get_genesis)
             self.cache["genesis_time"] = int(genesis["data"]["genesis_time"])
```

### Comparing `stakefish_web3_utils-0.7.1/web3_utils/gitlab.py` & `stakefish_web3_utils-0.7.4/web3_utils/gitlab.py`

 * *Files identical despite different names*

### Comparing `stakefish_web3_utils-0.7.1/web3_utils/load_public_keys_from_files.py` & `stakefish_web3_utils-0.7.4/web3_utils/load_public_keys_from_files.py`

 * *Files identical despite different names*

### Comparing `stakefish_web3_utils-0.7.1/web3_utils/retryable_eth_module.py` & `stakefish_web3_utils-0.7.4/web3_utils/retryable_eth_module.py`

 * *Files identical despite different names*

