# Comparing `tmp/test-set-sdk-1.0.12.tar.gz` & `tmp/test-set-sdk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/test-set-sdk-1.0.12.tar", last modified: Mon May 13 03:35:28 2024, max compression
+gzip compressed data, was "dist/test-set-sdk-1.0.5.tar", last modified: Fri Mar  1 12:08:02 2024, max compression
```

## Comparing `test-set-sdk-1.0.12.tar` & `test-set-sdk-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-13 03:35:28.000000 test-set-sdk-1.0.12/
--rw-r--r--   0 bytedance   (501) staff       (20)      268 2024-05-13 03:35:28.000000 test-set-sdk-1.0.12/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      616 2024-05-13 03:35:12.000000 test-set-sdk-1.0.12/setup.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-13 03:35:28.000000 test-set-sdk-1.0.12/test_set_sdk.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)      268 2024-05-13 03:35:28.000000 test-set-sdk-1.0.12/test_set_sdk.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      292 2024-05-13 03:35:28.000000 test-set-sdk-1.0.12/test_set_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)      103 2024-05-13 03:35:28.000000 test-set-sdk-1.0.12/test_set_sdk.egg-info/requires.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       10 2024-05-13 03:35:28.000000 test-set-sdk-1.0.12/test_set_sdk.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2024-05-13 03:35:28.000000 test-set-sdk-1.0.12/test_set_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2024-05-13 03:35:28.000000 test-set-sdk-1.0.12/setup.cfg
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-13 03:35:28.000000 test-set-sdk-1.0.12/testsetup/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2024-05-13 03:35:12.000000 test-set-sdk-1.0.12/testsetup/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-13 03:35:28.000000 test-set-sdk-1.0.12/testsetup/testcl/
--rw-r--r--   0 bytedance   (501) staff       (20)       43 2024-05-13 03:35:12.000000 test-set-sdk-1.0.12/testsetup/testcl/test_01.py
--rw-r--r--   0 bytedance   (501) staff       (20)       88 2024-05-13 03:35:12.000000 test-set-sdk-1.0.12/testsetup/testcl/test1.py
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2024-05-13 03:35:12.000000 test-set-sdk-1.0.12/testsetup/testcl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 12:08:02.000000 test-set-sdk-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-01 12:08:02.000000 test-set-sdk-1.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 12:08:02.000000 test-set-sdk-1.0.5/test_set_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      227 2024-03-01 12:08:02.000000 test-set-sdk-1.0.5/test_set_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 12:08:02.000000 test-set-sdk-1.0.5/test_set_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      267 2024-03-01 12:08:02.000000 test-set-sdk-1.0.5/test_set_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       10 2024-03-01 12:08:02.000000 test-set-sdk-1.0.5/test_set_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2024-03-01 12:08:02.000000 test-set-sdk-1.0.5/test_set_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      267 2024-03-01 12:08:02.000000 test-set-sdk-1.0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 12:08:02.000000 test-set-sdk-1.0.5/testsetup/
+-rw-r--r--   0 root         (0) root         (0)       44 2024-03-01 11:34:21.000000 test-set-sdk-1.0.5/testsetup/test.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-01 11:33:52.000000 test-set-sdk-1.0.5/testsetup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      585 2024-03-01 12:07:40.000000 test-set-sdk-1.0.5/setup.py
```

### Comparing `test-set-sdk-1.0.12/setup.py` & `test-set-sdk-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-# coding:utf-8
-import sys
-
 from setuptools import setup, find_packages
 
 install_requires = [
     "requests>=2.25.1",
     "retry==0.9.2",
     "pytz==2020.5",
     "pycryptodome==3.9.9",
     "protobuf>=3.18.3",
     "google>=3.0.0",
     "six>=1.0",
 ]
-
 setup(
     name="test-set-sdk",
-    version="1.0.12",
+    version="1.0.5",
     keywords=("pip", "test", "test-set-sdk"),
     description="The test set SDK for Python",
     license="MIT License",
-
     url="https://github.com/johlin/test3",
     author="test-set SDK",
-
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
     install_requires=install_requires
 )
```

