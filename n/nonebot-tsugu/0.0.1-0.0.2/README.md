# Comparing `tmp/nonebot_tsugu-0.0.1.tar.gz` & `tmp/nonebot_tsugu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_tsugu-0.0.1.tar", last modified: Mon May 13 03:00:31 2024, max compression
+gzip compressed data, was "nonebot_tsugu-0.0.2.tar", last modified: Mon May 13 03:40:17 2024, max compression
```

## Comparing `nonebot_tsugu-0.0.1.tar` & `nonebot_tsugu-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 03:00:31.662693 nonebot_tsugu-0.0.1/
--rw-rw-rw-   0        0        0     2749 2024-05-13 03:00:31.661692 nonebot_tsugu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2024-05-13 01:32:36.000000 nonebot_tsugu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 03:00:31.650690 nonebot_tsugu-0.0.1/nonebot_tsugu/
--rw-rw-rw-   0        0        0    17965 2024-05-13 01:01:39.000000 nonebot_tsugu-0.0.1/nonebot_tsugu/__init__.py
--rw-rw-rw-   0        0        0    15478 2024-05-13 01:06:00.000000 nonebot_tsugu-0.0.1/nonebot_tsugu/api.py
--rw-rw-rw-   0        0        0     4184 2024-05-13 02:27:10.000000 nonebot_tsugu-0.0.1/nonebot_tsugu/entity.py
--rw-rw-rw-   0        0        0     3741 2024-05-13 00:50:02.000000 nonebot_tsugu-0.0.1/nonebot_tsugu/util.py
-drwxrwxrwx   0        0        0        0 2024-05-13 03:00:31.659692 nonebot_tsugu-0.0.1/nonebot_tsugu.egg-info/
--rw-rw-rw-   0        0        0     2749 2024-05-13 03:00:31.000000 nonebot_tsugu-0.0.1/nonebot_tsugu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-05-13 03:00:31.000000 nonebot_tsugu-0.0.1/nonebot_tsugu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 03:00:31.000000 nonebot_tsugu-0.0.1/nonebot_tsugu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-13 03:00:31.000000 nonebot_tsugu-0.0.1/nonebot_tsugu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 03:00:31.000000 nonebot_tsugu-0.0.1/nonebot_tsugu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      107 2024-05-13 02:59:06.000000 nonebot_tsugu-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 03:00:31.662693 nonebot_tsugu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      774 2024-05-13 02:35:16.000000 nonebot_tsugu-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:40:17.915706 nonebot_tsugu-0.0.2/
+-rw-rw-rw-   0        0        0     2749 2024-05-13 03:40:17.914710 nonebot_tsugu-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2024-05-13 01:32:36.000000 nonebot_tsugu-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 03:40:17.903572 nonebot_tsugu-0.0.2/nonebot_tsugu/
+-rw-rw-rw-   0        0        0    17965 2024-05-13 01:01:39.000000 nonebot_tsugu-0.0.2/nonebot_tsugu/__init__.py
+-rw-rw-rw-   0        0        0    15478 2024-05-13 01:06:00.000000 nonebot_tsugu-0.0.2/nonebot_tsugu/api.py
+-rw-rw-rw-   0        0        0     4184 2024-05-13 02:27:10.000000 nonebot_tsugu-0.0.2/nonebot_tsugu/entity.py
+-rw-rw-rw-   0        0        0     3741 2024-05-13 00:50:02.000000 nonebot_tsugu-0.0.2/nonebot_tsugu/util.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:40:17.912197 nonebot_tsugu-0.0.2/nonebot_tsugu.egg-info/
+-rw-rw-rw-   0        0        0     2749 2024-05-13 03:40:17.000000 nonebot_tsugu-0.0.2/nonebot_tsugu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-13 03:40:17.000000 nonebot_tsugu-0.0.2/nonebot_tsugu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 03:40:17.000000 nonebot_tsugu-0.0.2/nonebot_tsugu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-13 03:40:17.000000 nonebot_tsugu-0.0.2/nonebot_tsugu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 03:40:17.000000 nonebot_tsugu-0.0.2/nonebot_tsugu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      179 2024-05-13 03:39:38.000000 nonebot_tsugu-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 03:40:17.915706 nonebot_tsugu-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      774 2024-05-13 03:37:05.000000 nonebot_tsugu-0.0.2/setup.py
```

### Comparing `nonebot_tsugu-0.0.1/PKG-INFO` & `nonebot_tsugu-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_tsugu
-Version: 0.0.1
+Version: 0.0.2
 Summary: 基于tsugu-bangdream-bot项目实现的nonebot2插件
 Home-page: https://github.com/otae-1204/NoneBot-Tsugu
 Author: otae
 Author-email: otae1204@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nonebot_tsugu-0.0.1/README.md` & `nonebot_tsugu-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_tsugu-0.0.1/nonebot_tsugu/__init__.py` & `nonebot_tsugu-0.0.2/nonebot_tsugu/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_tsugu-0.0.1/nonebot_tsugu/api.py` & `nonebot_tsugu-0.0.2/nonebot_tsugu/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_tsugu-0.0.1/nonebot_tsugu/entity.py` & `nonebot_tsugu-0.0.2/nonebot_tsugu/entity.py`

 * *Files identical despite different names*

### Comparing `nonebot_tsugu-0.0.1/nonebot_tsugu/util.py` & `nonebot_tsugu-0.0.2/nonebot_tsugu/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_tsugu-0.0.1/nonebot_tsugu.egg-info/PKG-INFO` & `nonebot_tsugu-0.0.2/nonebot_tsugu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-tsugu
-Version: 0.0.1
+Version: 0.0.2
 Summary: 基于tsugu-bangdream-bot项目实现的nonebot2插件
 Home-page: https://github.com/otae-1204/NoneBot-Tsugu
 Author: otae
 Author-email: otae1204@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nonebot_tsugu-0.0.1/setup.py` & `nonebot_tsugu-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='nonebot_tsugu',
-    version='0.0.1',
+    version='0.0.2',
     author='otae',
     author_email='otae1204@qq.com',
     description='基于tsugu-bangdream-bot项目实现的nonebot2插件',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/otae-1204/NoneBot-Tsugu',
     include_package_data=False,
```

