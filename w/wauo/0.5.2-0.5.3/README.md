# Comparing `tmp/wauo-0.5.2.tar.gz` & `tmp/wauo-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wauo-0.5.2.tar", last modified: Wed May  8 16:43:30 2024, max compression
+gzip compressed data, was "wauo-0.5.3.tar", last modified: Mon May 13 14:44:02 2024, max compression
```

## Comparing `wauo-0.5.2.tar` & `wauo-0.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 16:43:30.046211 wauo-0.5.2/
--rw-r--r--   0 wangtuo    (501) staff       (20)     1594 2024-05-08 16:43:30.046002 wauo-0.5.2/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)     1335 2024-04-28 13:29:40.000000 wauo-0.5.2/README.md
--rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-08 16:43:30.046245 wauo-0.5.2/setup.cfg
--rw-r--r--   0 wangtuo    (501) staff       (20)      615 2024-05-08 16:43:26.000000 wauo-0.5.2/setup.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 16:43:30.045025 wauo-0.5.2/wauo/
--rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.5.2/wauo/__init__.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.5.2/wauo/exceptions.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.5.2/wauo/response.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     5228 2024-05-08 14:14:02.000000 wauo-0.5.2/wauo/spiders.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-03 14:44:50.000000 wauo-0.5.2/wauo/test.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 16:43:30.045842 wauo-0.5.2/wauo.egg-info/
--rw-r--r--   0 wangtuo    (501) staff       (20)     1594 2024-05-08 16:43:30.000000 wauo-0.5.2/wauo.egg-info/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)      266 2024-05-08 16:43:30.000000 wauo-0.5.2/wauo.egg-info/SOURCES.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-08 16:43:30.000000 wauo-0.5.2/wauo.egg-info/dependency_links.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-08 16:43:30.000000 wauo-0.5.2/wauo.egg-info/not-zip-safe
--rw-r--r--   0 wangtuo    (501) staff       (20)       31 2024-05-08 16:43:30.000000 wauo-0.5.2/wauo.egg-info/requires.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-08 16:43:30.000000 wauo-0.5.2/wauo.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-13 14:44:02.198037 wauo-0.5.3/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1730 2024-05-13 14:44:02.197804 wauo-0.5.3/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1471 2024-05-13 14:43:30.000000 wauo-0.5.3/README.md
+-rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-13 14:44:02.198085 wauo-0.5.3/setup.cfg
+-rw-r--r--   0 wangtuo    (501) staff       (20)      615 2024-05-13 14:43:30.000000 wauo-0.5.3/setup.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-13 14:44:02.196785 wauo-0.5.3/wauo/
+-rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.5.3/wauo/__init__.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.5.3/wauo/exceptions.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.5.3/wauo/response.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     5506 2024-05-13 14:43:30.000000 wauo-0.5.3/wauo/spiders.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-13 14:31:08.000000 wauo-0.5.3/wauo/test.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-13 14:44:02.197602 wauo-0.5.3/wauo.egg-info/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1730 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)      266 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/not-zip-safe
+-rw-r--r--   0 wangtuo    (501) staff       (20)       31 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/requires.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/top_level.txt
```

### Comparing `wauo-0.5.2/PKG-INFO` & `wauo-0.5.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-Metadata-Version: 2.1
-Name: wauo
-Version: 0.5.2
-Summary: 爬虫者的贴心助手
-Home-page: https://github.com/markadc/wauo
-Author: WangTuo
-Author-email: markadc@126.com
-License: MIT
-Keywords: python,requests,spider
-Description-Content-Type: text/markdown
+# 更新历史
+
+- 新增`jsonp2json`静态方法
+- 爬虫`默认保持会话`状态
+- 新增`get_uuid`、`base64加解密`静态方法
 
 # 项目说明
 
 - 基于requests封装的一个爬虫类
 
 # Python解释器
 
