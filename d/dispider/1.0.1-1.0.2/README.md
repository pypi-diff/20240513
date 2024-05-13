# Comparing `tmp/dispider-1.0.1.tar.gz` & `tmp/dispider-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispider-1.0.1.tar", last modified: Thu Apr 25 16:14:36 2024, max compression
+gzip compressed data, was "dispider-1.0.2.tar", last modified: Mon May 13 03:33:47 2024, max compression
```

## Comparing `dispider-1.0.1.tar` & `dispider-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 16:14:36.260416 dispider-1.0.1/
--rw-rw-rw-   0        0        0      615 2024-04-25 16:14:36.259404 dispider-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       15 2024-04-25 13:46:01.000000 dispider-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 16:14:36.255012 dispider-1.0.1/dispider/
--rw-rw-rw-   0        0        0     3852 2024-04-25 16:13:52.000000 dispider-1.0.1/dispider/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 16:14:36.259404 dispider-1.0.1/dispider.egg-info/
--rw-rw-rw-   0        0        0      615 2024-04-25 16:14:36.000000 dispider-1.0.1/dispider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-04-25 16:14:36.000000 dispider-1.0.1/dispider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 16:14:36.000000 dispider-1.0.1/dispider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-25 16:14:36.000000 dispider-1.0.1/dispider.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 16:14:36.000000 dispider-1.0.1/dispider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 16:14:36.260416 dispider-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1110 2024-04-25 16:14:32.000000 dispider-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:33:47.710502 dispider-1.0.2/
+-rw-rw-rw-   0        0        0      615 2024-05-13 03:33:47.710502 dispider-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2024-04-25 13:46:01.000000 dispider-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 03:33:47.707503 dispider-1.0.2/dispider/
+-rw-rw-rw-   0        0        0     3862 2024-05-13 03:33:44.000000 dispider-1.0.2/dispider/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:33:47.710502 dispider-1.0.2/dispider.egg-info/
+-rw-rw-rw-   0        0        0      615 2024-05-13 03:33:47.000000 dispider-1.0.2/dispider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-13 03:33:47.000000 dispider-1.0.2/dispider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 03:33:47.000000 dispider-1.0.2/dispider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-13 03:33:47.000000 dispider-1.0.2/dispider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 03:33:47.000000 dispider-1.0.2/dispider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 03:33:47.711502 dispider-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2024-05-13 03:33:33.000000 dispider-1.0.2/setup.py
```

### Comparing `dispider-1.0.1/PKG-INFO` & `dispider-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispider
-Version: 1.0.1
+Version: 1.0.2
 Summary: A toolkit to help beginners quickly deploy crawlers in batches and manage tasks.
 Author: data.dilattice.top
 Author-email: 
 Keywords: python,spider,dispider,windows,mac,linux
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dispider-1.0.1/dispider/__init__.py` & `dispider-1.0.2/dispider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import requests
 import pandas as pd
 
 
 # 定义项目工具类
 class Dispider:
     # 初始化
-    def __init__(self, worker, project=str):
+    def __init__(self, worker, project=str, host='10.240.61.63'):
         # 设置请求主站地址
-        self.host = 'http://data.dilattice.top:8000/'
+        self.host = f'http://{host}:8000/'
         # 检测项目名的存在性
         name_permission = requests.post(url=self.host + 'project/check/', data={'project': project.lower()}).json()[
             '反馈']
         # 初始化项目名或抛出报错
         if name_permission:
             self.project_name = project
             print(f'欢迎进入{project}项目')
```

### Comparing `dispider-1.0.1/dispider.egg-info/PKG-INFO` & `dispider-1.0.2/dispider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispider
-Version: 1.0.1
+Version: 1.0.2
 Summary: A toolkit to help beginners quickly deploy crawlers in batches and manage tasks.
 Author: data.dilattice.top
 Author-email: 
 Keywords: python,spider,dispider,windows,mac,linux
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dispider-1.0.1/setup.py` & `dispider-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # these things are needed for the README.md show on pypi
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = "A toolkit to help beginners quickly deploy crawlers in batches and manage tasks."
 
 # Setting up
 setup(
     name="dispider",
     version=VERSION,
     author="data.dilattice.top",
```

