# Comparing `tmp/alibabacloud_antiddos-public20170518-1.0.2.tar.gz` & `tmp/alibabacloud_antiddos-public20170518-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_antiddos-public20170518-1.0.2.tar", last modified: Tue Jul 12 10:01:51 2022, max compression
+gzip compressed data, was "dist/alibabacloud_antiddos-public20170518-1.0.3.tar", last modified: Mon May 13 03:49:51 2024, max compression
```

## Comparing `alibabacloud_antiddos-public20170518-1.0.2.tar` & `alibabacloud_antiddos-public20170518-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2400 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1058 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518/
--rw-r--r--   0 root         (0) root         (0)       21 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45433 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518/client.py
--rw-r--r--   0 root         (0) root         (0)    78609 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2400 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2672 2022-07-12 10:01:51.000000 alibabacloud_antiddos-public20170518-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:49:51.000000 alibabacloud_antiddos-public20170518-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      154 2024-05-13 03:49:50.000000 alibabacloud_antiddos-public20170518-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-13 03:49:50.000000 alibabacloud_antiddos-public20170518-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-13 03:49:50.000000 alibabacloud_antiddos-public20170518-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-05-13 03:49:51.000000 alibabacloud_antiddos-public20170518-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-13 03:49:50.000000 alibabacloud_antiddos-public20170518-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1228 2024-05-13 03:49:50.000000 alibabacloud_antiddos-public20170518-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:49:51.000000 alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-13 03:49:50.000000 alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101506 2024-05-13 03:49:50.000000 alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518/client.py
+-rw-r--r--   0 root         (0) root         (0)   101193 2024-05-13 03:49:50.000000 alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:49:51.000000 alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-05-13 03:49:51.000000 alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2024-05-13 03:49:51.000000 alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 03:49:51.000000 alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-13 03:49:51.000000 alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-05-13 03:49:51.000000 alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-13 03:49:51.000000 alibabacloud_antiddos-public20170518-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-05-13 03:49:50.000000 alibabacloud_antiddos-public20170518-1.0.3/setup.py
```

### Comparing `alibabacloud_antiddos-public20170518-1.0.2/LICENSE` & `alibabacloud_antiddos-public20170518-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_antiddos-public20170518-1.0.2/PKG-INFO` & `alibabacloud_antiddos-public20170518-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_antiddos-public20170518
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud antiddos-public (20170518) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/antiddos-public-20170518/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_antiddos-public20170518-1.0.2/README-CN.md` & `alibabacloud_antiddos-public20170518-1.0.3/README-CN.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/antiddos-public-20170518/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_antiddos-public20170518-1.0.2/README.md` & `alibabacloud_antiddos-public20170518-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/antiddos-public-20170518/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518.egg-info/PKG-INFO` & `alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-antiddos-public20170518
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud antiddos-public (20170518) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/antiddos-public-20170518/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_antiddos-public20170518-1.0.2/alibabacloud_antiddos_public20170518.egg-info/SOURCES.txt` & `alibabacloud_antiddos-public20170518-1.0.3/alibabacloud_antiddos_public20170518.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_antiddos-public20170518-1.0.2/setup.py` & `alibabacloud_antiddos-public20170518-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_antiddos-public20170518.
 
-Created on 12/07/2022
+Created on 13/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_antiddos_public20170518"
 NAME = "alibabacloud_antiddos-public20170518" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud antiddos-public (20170518) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

