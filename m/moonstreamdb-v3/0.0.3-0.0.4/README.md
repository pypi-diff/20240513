# Comparing `tmp/moonstreamdb-v3-0.0.3.tar.gz` & `tmp/moonstreamdb-v3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstreamdb-v3-0.0.3.tar", last modified: Thu Apr 25 09:42:18 2024, max compression
+gzip compressed data, was "moonstreamdb-v3-0.0.4.tar", last modified: Mon May 13 12:33:34 2024, max compression
```

## Comparing `moonstreamdb-v3-0.0.3.tar` & `moonstreamdb-v3-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 09:42:18.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-25 09:42:18.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:42:18.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:42:08.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 09:42:18.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 09:42:18.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/moonstreamdbv3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)    49749 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:33:34.527914 moonstreamdb-v3-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-13 12:33:34.527914 moonstreamdb-v3-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:33:34.527914 moonstreamdb-v3-0.0.4/moonstreamdb_v3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-13 12:33:34.000000 moonstreamdb-v3-0.0.4/moonstreamdb_v3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-13 12:33:34.000000 moonstreamdb-v3-0.0.4/moonstreamdb_v3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:33:34.000000 moonstreamdb-v3-0.0.4/moonstreamdb_v3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:33:24.000000 moonstreamdb-v3-0.0.4/moonstreamdb_v3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 12:33:34.000000 moonstreamdb-v3-0.0.4/moonstreamdb_v3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 12:33:34.000000 moonstreamdb-v3-0.0.4/moonstreamdb_v3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:33:34.527914 moonstreamdb-v3-0.0.4/moonstreamdbv3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/moonstreamdbv3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:33:34.527914 moonstreamdb-v3-0.0.4/moonstreamdbv3/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/moonstreamdbv3/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/moonstreamdbv3/alembic/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:33:34.527914 moonstreamdb-v3-0.0.4/moonstreamdbv3/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)    49749 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/moonstreamdbv3/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/moonstreamdbv3/alembic/versions/e9f640a2b45b_arbitrum_one_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/moonstreamdbv3/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/moonstreamdbv3/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/moonstreamdbv3/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:33:34.527914 moonstreamdb-v3-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-13 12:33:20.000000 moonstreamdb-v3-0.0.4/setup.py
```

### Comparing `moonstreamdb-v3-0.0.3/PKG-INFO` & `moonstreamdb-v3-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb-v3
-Version: 0.0.3
+Version: 0.0.4
 Summary: Moonstream V3 database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstreamdb-v3
```

### Comparing `moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/PKG-INFO` & `moonstreamdb-v3-0.0.4/moonstreamdb_v3.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb-v3
-Version: 0.0.3
+Version: 0.0.4
 Summary: Moonstream V3 database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstreamdb-v3
```

### Comparing `moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/SOURCES.txt` & `moonstreamdb-v3-0.0.4/moonstreamdb_v3.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 moonstreamdbv3/db.py
 moonstreamdbv3/models.py
 moonstreamdbv3/version.py
 moonstreamdbv3/alembic/__init__.py
 moonstreamdbv3/alembic/env.py
 moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py
 moonstreamdbv3/alembic/versions/__init__.py
-moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py
+moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py
+moonstreamdbv3/alembic/versions/e9f640a2b45b_arbitrum_one_blockchain.py
```

### Comparing `moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/env.py` & `moonstreamdb-v3-0.0.4/moonstreamdbv3/alembic/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     MumbaiLabel,
     AmoyLabel,
     XDaiLabel,
     ZkSyncEraLabel,
     ZkSyncEraSepoliaLabel,
     BaseLabel,
     ArbitrumNovaLabel,
+    ArbitrumOneLabel,
     ArbitrumSepoliaLabel,
     XaiLabel,
     XaiSepoliaLabel,
     AvalancheLabel,
     AvalancheFujiLabel,
     BlastLabel,
     BlastSepoliaLabel,
```

### Comparing `moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py` & `moonstreamdb-v3-0.0.4/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py` & `moonstreamdb-v3-0.0.4/moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.3/moonstreamdbv3/db.py` & `moonstreamdb-v3-0.0.4/moonstreamdbv3/db.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.3/moonstreamdbv3/models.py` & `moonstreamdb-v3-0.0.4/moonstreamdbv3/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,14 +303,33 @@
             "address",
             "block_timestamp",
             unique=False,
         ),
     )
 
 
+class ArbitrumOneLabel(EvmBasedLabel):  # type: ignore
+    __tablename__ = "arbitrum_one_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_arbitrum_one_labels_addr_block_num",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_arbitrum_one_labels_addr_block_ts",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+
 class ArbitrumSepoliaLabel(EvmBasedLabel):  # type: ignore
     __tablename__ = "arbitrum_sepolia_labels"
 
     __table_args__ = (
         Index(
             "ix_arbitrum_sepolia_labels_addr_block_num",
             "address",
```

### Comparing `moonstreamdb-v3-0.0.3/setup.py` & `moonstreamdb-v3-0.0.4/setup.py`

 * *Files identical despite different names*

