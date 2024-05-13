# Comparing `tmp/co6co-0.0.3.231001.tar.gz` & `tmp/co6co-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "co6co-0.0.3.231001.tar", last modified: Thu Oct 19 02:27:32 2023, max compression
+gzip compressed data, was "co6co-0.0.4.tar", last modified: Sat May 11 06:44:42 2024, max compression
```

## Comparing `co6co-0.0.3.231001.tar` & `co6co-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-10-19 02:27:32.254814 co6co-0.0.3.231001/
--rw-rw-rw-   0        0        0       13 2023-08-16 08:48:34.000000 co6co-0.0.3.231001/MANIFEST.in
--rw-rw-rw-   0        0        0      440 2023-10-19 02:27:32.251813 co6co-0.0.3.231001/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-08-18 01:57:56.000000 co6co-0.0.3.231001/README.md
-drwxrwxrwx   0        0        0        0 2023-10-19 02:27:32.209826 co6co-0.0.3.231001/co6co/
--rw-rw-rw-   0        0        0      432 2023-10-19 02:26:48.000000 co6co-0.0.3.231001/co6co/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-19 02:27:32.250813 co6co-0.0.3.231001/co6co/utils/
--rw-rw-rw-   0        0        0     1059 2023-09-04 08:02:30.000000 co6co-0.0.3.231001/co6co/utils/File.py
--rw-rw-rw-   0        0        0      362 2023-10-13 02:58:49.000000 co6co-0.0.3.231001/co6co/utils/__init__.py
--rw-rw-rw-   0        0        0      174 2023-10-16 05:08:36.000000 co6co-0.0.3.231001/co6co/utils/hash.py
--rw-rw-rw-   0        0        0     2400 2023-09-14 01:40:45.000000 co6co-0.0.3.231001/co6co/utils/http.py
--rw-rw-rw-   0        0        0      531 2023-10-13 01:30:19.000000 co6co-0.0.3.231001/co6co/utils/json_util.py
--rw-rw-rw-   0        0        0     2931 2023-09-07 02:12:59.000000 co6co-0.0.3.231001/co6co/utils/log.py
--rw-rw-rw-   0        0        0        0 2023-10-13 01:38:34.000000 co6co-0.0.3.231001/co6co/utils/tool_util.py
-drwxrwxrwx   0        0        0        0 2023-10-19 02:27:32.232819 co6co-0.0.3.231001/co6co.egg-info/
--rw-rw-rw-   0        0        0      440 2023-10-19 02:27:32.000000 co6co-0.0.3.231001/co6co.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-10-19 02:27:32.000000 co6co-0.0.3.231001/co6co.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-19 02:27:32.000000 co6co-0.0.3.231001/co6co.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-10-19 02:27:32.000000 co6co-0.0.3.231001/co6co.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-08-16 08:23:34.000000 co6co-0.0.3.231001/co6co.egg-info/zip-safe
--rw-rw-rw-   0        0        0       30 2023-08-17 03:39:37.000000 co6co-0.0.3.231001/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-10-19 02:27:32.255814 co6co-0.0.3.231001/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-09-04 06:05:12.000000 co6co-0.0.3.231001/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.211477 co6co-0.0.4/
+-rw-rw-rw-   0        0        0       13 2023-08-16 08:48:34.000000 co6co-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      433 2024-05-11 06:44:42.210478 co6co-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-08-18 01:57:56.000000 co6co-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.175032 co6co-0.0.4/co6co/
+-rw-rw-rw-   0        0        0     1070 2024-05-11 06:44:40.000000 co6co-0.0.4/co6co/__init__.py
+-rw-rw-rw-   0        0        0      281 2024-01-05 09:13:48.000000 co6co-0.0.4/co6co/demo.test.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.192696 co6co-0.0.4/co6co/enums/
+-rw-rw-rw-   0        0        0     2253 2024-04-10 08:24:13.000000 co6co-0.0.4/co6co/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.194693 co6co-0.0.4/co6co/task/
+-rw-rw-rw-   0        0        0        0 2024-01-19 08:21:45.000000 co6co-0.0.4/co6co/task/__init__.py
+-rw-rw-rw-   0        0        0     2219 2024-03-14 02:19:00.000000 co6co-0.0.4/co6co/task/thread.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.204550 co6co-0.0.4/co6co/utils/
+-rw-rw-rw-   0        0        0     2674 2024-03-29 09:20:58.000000 co6co-0.0.4/co6co/utils/File.py
+-rw-rw-rw-   0        0        0      920 2024-03-18 01:38:20.000000 co6co-0.0.4/co6co/utils/__init__.py
+-rw-rw-rw-   0        0        0     6035 2023-12-18 01:29:31.000000 co6co-0.0.4/co6co/utils/hash.py
+-rw-rw-rw-   0        0        0     2400 2023-09-14 01:40:45.000000 co6co-0.0.4/co6co/utils/http.py
+-rw-rw-rw-   0        0        0      512 2023-12-18 01:29:31.000000 co6co-0.0.4/co6co/utils/json_util.py
+-rw-rw-rw-   0        0        0     3478 2024-04-29 08:11:33.000000 co6co-0.0.4/co6co/utils/log.py
+-rw-rw-rw-   0        0        0     1393 2024-05-07 09:41:22.000000 co6co-0.0.4/co6co/utils/tool_util.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.189349 co6co-0.0.4/co6co.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-11 06:44:42.000000 co6co-0.0.4/co6co.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2024-05-11 06:44:42.000000 co6co-0.0.4/co6co.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 06:44:42.000000 co6co-0.0.4/co6co.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-11 06:44:42.000000 co6co-0.0.4/co6co.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-16 08:23:34.000000 co6co-0.0.4/co6co.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       30 2023-08-17 03:39:37.000000 co6co-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0      684 2024-04-22 05:42:25.000000 co6co-0.0.4/service.encode.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 06:44:42.211477 co6co-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1116 2024-02-27 01:32:43.000000 co6co-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:44:42.209479 co6co-0.0.4/tests/
+-rw-rw-rw-   0        0        0      356 2024-02-27 01:32:43.000000 co6co-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      255 2024-02-27 01:32:43.000000 co6co-0.0.4/tests/unittest.md
+-rw-rw-rw-   0        0        0     1934 2024-02-27 01:32:43.000000 co6co-0.0.4/tests/v_utils_test.py
```

### Comparing `co6co-0.0.3.231001/co6co/utils/http.py` & `co6co-0.0.4/co6co/utils/http.py`

 * *Files identical despite different names*

### Comparing `co6co-0.0.3.231001/co6co/utils/json_util.py` & `co6co-0.0.4/co6co/utils/json_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding:utf-8 -*-
 
 
 import json,datetime
 from typing import Any
 
 class JSON_util(json.JSONEncoder):
-    def default(self, obj: Any) -> Any: 
-        print(obj)
+    def default(self, obj: Any) -> Any:  
         if isinstance(obj, datetime.datetime):  return obj.strftime("%Y-%m-%d %H:%M:%S")
         elif isinstance(obj, bytes): return str(obj, encoding='utf-8')
         elif isinstance(obj, int): return int(obj)
         elif isinstance(obj, float):return float(obj) 
         elif hasattr(obj,"__dict__"):  return obj.__dict__ 
         return None
```

### Comparing `co6co-0.0.3.231001/setup.py` & `co6co-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 currentDir = path.abspath(path.dirname(__file__))
 with open(path.join(currentDir, 'README.md'), encoding='utf-8') as f: long_description = f.read()
 
 
 setup(
     name="co6co",
     version=VERSION,
-    description="基础模块",
-    packages=find_packages(),
+    description="基础模块", 
+    packages=find_packages( ),  
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[ "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.6" ],
     include_package_data=True, zip_safe=True,
     #依赖哪些模块
     install_requires=[ ],
     #package_dir= {'utils':'src/log','main_package':'main'},#告诉Distutils哪些目录下的文件被映射到哪个源码
```