@@ -89,8 +84,8 @@
 
 - 每一次请求的headers都带上cookie
 
 ```python
 spider = WauoSpider(default_headers={'Cookie': 'Your Cookies'})
 resp = spider.send('https://github.com/markadc')
 print(resp.request.headers)
-```
+```
```

### Comparing `wauo-0.5.2/setup.py` & `wauo-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='wauo',
-    version='0.5.2',
+    version='0.5.3',
     description='爬虫者的贴心助手',
     url='https://github.com/markadc/wauo',
     author='WangTuo',
     author_email='markadc@126.com',
     packages=find_packages(),
     license='MIT',
     zip_safe=False,
```

### Comparing `wauo-0.5.2/wauo/response.py` & `wauo-0.5.3/wauo/response.py`

 * *Files identical despite different names*

### Comparing `wauo-0.5.2/wauo/spiders.py` & `wauo-0.5.3/wauo/spiders.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import base64
 import hashlib
+import json
 import os
 import random
+import re
 import string
 import time
 import uuid
 from datetime import datetime
 from typing import Callable
 
 import requests
@@ -18,14 +20,20 @@
 from wauo.response import Response
 
 
 class SpiderTools:
     """爬虫工具"""
 
     @staticmethod
+    def jsonp2json(jsonp):
+        """jsonp转换为json"""
+        data: dict = json.loads(re.match(".*?({.*}).*", jsonp, re.S).group(1))
+        return data
+
+    @staticmethod
     def get_uuid():
         """获取uuid"""
         uuid4 = str(uuid.uuid4())
         return uuid4
 
     @staticmethod
     def b64_encode(s: str):
@@ -108,30 +116,34 @@
                 )
         logger.error('Failed  ==>  {}'.format(url))
 
     return _retry
 
 
 class BaseSpider(SpiderTools):
+    """爬虫基类"""
+
     ua = UserAgent()
 
     def get_headers(self) -> dict:
         """获取headers"""
         headers = {'User-Agent': self.ua.random}
         return headers
 
     @staticmethod
     def get_proxies() -> dict:
         """获取代理"""
         return {}
 
 
 class WauoSpider(BaseSpider):
+    """该爬虫默认保持会话状态"""
+
     def __init__(self, session=True, default_headers: dict = None):
-        self.req = requests.Session() if session else requests
+        self.client = requests.Session() if session else requests
         self.default_headers = default_headers or {}
 
     @retry
     def send(
             self, url: str, headers: dict = None, proxies: dict = None, timeout=3,
             data: dict = None, json: dict = None,
             cookie: str = None, codes: list = None, checker: Callable = None,
@@ -146,17 +158,17 @@
         if cookie:
             headers.setdefault('Cookie', cookie)
         for key, value in self.default_headers.items():
             headers.setdefault(key, value)
 
         same = dict(headers=headers, proxies=proxies, timeout=timeout)
         if data is None and json is None:
-            response = self.req.get(url, **same, **kwargs)
+            response = self.client.get(url, **same, **kwargs)
         else:
-            response = self.req.post(url, data=data, json=json, **same, **kwargs)
+            response = self.client.post(url, data=data, json=json, **same, **kwargs)
 
         if codes and response.status_code not in codes:
             raise ResponseCodeError('{} not in {}'.format(response.status_code, codes))
         if checker and checker(response) is False:
             raise ResponseTextError('not ideal text')
 
         return Response(response)
```

### Comparing `wauo-0.5.2/wauo.egg-info/PKG-INFO` & `wauo-0.5.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: wauo
-Version: 0.5.2
+Version: 0.5.3
 Summary: 爬虫者的贴心助手
 Home-page: https://github.com/markadc/wauo
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: python,requests,spider
 Description-Content-Type: text/markdown
 
+# 更新历史
+
+- 新增`jsonp2json`静态方法
+- 爬虫`默认保持会话`状态
+- 新增`get_uuid`、`base64加解密`静态方法
+
 # 项目说明
 
 - 基于requests封装的一个爬虫类
 
 # Python解释器
 
 - python3
```

