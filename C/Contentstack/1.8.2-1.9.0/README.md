# Comparing `tmp/Contentstack-1.8.2.tar.gz` & `tmp/contentstack-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Contentstack-1.8.2.tar", last modified: Wed Dec  6 07:04:17 2023, max compression
+gzip compressed data, was "contentstack-1.9.0.tar", last modified: Mon May 13 11:57:39 2024, max compression
```

## Comparing `Contentstack-1.8.2.tar` & `contentstack-1.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 07:04:17.434173 Contentstack-1.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 07:04:17.434173 Contentstack-1.8.2/Contentstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9092 2023-12-06 07:04:17.000000 Contentstack-1.8.2/Contentstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      719 2023-12-06 07:04:17.000000 Contentstack-1.8.2/Contentstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 07:04:17.000000 Contentstack-1.8.2/Contentstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 07:04:17.000000 Contentstack-1.8.2/Contentstack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 07:04:17.000000 Contentstack-1.8.2/Contentstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-06 07:04:17.000000 Contentstack-1.8.2/Contentstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-06 07:04:08.000000 Contentstack-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9092 2023-12-06 07:04:17.434173 Contentstack-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2023-12-06 07:04:08.000000 Contentstack-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 07:04:17.434173 Contentstack-1.8.2/contentstack/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/assetquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/basequery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/contenttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/deep_merge_lp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/entryqueryable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    14757 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    15324 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-12-06 07:04:08.000000 Contentstack-1.8.2/contentstack/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 07:04:17.434173 Contentstack-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2023-12-06 07:04:08.000000 Contentstack-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 07:04:17.434173 Contentstack-1.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2023-12-06 07:04:08.000000 Contentstack-1.8.2/tests/test_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2023-12-06 07:04:08.000000 Contentstack-1.8.2/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2023-12-06 07:04:08.000000 Contentstack-1.8.2/tests/test_live_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2023-12-06 07:04:08.000000 Contentstack-1.8.2/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7708 2023-12-06 07:04:08.000000 Contentstack-1.8.2/tests/test_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:57:39.429557 contentstack-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:57:39.429557 contentstack-1.9.0/Contentstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9092 2024-05-13 11:57:39.000000 contentstack-1.9.0/Contentstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-13 11:57:39.000000 contentstack-1.9.0/Contentstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:57:39.000000 contentstack-1.9.0/Contentstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:57:39.000000 contentstack-1.9.0/Contentstack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:57:39.000000 contentstack-1.9.0/Contentstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 11:57:39.000000 contentstack-1.9.0/Contentstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-13 11:57:31.000000 contentstack-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9092 2024-05-13 11:57:39.429557 contentstack-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-13 11:57:31.000000 contentstack-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:57:39.425557 contentstack-1.9.0/contentstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/assetquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/basequery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/contenttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/deep_merge_lp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/entryqueryable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15474 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-13 11:57:31.000000 contentstack-1.9.0/contentstack/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:57:39.429557 contentstack-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-13 11:57:31.000000 contentstack-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:57:39.429557 contentstack-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-05-13 11:57:31.000000 contentstack-1.9.0/tests/test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-13 11:57:31.000000 contentstack-1.9.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-13 11:57:31.000000 contentstack-1.9.0/tests/test_live_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-05-13 11:57:31.000000 contentstack-1.9.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-13 11:57:31.000000 contentstack-1.9.0/tests/test_stack.py
```

### Comparing `Contentstack-1.8.2/Contentstack.egg-info/PKG-INFO` & `contentstack-1.9.0/Contentstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Contentstack
-Version: 1.8.2
+Version: 1.9.0
 Summary: Contentstack is a headless CMS with an API-first approach.
 Home-page: https://github.com/contentstack/contentstack-python
 Author: Contentstack
 Author-email: shailesh.mishra@contentstack.com, sunil.lakshman@contentstack.com
 License: MIT
 Keywords: contentstack-python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Contentstack-1.8.2/Contentstack.egg-info/SOURCES.txt` & `contentstack-1.9.0/Contentstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/LICENSE` & `contentstack-1.9.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2012 - 2023 Contentstack. All rights reserved.
