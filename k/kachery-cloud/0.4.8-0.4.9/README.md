# Comparing `tmp/kachery_cloud-0.4.8.tar.gz` & `tmp/kachery_cloud-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kachery_cloud-0.4.8.tar", last modified: Mon Mar  4 21:45:16 2024, max compression
+gzip compressed data, was "kachery_cloud-0.4.9.tar", last modified: Mon May 13 18:36:48 2024, max compression
```

## Comparing `kachery_cloud-0.4.8.tar` & `kachery_cloud-0.4.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-03-04 21:45:16.760954 kachery_cloud-0.4.8/
--rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/LICENSE
--rw-r--r--   0 magland   (1000) magland   (1000)      626 2024-03-04 21:45:16.760954 kachery_cloud-0.4.8/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)     5345 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/README.md
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-03-04 21:45:16.760954 kachery_cloud-0.4.8/kachery_cloud/
--rw-rw-r--   0 magland   (1000) magland   (1000)     1465 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/TemporaryDirectory.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1029 2024-01-10 16:46:42.000000 kachery_cloud-0.4.8/kachery_cloud/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     6265 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/_client_keys.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      780 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/_custom_storage_backend.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1065 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/_fs_operations.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1136 2024-01-09 18:22:25.000000 kachery_cloud-0.4.8/kachery_cloud/_get_kachery_gateway_url.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      707 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/_get_local_client_config.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      843 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/_json_stringify_deterministic.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1058 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/_kachery_gateway_request.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1896 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/_load_github_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2391 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/_safe_pickle.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2348 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/_serialize.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      217 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/_sha1_of_dict.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      136 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/_sha1_of_string.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      658 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/admin_delete_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      442 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/cat_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2394 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/cli.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3615 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/core.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      141 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/get_client_id.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2258 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/get_kachery_cloud_dir.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3259 2024-03-04 21:44:20.000000 kachery_cloud-0.4.8/kachery_cloud/init.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1102 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/link_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1276 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/load_bytes.py
--rw-rw-r--   0 magland   (1000) magland   (1000)    10706 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/load_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2878 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/mutable_local.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3185 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/request_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     4277 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/store_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3835 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/store_file_local.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-03-04 21:45:16.760954 kachery_cloud-0.4.8/kachery_cloud/zenodo_upload/
--rw-rw-r--   0 magland   (1000) magland   (1000)        0 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/zenodo_upload/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     5225 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/kachery_cloud/zenodo_upload/zenodo_upload.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-03-04 21:45:16.760954 kachery_cloud-0.4.8/kachery_cloud.egg-info/
--rw-r--r--   0 magland   (1000) magland   (1000)      626 2024-03-04 21:45:16.000000 kachery_cloud-0.4.8/kachery_cloud.egg-info/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)     1241 2024-03-04 21:45:16.000000 kachery_cloud-0.4.8/kachery_cloud.egg-info/SOURCES.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        1 2024-03-04 21:45:16.000000 kachery_cloud-0.4.8/kachery_cloud.egg-info/dependency_links.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)      670 2024-03-04 21:45:16.000000 kachery_cloud-0.4.8/kachery_cloud.egg-info/entry_points.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       71 2024-03-04 21:45:16.000000 kachery_cloud-0.4.8/kachery_cloud.egg-info/requires.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       14 2024-03-04 21:45:16.000000 kachery_cloud-0.4.8/kachery_cloud.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)      490 2024-03-04 21:45:16.764953 kachery_cloud-0.4.8/setup.cfg
--rw-rw-r--   0 magland   (1000) magland   (1000)     1189 2024-01-09 14:21:07.000000 kachery_cloud-0.4.8/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-05-13 18:36:48.747841 kachery_cloud-0.4.9/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/LICENSE
+-rw-r--r--   0 magland   (1000) magland   (1000)      626 2024-05-13 18:36:48.747841 kachery_cloud-0.4.9/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)     5345 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/README.md
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-05-13 18:36:48.747841 kachery_cloud-0.4.9/kachery_cloud/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1465 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/TemporaryDirectory.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1029 2024-01-10 16:46:42.000000 kachery_cloud-0.4.9/kachery_cloud/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     6265 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/_client_keys.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      780 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/_custom_storage_backend.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1065 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/_fs_operations.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1136 2024-01-09 18:22:25.000000 kachery_cloud-0.4.9/kachery_cloud/_get_kachery_gateway_url.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      707 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/_get_local_client_config.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      843 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/_json_stringify_deterministic.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1058 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/_kachery_gateway_request.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1896 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/_load_github_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2391 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/_safe_pickle.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2348 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/_serialize.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      217 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/_sha1_of_dict.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      136 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/_sha1_of_string.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      658 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/admin_delete_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      442 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/cat_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2394 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/cli.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3615 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/core.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      141 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/get_client_id.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2258 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/get_kachery_cloud_dir.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3616 2024-05-13 18:35:55.000000 kachery_cloud-0.4.9/kachery_cloud/init.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1102 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/link_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1276 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/load_bytes.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)    10706 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/load_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2878 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/mutable_local.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3185 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/request_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     4277 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/store_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3835 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/store_file_local.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-05-13 18:36:48.747841 kachery_cloud-0.4.9/kachery_cloud/zenodo_upload/
+-rw-rw-r--   0 magland   (1000) magland   (1000)        0 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/zenodo_upload/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     5225 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/kachery_cloud/zenodo_upload/zenodo_upload.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-05-13 18:36:48.747841 kachery_cloud-0.4.9/kachery_cloud.egg-info/
+-rw-r--r--   0 magland   (1000) magland   (1000)      626 2024-05-13 18:36:48.000000 kachery_cloud-0.4.9/kachery_cloud.egg-info/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1241 2024-05-13 18:36:48.000000 kachery_cloud-0.4.9/kachery_cloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        1 2024-05-13 18:36:48.000000 kachery_cloud-0.4.9/kachery_cloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)      670 2024-05-13 18:36:48.000000 kachery_cloud-0.4.9/kachery_cloud.egg-info/entry_points.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       71 2024-05-13 18:36:48.000000 kachery_cloud-0.4.9/kachery_cloud.egg-info/requires.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       14 2024-05-13 18:36:48.000000 kachery_cloud-0.4.9/kachery_cloud.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)      490 2024-05-13 18:36:48.747841 kachery_cloud-0.4.9/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1189 2024-01-09 14:21:07.000000 kachery_cloud-0.4.9/setup.py
```

### Comparing `kachery_cloud-0.4.8/LICENSE` & `kachery_cloud-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/PKG-INFO` & `kachery_cloud-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kachery_cloud
-Version: 0.4.8
+Version: 0.4.9
 Summary: None
 Home-page: https://github.com/flatironinstitute/kachery-cloud
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Project-URL: Bug Tracker, https://github.com/flatironinstitute/kachery-cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `kachery_cloud-0.4.8/README.md` & `kachery_cloud-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/TemporaryDirectory.py` & `kachery_cloud-0.4.9/kachery_cloud/TemporaryDirectory.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/__init__.py` & `kachery_cloud-0.4.9/kachery_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/_client_keys.py` & `kachery_cloud-0.4.9/kachery_cloud/_client_keys.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/_custom_storage_backend.py` & `kachery_cloud-0.4.9/kachery_cloud/_custom_storage_backend.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/_fs_operations.py` & `kachery_cloud-0.4.9/kachery_cloud/_fs_operations.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/_get_kachery_gateway_url.py` & `kachery_cloud-0.4.9/kachery_cloud/_get_kachery_gateway_url.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/_get_local_client_config.py` & `kachery_cloud-0.4.9/kachery_cloud/_get_local_client_config.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/_json_stringify_deterministic.py` & `kachery_cloud-0.4.9/kachery_cloud/_json_stringify_deterministic.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/_kachery_gateway_request.py` & `kachery_cloud-0.4.9/kachery_cloud/_kachery_gateway_request.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/_load_github_file.py` & `kachery_cloud-0.4.9/kachery_cloud/_load_github_file.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/_safe_pickle.py` & `kachery_cloud-0.4.9/kachery_cloud/_safe_pickle.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/_serialize.py` & `kachery_cloud-0.4.9/kachery_cloud/_serialize.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/admin_delete_file.py` & `kachery_cloud-0.4.9/kachery_cloud/admin_delete_file.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/cli.py` & `kachery_cloud-0.4.9/kachery_cloud/cli.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/core.py` & `kachery_cloud-0.4.9/kachery_cloud/core.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/get_kachery_cloud_dir.py` & `kachery_cloud-0.4.9/kachery_cloud/get_kachery_cloud_dir.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/init.py` & `kachery_cloud-0.4.9/kachery_cloud/init.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,24 @@
     If the client is not registered, returns None.
 
     Returns
     -------
     response: dict
         The response dict from the Kachery Gateway
     """
+    # first check if we are using a custom storage backend
+    from ._custom_storage_backend import get_custom_storage_backend
+    sb = get_custom_storage_backend()
+    if sb is not None and hasattr(sb, 'store_file'):
+        return {
+            'type': 'getClientInfo',
+            'found': True,
+            'client': 'custom_storage_backend'
+        }
+
     if _global_init['client_info'] != 0:
         if _global_init['client_info']["client"]["clientId"] != get_client_id():
             logging.warning("Client ID in current `KACHERY_CLOUD_DIR`, does not match cached client info. \n"
                             + "If experiencing issues, please restart your python session and register the client again "
                             + f"with `KACHERY_CLOUD_DIR` set to {os.getenv('KACHERY_CLOUD_DIR')}")
         return _global_init['client_info']
     client_id = get_client_id()
```

### Comparing `kachery_cloud-0.4.8/kachery_cloud/link_file.py` & `kachery_cloud-0.4.9/kachery_cloud/link_file.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/load_bytes.py` & `kachery_cloud-0.4.9/kachery_cloud/load_bytes.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/load_file.py` & `kachery_cloud-0.4.9/kachery_cloud/load_file.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/mutable_local.py` & `kachery_cloud-0.4.9/kachery_cloud/mutable_local.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/request_file.py` & `kachery_cloud-0.4.9/kachery_cloud/request_file.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/store_file.py` & `kachery_cloud-0.4.9/kachery_cloud/store_file.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/store_file_local.py` & `kachery_cloud-0.4.9/kachery_cloud/store_file_local.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud/zenodo_upload/zenodo_upload.py` & `kachery_cloud-0.4.9/kachery_cloud/zenodo_upload/zenodo_upload.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud.egg-info/PKG-INFO` & `kachery_cloud-0.4.9/kachery_cloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kachery_cloud
-Version: 0.4.8
+Version: 0.4.9
 Summary: None
 Home-page: https://github.com/flatironinstitute/kachery-cloud
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Project-URL: Bug Tracker, https://github.com/flatironinstitute/kachery-cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `kachery_cloud-0.4.8/kachery_cloud.egg-info/SOURCES.txt` & `kachery_cloud-0.4.9/kachery_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/kachery_cloud.egg-info/entry_points.txt` & `kachery_cloud-0.4.9/kachery_cloud.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.8/setup.py` & `kachery_cloud-0.4.9/setup.py`

 * *Files identical despite different names*

