# Comparing `tmp/tsugu-api-python-1.0.0.tar.gz` & `tmp/tsugu-api-python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-1.0.0.tar", last modified: Mon May 13 01:41:07 2024, max compression
+gzip compressed data, was "tsugu-api-python-1.0.1.tar", last modified: Mon May 13 02:52:41 2024, max compression
```

## Comparing `tsugu-api-python-1.0.0.tar` & `tsugu-api-python-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-13 01:41:07.000000 tsugu-api-python-1.0.0/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-13 01:41:07.000000 tsugu-api-python-1.0.0/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 01:41:07.000000 tsugu-api-python-1.0.0/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 01:41:07.000000 tsugu-api-python-1.0.0/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:52:41.182197 tsugu-api-python-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-13 02:52:41.182197 tsugu-api-python-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 02:52:41.182197 tsugu-api-python-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:52:41.178197 tsugu-api-python-1.0.1/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:52:41.178197 tsugu-api-python-1.0.1/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-13 02:52:29.000000 tsugu-api-python-1.0.1/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:52:41.178197 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-13 02:52:40.000000 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-13 02:52:41.000000 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 02:52:40.000000 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 02:52:40.000000 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 02:52:40.000000 tsugu-api-python-1.0.1/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-1.0.0/LICENSE` & `tsugu-api-python-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/PKG-INFO` & `tsugu-api-python-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
         
@@ -30,14 +30,18 @@
           <img src="https://img.shields.io/github/license/WindowsSov8forUs/tsugu-api-python" alt="License">
         </a>
         
         <a href="https://www.python.org/downloads/">
           <img src="https://img.shields.io/pypi/pyversions/tsugu-api-python" alt="Python Version">
         </a>
         
+        <a href="https://pypi.org/project/tsugu-api-python/">
+          <img src="https://img.shields.io/pypi/v/tsugu-api-python" alt="PyPI Version">
+        </a>
+        
         </p>
         
         ## 说明
         
         这是一个用 Python 编写的调用 [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file) 相关各种功能 API 的库，包括绝大部分 Tsugu 提供的功能。使用本 API 库提供的方法可以实现绝大部分功能，而搭配 [bestdori-api](https://github.com/WindowsSov8forUs/bestdori-api) 可以实现用户绑定等其他功能。
         
         > 该 API 库同时提供了异步与同步版本，可自行选择使用。
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.0 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.1 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
-          _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
+   _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _V_e_r_s_i_o_n_]
 ## è¯´æ è¿æ¯ä¸ä¸ªç¨ Python ç¼åçè°ç¨ [TsuguBanGDreamBot](https://
 github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file)
 ç¸å³åç§åè½ API çåºï¼åæ¬ç»å¤§é¨å Tsugu
 æä¾çåè½ãä½¿ç¨æ¬ API
 åºæä¾çæ¹æ³å¯ä»¥å®ç°ç»å¤§é¨ååè½ï¼èæ­é [bestdori-api]
 (https://github.com/WindowsSov8forUs/bestdori-api)
 å¯ä»¥å®ç°ç¨æ·ç»å®ç­å¶ä»åè½ã > è¯¥ API
```

### Comparing `tsugu-api-python-1.0.0/README.md` & `tsugu-api-python-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,18 @@
   <img src="https://img.shields.io/github/license/WindowsSov8forUs/tsugu-api-python" alt="License">
 </a>
 
 <a href="https://www.python.org/downloads/">
   <img src="https://img.shields.io/pypi/pyversions/tsugu-api-python" alt="Python Version">
 </a>
 
+<a href="https://pypi.org/project/tsugu-api-python/">
+  <img src="https://img.shields.io/pypi/v/tsugu-api-python" alt="PyPI Version">
+</a>
+
 </p>
 
 ## 说明
 
 这是一个用 Python 编写的调用 [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file) 相关各种功能 API 的库，包括绝大部分 Tsugu 提供的功能。使用本 API 库提供的方法可以实现绝大部分功能，而搭配 [bestdori-api](https://github.com/WindowsSov8forUs/bestdori-api) 可以实现用户绑定等其他功能。
 
 > 该 API 库同时提供了异步与同步版本，可自行选择使用。
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
-          _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
+   _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _V_e_r_s_i_o_n_]
 ## è¯´æ è¿æ¯ä¸ä¸ªç¨ Python ç¼åçè°ç¨ [TsuguBanGDreamBot](https://
 github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file)
 ç¸å³åç§åè½ API çåºï¼åæ¬ç»å¤§é¨å Tsugu
 æä¾çåè½ãä½¿ç¨æ¬ API
 åºæä¾çæ¹æ³å¯ä»¥å®ç°ç»å¤§é¨ååè½ï¼èæ­é [bestdori-api]
 (https://github.com/WindowsSov8forUs/bestdori-api)
 å¯ä»¥å®ç°ç¨æ·ç»å®ç­å¶ä»åè½ã > è¯¥ API
```

### Comparing `tsugu-api-python-1.0.0/setup.py` & `tsugu-api-python-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='1.0.0',
+    version='1.0.1',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
@@ -17,8 +17,12 @@
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     python_requires='>=3.8',
+    install_requires=[
+        'httpx>=0.18.2',
+        'aiohttp>=3.7.4'
+    ]
 )
