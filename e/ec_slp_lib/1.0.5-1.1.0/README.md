# Comparing `tmp/ec_slp_lib-1.0.5.tar.gz` & `tmp/ec_slp_lib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec_slp_lib-1.0.5.tar", max compression
+gzip compressed data, was "ec_slp_lib-1.1.0.tar", max compression
```

## Comparing `ec_slp_lib-1.0.5.tar` & `ec_slp_lib-1.1.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     8314 2024-05-05 09:06:47.936651 ec_slp_lib-1.0.5/ec_slp_lib.py
--rw-r--r--   0        0        0      512 2024-05-05 09:06:21.465340 ec_slp_lib-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 ec_slp_lib-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     8314 2024-05-13 08:42:52.343181 ec_slp_lib-1.1.0/ec_slp_lib.py
+-rw-r--r--   0        0        0      512 2024-05-13 08:41:51.476743 ec_slp_lib-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 ec_slp_lib-1.1.0/PKG-INFO
```

### Comparing `ec_slp_lib-1.0.5/ec_slp_lib.py` & `ec_slp_lib-1.1.0/ec_slp_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 logger = logging.getLogger(__name__)
 
 __author__ = "uak"
 __copyright__ = "Copyright 2024"
 __credits__ = ["uak"]
 __license__ = "LGPL"
-__version__ = "1.0.5"
+__version__ = "1.1.0"
 
 
 class EcSLP:
     """EC SLP class
     """
     def set_rpc_port(self, params, rpc):
         """Set rpc port in Electron Cash config file
```

### Comparing `ec_slp_lib-1.0.5/pyproject.toml` & `ec_slp_lib-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ec_slp_lib"
-version = "1.0.5"
+version = "1.1.0"
 description = "Wrapper for Electron Cash commands based on its CLI and RPC commands"
 authors = ["uak <4626956-uak@users.noreply.gitlab.com>"]
 license = "LGPLv3+"
 repository = "https://gitlab.com/uak/electron-cash-slp-basic-lib"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ec_slp_lib-1.0.5/PKG-INFO` & `ec_slp_lib-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec_slp_lib
-Version: 1.0.5
+Version: 1.1.0
 Summary: Wrapper for Electron Cash commands based on its CLI and RPC commands
 Home-page: https://gitlab.com/uak/electron-cash-slp-basic-lib
 License: LGPLv3+
 Author: uak
 Author-email: 4626956-uak@users.noreply.gitlab.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

