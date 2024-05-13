# Comparing `tmp/folkmq-1.4.3.tar.gz` & `tmp/folkmq-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folkmq-1.4.3.tar", last modified: Tue Apr 30 10:16:16 2024, max compression
+gzip compressed data, was "folkmq-1.4.4.tar", last modified: Mon May 13 00:12:56 2024, max compression
```

## Comparing `folkmq-1.4.3.tar` & `folkmq-1.4.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-30 10:16:15.998992 folkmq-1.4.3/
--rw-r--r--   0 noear      (501) staff       (20)      590 2024-04-30 10:16:15.998004 folkmq-1.4.3/PKG-INFO
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-30 10:16:15.969833 folkmq-1.4.3/folkmq/
--rw-r--r--   0 noear      (501) staff       (20)      504 2024-04-29 12:16:07.000000 folkmq-1.4.3/folkmq/FolkMQ.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:58:52.000000 folkmq-1.4.3/folkmq/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-30 10:16:15.983984 folkmq-1.4.3/folkmq/client/
--rw-r--r--   0 noear      (501) staff       (20)      163 2024-04-18 13:21:26.000000 folkmq-1.4.3/folkmq/client/MqAlarm.py
--rw-r--r--   0 noear      (501) staff       (20)     4015 2024-04-30 04:31:18.000000 folkmq-1.4.3/folkmq/client/MqClient.py
--rw-r--r--   0 noear      (501) staff       (20)    15358 2024-04-30 04:37:16.000000 folkmq-1.4.3/folkmq/client/MqClientDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     5518 2024-04-29 00:27:34.000000 folkmq-1.4.3/folkmq/client/MqClientListener.py
--rw-r--r--   0 noear      (501) staff       (20)     3807 2024-04-28 14:43:14.000000 folkmq-1.4.3/folkmq/client/MqMessage.py
--rw-r--r--   0 noear      (501) staff       (20)     3386 2024-04-28 14:55:57.000000 folkmq-1.4.3/folkmq/client/MqMessageReceived.py
--rw-r--r--   0 noear      (501) staff       (20)     1091 2024-04-23 13:26:37.000000 folkmq-1.4.3/folkmq/client/MqRouter.py
--rw-r--r--   0 noear      (501) staff       (20)      883 2024-04-23 13:35:12.000000 folkmq-1.4.3/folkmq/client/MqSubscription.py
--rw-r--r--   0 noear      (501) staff       (20)     1071 2024-04-28 14:37:03.000000 folkmq-1.4.3/folkmq/client/MqTransaction.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:59:09.000000 folkmq-1.4.3/folkmq/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-30 10:16:15.992262 folkmq-1.4.3/folkmq/common/
--rw-r--r--   0 noear      (501) staff       (20)      315 2024-04-18 12:44:59.000000 folkmq-1.4.3/folkmq/common/MqApis.py
--rw-r--r--   0 noear      (501) staff       (20)     1054 2024-04-28 12:22:21.000000 folkmq-1.4.3/folkmq/common/MqAssert.py
--rw-r--r--   0 noear      (501) staff       (20)     2372 2024-04-18 12:55:36.000000 folkmq-1.4.3/folkmq/common/MqConstants.py
--rw-r--r--   0 noear      (501) staff       (20)     2510 2024-04-28 14:52:59.000000 folkmq-1.4.3/folkmq/common/MqMetasResolver.py
--rw-r--r--   0 noear      (501) staff       (20)     4772 2024-04-28 14:52:31.000000 folkmq-1.4.3/folkmq/common/MqMetasResolverV1.py
--rw-r--r--   0 noear      (501) staff       (20)     4985 2024-04-28 14:52:42.000000 folkmq-1.4.3/folkmq/common/MqMetasResolverV2.py
--rw-r--r--   0 noear      (501) staff       (20)      773 2024-04-18 13:07:55.000000 folkmq-1.4.3/folkmq/common/MqMetasV1.py
--rw-r--r--   0 noear      (501) staff       (20)      999 2024-04-18 13:09:13.000000 folkmq-1.4.3/folkmq/common/MqMetasV2.py
--rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-28 14:12:52.000000 folkmq-1.4.3/folkmq/common/MqTopicHelper.py
--rw-r--r--   0 noear      (501) staff       (20)     1178 2024-04-28 14:41:42.000000 folkmq-1.4.3/folkmq/common/MqUtils.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:59:18.000000 folkmq-1.4.3/folkmq/common/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-30 10:16:15.994703 folkmq-1.4.3/folkmq/exception/
--rw-r--r--   0 noear      (501) staff       (20)      185 2024-04-18 10:00:43.000000 folkmq-1.4.3/folkmq/exception/FolkmqException.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:59:34.000000 folkmq-1.4.3/folkmq/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-30 10:16:15.995927 folkmq-1.4.3/folkmq.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      590 2024-04-30 10:16:15.000000 folkmq-1.4.3/folkmq.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)      896 2024-04-30 10:16:15.000000 folkmq-1.4.3/folkmq.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-30 10:16:15.000000 folkmq-1.4.3/folkmq.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       50 2024-04-30 10:16:15.000000 folkmq-1.4.3/folkmq.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)        7 2024-04-30 10:16:15.000000 folkmq-1.4.3/folkmq.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-30 10:16:15.000000 folkmq-1.4.3/folkmq.egg-info/zip-safe
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-30 10:16:15.999400 folkmq-1.4.3/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      913 2024-04-30 10:16:11.000000 folkmq-1.4.3/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.811900 folkmq-1.4.4/
+-rw-r--r--   0 noear      (501) staff       (20)      590 2024-05-13 00:12:56.811408 folkmq-1.4.4/PKG-INFO
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.801099 folkmq-1.4.4/folkmq/
+-rw-r--r--   0 noear      (501) staff       (20)      504 2024-05-12 15:23:34.000000 folkmq-1.4.4/folkmq/FolkMQ.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.805958 folkmq-1.4.4/folkmq/client/
+-rw-r--r--   0 noear      (501) staff       (20)      163 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqAlarm.py
+-rw-r--r--   0 noear      (501) staff       (20)     4015 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqClient.py
+-rw-r--r--   0 noear      (501) staff       (20)    15358 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqClientDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     5518 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqClientListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     3807 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqMessage.py
+-rw-r--r--   0 noear      (501) staff       (20)     3386 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqMessageReceived.py
+-rw-r--r--   0 noear      (501) staff       (20)     1091 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqRouter.py
+-rw-r--r--   0 noear      (501) staff       (20)      883 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqSubscription.py
+-rw-r--r--   0 noear      (501) staff       (20)     1071 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqTransaction.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.809294 folkmq-1.4.4/folkmq/common/
+-rw-r--r--   0 noear      (501) staff       (20)      315 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqApis.py
+-rw-r--r--   0 noear      (501) staff       (20)     1054 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqAssert.py
+-rw-r--r--   0 noear      (501) staff       (20)     2372 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqConstants.py
+-rw-r--r--   0 noear      (501) staff       (20)     2510 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqMetasResolver.py
+-rw-r--r--   0 noear      (501) staff       (20)     4772 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqMetasResolverV1.py
+-rw-r--r--   0 noear      (501) staff       (20)     4985 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqMetasResolverV2.py
+-rw-r--r--   0 noear      (501) staff       (20)      773 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqMetasV1.py
+-rw-r--r--   0 noear      (501) staff       (20)      999 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqMetasV2.py
+-rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqTopicHelper.py
+-rw-r--r--   0 noear      (501) staff       (20)     1178 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.810492 folkmq-1.4.4/folkmq/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      185 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/exception/FolkmqException.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.810854 folkmq-1.4.4/folkmq.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      590 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)      896 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       50 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)        7 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/zip-safe
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-05-13 00:12:56.812004 folkmq-1.4.4/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      913 2024-05-13 00:12:34.000000 folkmq-1.4.4/setup.py
```

### Comparing `folkmq-1.4.3/PKG-INFO` & `folkmq-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: folkmq
-Version: 1.4.3
+Version: 1.4.4
 Summary: @noear/folkmq python project
 Home-page: https://folkmq.noear.org/
 Author: noear
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: websockets>=12.0
-Requires-Dist: socket.d>=2.4.14.5
+Requires-Dist: socket.d>=2.4.16.1
```

### Comparing `folkmq-1.4.3/folkmq/client/MqClient.py` & `folkmq-1.4.4/folkmq/client/MqClient.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/client/MqClientDefault.py` & `folkmq-1.4.4/folkmq/client/MqClientDefault.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/client/MqClientListener.py` & `folkmq-1.4.4/folkmq/client/MqClientListener.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/client/MqMessage.py` & `folkmq-1.4.4/folkmq/client/MqMessage.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/client/MqMessageReceived.py` & `folkmq-1.4.4/folkmq/client/MqMessageReceived.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/client/MqRouter.py` & `folkmq-1.4.4/folkmq/client/MqRouter.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/client/MqSubscription.py` & `folkmq-1.4.4/folkmq/client/MqSubscription.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/client/MqTransaction.py` & `folkmq-1.4.4/folkmq/client/MqTransaction.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/common/MqAssert.py` & `folkmq-1.4.4/folkmq/common/MqAssert.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/common/MqConstants.py` & `folkmq-1.4.4/folkmq/common/MqConstants.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/common/MqMetasResolver.py` & `folkmq-1.4.4/folkmq/common/MqMetasResolver.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/common/MqMetasResolverV1.py` & `folkmq-1.4.4/folkmq/common/MqMetasResolverV1.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/common/MqMetasResolverV2.py` & `folkmq-1.4.4/folkmq/common/MqMetasResolverV2.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/common/MqMetasV1.py` & `folkmq-1.4.4/folkmq/common/MqMetasV1.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/common/MqMetasV2.py` & `folkmq-1.4.4/folkmq/common/MqMetasV2.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq/common/MqUtils.py` & `folkmq-1.4.4/folkmq/common/MqUtils.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/folkmq.egg-info/PKG-INFO` & `folkmq-1.4.4/folkmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: folkmq
-Version: 1.4.3
+Version: 1.4.4
 Summary: @noear/folkmq python project
 Home-page: https://folkmq.noear.org/
 Author: noear
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: websockets>=12.0
-Requires-Dist: socket.d>=2.4.14.5
+Requires-Dist: socket.d>=2.4.16.1
```

### Comparing `folkmq-1.4.3/folkmq.egg-info/SOURCES.txt` & `folkmq-1.4.4/folkmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.3/setup.py` & `folkmq-1.4.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*_
 from setuptools import setup,find_packages
 
 setup(
     name='folkmq',
-    version='1.4.3',
+    version='1.4.4',
     description='@noear/folkmq python project',
     author='noear',
     url='https://folkmq.noear.org/',
     packages=find_packages(exclude=['*folkmq-test*']),   # 包内不需要引用的文件夹
     install_requires=[                          # 依赖包
         'loguru>=0.7.2',
         'websockets>=12.0',
-        'socket.d>=2.4.14.5'
+        'socket.d>=2.4.16.1'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

