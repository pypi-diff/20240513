# Comparing `tmp/stac_asset-0.3.0.tar.gz` & `tmp/stac_asset-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_asset-0.3.0.tar", last modified: Wed Apr 24 13:06:45 2024, max compression
+gzip compressed data, was "stac_asset-0.3.1.tar", last modified: Mon May 13 14:33:06 2024, max compression
```

## Comparing `stac_asset-0.3.0.tar` & `stac_asset-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:45.243191 stac_asset-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 13:06:37.000000 stac_asset-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 13:06:37.000000 stac_asset-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 13:06:37.000000 stac_asset-0.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-24 13:06:45.243191 stac_asset-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-24 13:06:37.000000 stac_asset-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-24 13:06:37.000000 stac_asset-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:06:45.243191 stac_asset-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:45.235191 stac_asset-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:45.239191 stac_asset-0.3.0/src/stac_asset/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    18954 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:45.239191 stac_asset-0.3.0/src/stac_asset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:45.239191 stac_asset-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:06.182827 stac_asset-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 14:33:02.000000 stac_asset-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 14:33:02.000000 stac_asset-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-13 14:33:02.000000 stac_asset-0.3.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-05-13 14:33:06.182827 stac_asset-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-13 14:33:02.000000 stac_asset-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-13 14:33:02.000000 stac_asset-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:33:06.182827 stac_asset-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:06.174827 stac_asset-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:06.178827 stac_asset-0.3.1/src/stac_asset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18954 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:06.182827 stac_asset-0.3.1/src/stac_asset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:06.182827 stac_asset-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_validate.py
```

### Comparing `stac_asset-0.3.0/LICENSE` & `stac_asset-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/NOTICE` & `stac_asset-0.3.1/NOTICE`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/PKG-INFO` & `stac_asset-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.3.0
+Version: 0.3.1
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Github, https://github.com/stac-utils/stac-asset
 Project-URL: CHANGELOG, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/stac-utils/stac-asset/issues
 Keywords: stac,async
@@ -33,15 +33,15 @@
 Provides-Extra: dev
 Requires-Dist: mypy~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
 Requires-Dist: pystac[validation]>=1.8.4; extra == "dev"
 Requires-Dist: pytest~=7.3; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.21; extra == "dev"
 Requires-Dist: pytest-cov>=5.0; extra == "dev"
-Requires-Dist: ruff==0.4.1; extra == "dev"
+Requires-Dist: ruff==0.4.4; extra == "dev"
 Requires-Dist: types-aiofiles~=23.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9; extra == "dev"
 Requires-Dist: types-tqdm~=4.66.0; extra == "dev"
 Requires-Dist: types-tabulate~=0.9.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
 Requires-Dist: sphinx~=7.3; extra == "docs"
```

### Comparing `stac_asset-0.3.0/README.md` & `stac_asset-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/pyproject.toml` & `stac_asset-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stac-asset"
-version = "0.3.0"
+version = "0.3.1"
 description = "Read and download STAC assets across platforms and providers"
 authors = [{ name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }]
 readme = "README.md"
 keywords = ["stac", "async"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
@@ -35,15 +35,15 @@
 dev = [
     "mypy~=1.3",
     "pre-commit~=3.3",
     "pystac[validation]>=1.8.4",
     "pytest~=7.3",
     "pytest-asyncio~=0.21",
     "pytest-cov>=5.0",
-    "ruff==0.4.1",
+    "ruff==0.4.4",
     "types-aiofiles~=23.1",
     "types-python-dateutil~=2.9",
     "types-tqdm~=4.66.0",
     "types-tabulate~=0.9.0",
 ]
 docs = ["pydata-sphinx-theme~=0.13", "sphinx~=7.3", "sphinx-click~=5.0"]
```

### Comparing `stac_asset-0.3.0/src/stac_asset/__init__.py` & `stac_asset-0.3.1/src/stac_asset/__init__.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/_cli.py` & `stac_asset-0.3.1/src/stac_asset/_cli.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/_functions.py` & `stac_asset-0.3.1/src/stac_asset/_functions.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/blocking.py` & `stac_asset-0.3.1/src/stac_asset/blocking.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/client.py` & `stac_asset-0.3.1/src/stac_asset/client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/config.py` & `stac_asset-0.3.1/src/stac_asset/config.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/earthdata_client.py` & `stac_asset-0.3.1/src/stac_asset/earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/errors.py` & `stac_asset-0.3.1/src/stac_asset/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,9 +39,9 @@
 
     exceptions: List[Exception]
 
     def __init__(self, exceptions: List[Exception], *args: Any, **kwargs: Any) -> None:
         self.exceptions = exceptions
         messages = list()
         for exception in exceptions:
-            messages.append(str(exception))
+            messages.append(f"{type(exception).__name__}: {exception}")
         super().__init__("\n".join(messages), *args, **kwargs)
```

### Comparing `stac_asset-0.3.0/src/stac_asset/filesystem_client.py` & `stac_asset-0.3.1/src/stac_asset/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/http_client.py` & `stac_asset-0.3.1/src/stac_asset/http_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/messages.py` & `stac_asset-0.3.1/src/stac_asset/messages.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/planetary_computer_client.py` & `stac_asset-0.3.1/src/stac_asset/planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/s3_client.py` & `stac_asset-0.3.1/src/stac_asset/s3_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/strategy.py` & `stac_asset-0.3.1/src/stac_asset/strategy.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/types.py` & `stac_asset-0.3.1/src/stac_asset/types.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset/validate.py` & `stac_asset-0.3.1/src/stac_asset/validate.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/src/stac_asset.egg-info/PKG-INFO` & `stac_asset-0.3.1/src/stac_asset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.3.0
+Version: 0.3.1
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Github, https://github.com/stac-utils/stac-asset
 Project-URL: CHANGELOG, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/stac-utils/stac-asset/issues
 Keywords: stac,async
@@ -33,15 +33,15 @@
 Provides-Extra: dev
 Requires-Dist: mypy~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
 Requires-Dist: pystac[validation]>=1.8.4; extra == "dev"
 Requires-Dist: pytest~=7.3; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.21; extra == "dev"
 Requires-Dist: pytest-cov>=5.0; extra == "dev"
-Requires-Dist: ruff==0.4.1; extra == "dev"
+Requires-Dist: ruff==0.4.4; extra == "dev"
 Requires-Dist: types-aiofiles~=23.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9; extra == "dev"
 Requires-Dist: types-tqdm~=4.66.0; extra == "dev"
 Requires-Dist: types-tabulate~=0.9.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
 Requires-Dist: sphinx~=7.3; extra == "docs"
```

### Comparing `stac_asset-0.3.0/src/stac_asset.egg-info/SOURCES.txt` & `stac_asset-0.3.1/src/stac_asset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/tests/test_blocking.py` & `stac_asset-0.3.1/tests/test_blocking.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/tests/test_cli.py` & `stac_asset-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/tests/test_earthdata_client.py` & `stac_asset-0.3.1/tests/test_earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/tests/test_filesystem_client.py` & `stac_asset-0.3.1/tests/test_filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/tests/test_functions.py` & `stac_asset-0.3.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/tests/test_planetary_computer_client.py` & `stac_asset-0.3.1/tests/test_planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/tests/test_s3_client.py` & `stac_asset-0.3.1/tests/test_s3_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.0/tests/test_validate.py` & `stac_asset-0.3.1/tests/test_validate.py`

 * *Files identical despite different names*