+Copyright (c) 2012 - 2024 Contentstack. All rights reserved.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `Contentstack-1.8.2/PKG-INFO` & `contentstack-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Contentstack
-Version: 1.8.2
+Version: 1.9.0
 Summary: Contentstack is a headless CMS with an API-first approach.
 Home-page: https://github.com/contentstack/contentstack-python
 Author: Contentstack
 Author-email: shailesh.mishra@contentstack.com, sunil.lakshman@contentstack.com
 License: MIT
 Keywords: contentstack-python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Contentstack-1.8.2/README.md` & `contentstack-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/__init__.py` & `contentstack-1.9.0/contentstack/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 "Stack",
 "Utils"
 )
 
 __title__ = 'contentstack-delivery-python'
 __author__ = 'contentstack'
 __status__ = 'debug'
-__version__ = 'v1.8.2'
+__version__ = 'v1.9.0'
 __endpoint__ = 'cdn.contentstack.io'
 __email__ = 'mobile@contentstack.com'
 __developer_email__ = 'shailesh.mishra@contentstack.com'
 __license__ = "MIT"
```

### Comparing `Contentstack-1.8.2/contentstack/asset.py` & `contentstack-1.9.0/contentstack/asset.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/assetquery.py` & `contentstack-1.9.0/contentstack/assetquery.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/basequery.py` & `contentstack-1.9.0/contentstack/basequery.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/contenttype.py` & `contentstack-1.9.0/contentstack/contenttype.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/controller.py` & `contentstack-1.9.0/contentstack/controller.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/deep_merge_lp.py` & `contentstack-1.9.0/contentstack/deep_merge_lp.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/entry.py` & `contentstack-1.9.0/contentstack/entry.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/entryqueryable.py` & `contentstack-1.9.0/contentstack/entryqueryable.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/https_connection.py` & `contentstack-1.9.0/contentstack/https_connection.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/image_transform.py` & `contentstack-1.9.0/contentstack/image_transform.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/query.py` & `contentstack-1.9.0/contentstack/query.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/contentstack/stack.py` & `contentstack-1.9.0/contentstack/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     """
     Sets region for the contentstack
     """
     US = 'us'
     EU = 'eu'
     AZURE_NA = 'azure-na'
     AZURE_EU = 'azure-eu'
+    GCP_NA = 'gcp-na'
 
 
 class Stack:
     """
     A stack can be defined as a pool of data or a container that holds all
     the content/assets related to a site. It is a collaboration space where multiple users can work
     together to create, edit, approve, and publish content.
@@ -112,14 +113,16 @@
 
         if self.region.value == 'eu' and self.host == DEFAULT_HOST:
             self.host = 'eu-cdn.contentstack.com'
         elif self.region.value == 'azure-na' and self.host == DEFAULT_HOST:
             self.host = 'azure-na-cdn.contentstack.com'
         elif self.region.value == 'azure-eu' and self.host == DEFAULT_HOST:
             self.host = 'azure-eu-cdn.contentstack.com'
+        elif self.region.value == 'gcp-na' and self.host == DEFAULT_HOST:
+            self.host = 'gcp-na-cdn.contentstack.com'
         elif self.region.value != 'us':
             self.host = f'{self.region.value}-{DEFAULT_HOST}'
         self.endpoint = f'https://{self.host}/{self.version}'
 
         self.headers = {
             'api_key': self.api_key,
             'access_token': self.delivery_token,
```

### Comparing `Contentstack-1.8.2/contentstack/utility.py` & `contentstack-1.9.0/contentstack/utility.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/setup.py` & `contentstack-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/tests/test_assets.py` & `contentstack-1.9.0/tests/test_assets.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/tests/test_entry.py` & `contentstack-1.9.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/tests/test_live_preview.py` & `contentstack-1.9.0/tests/test_live_preview.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/tests/test_query.py` & `contentstack-1.9.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `Contentstack-1.8.2/tests/test_stack.py` & `contentstack-1.9.0/tests/test_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,19 @@
         self.assertEqual(HOST, stack_instance.host)
 
     def test_02_stack_region(self):
         stack_region = contentstack.Stack(
             API_KEY, DELIVERY_TOKEN, ENVIRONMENT, region=ContentstackRegion.EU)
         self.assertEqual('eu-cdn.contentstack.com', stack_region.host)
 
+    def test_02_stack_gcp_na_region(self):
+        stack_region = contentstack.Stack(
+            API_KEY, DELIVERY_TOKEN, ENVIRONMENT, region=ContentstackRegion.GCP_NA)
+        self.assertEqual('gcp-na-cdn.contentstack.com', stack_region.host)
+
     def test_03_stack_endpoint(self):
         self.assertEqual(f"https://{config.HOST}/v3",
                          self.stack.endpoint)
 
     def test_04_permission_error_api_key(self):
         try:
             stack_local = contentstack.Stack(
```

