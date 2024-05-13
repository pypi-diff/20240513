# Comparing `tmp/lxs_simpletools-1.0.0.tar.gz` & `tmp/lxs_simpletools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxs_simpletools-1.0.0.tar", last modified: Mon May 13 08:08:57 2024, max compression
+gzip compressed data, was "lxs_simpletools-1.0.1.tar", last modified: Mon May 13 08:49:38 2024, max compression
```

## Comparing `lxs_simpletools-1.0.0.tar` & `lxs_simpletools-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-13 08:08:57.637537 lxs_simpletools-1.0.0/
--rw-r--r--   0 root         (0) staff       (20)      511 2024-05-13 08:08:57.637340 lxs_simpletools-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-13 08:08:57.637122 lxs_simpletools-1.0.0/lxs_SimpleTools.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      511 2024-05-13 08:08:57.000000 lxs_simpletools-1.0.0/lxs_SimpleTools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      164 2024-05-13 08:08:57.000000 lxs_simpletools-1.0.0/lxs_SimpleTools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-05-13 08:08:57.000000 lxs_simpletools-1.0.0/lxs_SimpleTools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-05-13 08:08:57.000000 lxs_simpletools-1.0.0/lxs_SimpleTools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2024-05-13 08:08:57.637577 lxs_simpletools-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      693 2024-05-13 08:08:03.000000 lxs_simpletools-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-13 08:49:38.543135 lxs_simpletools-1.0.1/
+-rw-r--r--   0 root         (0) staff       (20)     7120 2024-05-13 08:49:38.542951 lxs_simpletools-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     6567 2024-05-13 08:49:25.000000 lxs_simpletools-1.0.1/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-13 08:49:38.542747 lxs_simpletools-1.0.1/lxs_SimpleTools.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     7120 2024-05-13 08:49:38.000000 lxs_simpletools-1.0.1/lxs_SimpleTools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      174 2024-05-13 08:49:38.000000 lxs_simpletools-1.0.1/lxs_SimpleTools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-13 08:49:38.000000 lxs_simpletools-1.0.1/lxs_SimpleTools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-13 08:49:38.000000 lxs_simpletools-1.0.1/lxs_SimpleTools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-13 08:49:38.543174 lxs_simpletools-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      868 2024-05-13 08:12:50.000000 lxs_simpletools-1.0.1/setup.py
```

### Comparing `lxs_simpletools-1.0.0/setup.py` & `lxs_simpletools-1.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from setuptools import setup, find_packages
 
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
+
 setup(
     name='lxs-SimpleTools',
-    version='1.0.0',
+    version='1.0.1',
     author='liuxiansong',
     author_email='326427540@qq.com',
     description='处理字符串和时间简单工具函数',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     packages=find_packages(),  # 自动查找并包含所有的包
     install_requires=[
 
     ],
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

