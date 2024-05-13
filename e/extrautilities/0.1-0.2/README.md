# Comparing `tmp/extrautilities-0.1.tar.gz` & `tmp/extrautilities-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-0.1.tar", last modified: Sun May 12 12:11:14 2024, max compression
+gzip compressed data, was "extrautilities-0.2.tar", last modified: Mon May 13 17:09:20 2024, max compression
```

## Comparing `extrautilities-0.1.tar` & `extrautilities-0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 12:11:14.425215 extrautilities-0.1/
-drwxrwxrwx   0        0        0        0 2024-05-12 12:11:14.408561 extrautilities-0.1/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.1/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.1/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0     2349 2024-05-12 12:11:14.424211 extrautilities-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1514 2024-05-12 12:05:10.000000 extrautilities-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 12:11:14.423714 extrautilities-0.1/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     2349 2024-05-12 12:11:14.000000 extrautilities-0.1/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-12 12:11:14.000000 extrautilities-0.1/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 12:11:14.000000 extrautilities-0.1/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-12 12:11:14.000000 extrautilities-0.1/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-12 12:11:14.000000 extrautilities-0.1/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 12:11:14.425215 extrautilities-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1040 2024-05-12 12:11:08.000000 extrautilities-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:09:20.687574 extrautilities-0.2/
+drwxrwxrwx   0        0        0        0 2024-05-13 17:09:20.676049 extrautilities-0.2/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.2/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.2/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0     1407 2024-05-13 17:07:47.000000 extrautilities-0.2/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0     2349 2024-05-13 17:09:20.687574 extrautilities-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1514 2024-05-12 12:05:10.000000 extrautilities-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 17:09:20.686571 extrautilities-0.2/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     2349 2024-05-13 17:09:20.000000 extrautilities-0.2/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-13 17:09:20.000000 extrautilities-0.2/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 17:09:20.000000 extrautilities-0.2/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-13 17:09:20.000000 extrautilities-0.2/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 17:09:20.000000 extrautilities-0.2/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 17:09:20.688079 extrautilities-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-13 17:09:18.000000 extrautilities-0.2/setup.py
```

### Comparing `extrautilities-0.1/ExtraUtils/RateLimit.py` & `extrautilities-0.2/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-0.1/PKG-INFO` & `extrautilities-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.1
+Version: 0.2
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit
 Platform: UNKNOWN
```

### Comparing `extrautilities-0.1/README.md` & `extrautilities-0.2/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-0.1/extrautilities.egg-info/PKG-INFO` & `extrautilities-0.2/extrautilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.1
+Version: 0.2
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit
 Platform: UNKNOWN
```

### Comparing `extrautilities-0.1/setup.py` & `extrautilities-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
@@ -19,9 +19,9 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     keywords='RateLimit',
-    install_requires=["extradecorators"],
+    install_requires=["extradecorators", "cryptography"],
 )
```