```

### Comparing `tsugu-api-python-1.0.0/tsugu_api/__init__.py` & `tsugu-api-python-1.0.1/tsugu_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api/_bandoristation.py` & `tsugu-api-python-1.0.1/tsugu_api/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api/_network.py` & `tsugu-api-python-1.0.1/tsugu_api/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api/_station.py` & `tsugu-api-python-1.0.1/tsugu_api/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api/_tsugu.py` & `tsugu-api-python-1.0.1/tsugu_api/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api/_typing.py` & `tsugu-api-python-1.0.1/tsugu_api/_typing.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api/_user.py` & `tsugu-api-python-1.0.1/tsugu_api/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api/settings.py` & `tsugu-api-python-1.0.1/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api/utils.py` & `tsugu-api-python-1.0.1/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api_async/__init__.py` & `tsugu-api-python-1.0.1/tsugu_api_async/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api_async/_bandoristation.py` & `tsugu-api-python-1.0.1/tsugu_api_async/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api_async/_network.py` & `tsugu-api-python-1.0.1/tsugu_api_async/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api_async/_station.py` & `tsugu-api-python-1.0.1/tsugu_api_async/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api_async/_tsugu.py` & `tsugu-api-python-1.0.1/tsugu_api_async/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api_async/_typing.py` & `tsugu-api-python-1.0.1/tsugu_api_async/_typing.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api_async/_user.py` & `tsugu-api-python-1.0.1/tsugu_api_async/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api_async/settings.py` & `tsugu-api-python-1.0.1/tsugu_api_async/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api_async/utils.py` & `tsugu-api-python-1.0.1/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.0/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-1.0.1/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
         
@@ -30,14 +30,18 @@
           <img src="https://img.shields.io/github/license/WindowsSov8forUs/tsugu-api-python" alt="License">
         </a>
         
         <a href="https://www.python.org/downloads/">
           <img src="https://img.shields.io/pypi/pyversions/tsugu-api-python" alt="Python Version">
         </a>
         
+        <a href="https://pypi.org/project/tsugu-api-python/">
+          <img src="https://img.shields.io/pypi/v/tsugu-api-python" alt="PyPI Version">
+        </a>
+        
         </p>
         
         ## 说明
         
         这是一个用 Python 编写的调用 [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file) 相关各种功能 API 的库，包括绝大部分 Tsugu 提供的功能。使用本 API 库提供的方法可以实现绝大部分功能，而搭配 [bestdori-api](https://github.com/WindowsSov8forUs/bestdori-api) 可以实现用户绑定等其他功能。
         
         > 该 API 库同时提供了异步与同步版本，可自行选择使用。
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.0 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.1 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
-          _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
+   _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _V_e_r_s_i_o_n_]
 ## è¯´æ è¿æ¯ä¸ä¸ªç¨ Python ç¼åçè°ç¨ [TsuguBanGDreamBot](https://
 github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file)
 ç¸å³åç§åè½ API çåºï¼åæ¬ç»å¤§é¨å Tsugu
 æä¾çåè½ãä½¿ç¨æ¬ API
 åºæä¾çæ¹æ³å¯ä»¥å®ç°ç»å¤§é¨ååè½ï¼èæ­é [bestdori-api]
 (https://github.com/WindowsSov8forUs/bestdori-api)
 å¯ä»¥å®ç°ç¨æ·ç»å®ç­å¶ä»åè½ã > è¯¥ API
```

### Comparing `tsugu-api-python-1.0.0/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-1.0.1/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 tsugu_api_async/_user.py
 tsugu_api_async/exception.py
 tsugu_api_async/settings.py
 tsugu_api_async/utils.py
 tsugu_api_python.egg-info/PKG-INFO
 tsugu_api_python.egg-info/SOURCES.txt
 tsugu_api_python.egg-info/dependency_links.txt
+tsugu_api_python.egg-info/requires.txt
 tsugu_api_python.egg-info/top_level.txt
```

