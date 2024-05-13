# Comparing `tmp/extrautilities-0.2.tar.gz` & `tmp/extrautilities-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-0.2.tar", last modified: Mon May 13 17:09:20 2024, max compression
+gzip compressed data, was "extrautilities-0.3.tar", last modified: Mon May 13 17:30:38 2024, max compression
```

## Comparing `extrautilities-0.2.tar` & `extrautilities-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 17:09:20.687574 extrautilities-0.2/
-drwxrwxrwx   0        0        0        0 2024-05-13 17:09:20.676049 extrautilities-0.2/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.2/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.2/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0     1407 2024-05-13 17:07:47.000000 extrautilities-0.2/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0     2349 2024-05-13 17:09:20.687574 extrautilities-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1514 2024-05-12 12:05:10.000000 extrautilities-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 17:09:20.686571 extrautilities-0.2/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     2349 2024-05-13 17:09:20.000000 extrautilities-0.2/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-13 17:09:20.000000 extrautilities-0.2/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 17:09:20.000000 extrautilities-0.2/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-13 17:09:20.000000 extrautilities-0.2/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 17:09:20.000000 extrautilities-0.2/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 17:09:20.688079 extrautilities-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-13 17:09:18.000000 extrautilities-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:30:38.723534 extrautilities-0.3/
+drwxrwxrwx   0        0        0        0 2024-05-13 17:30:38.709870 extrautilities-0.3/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.3/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.3/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0     1400 2024-05-13 17:30:18.000000 extrautilities-0.3/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0     2349 2024-05-13 17:30:38.723029 extrautilities-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1514 2024-05-12 12:05:10.000000 extrautilities-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 17:30:38.722198 extrautilities-0.3/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     2349 2024-05-13 17:30:38.000000 extrautilities-0.3/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-13 17:30:38.000000 extrautilities-0.3/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 17:30:38.000000 extrautilities-0.3/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-13 17:30:38.000000 extrautilities-0.3/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 17:30:38.000000 extrautilities-0.3/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 17:30:38.723534 extrautilities-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-13 17:30:35.000000 extrautilities-0.3/setup.py
```

### Comparing `extrautilities-0.2/ExtraUtils/RateLimit.py` & `extrautilities-0.3/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-0.2/ExtraUtils/asyncTokens.py` & `extrautilities-0.3/ExtraUtils/asyncTokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         key_size=2048,
         backend=default_backend()
     )
     pub_key = priv_key.public_key()
     return (priv_key, pub_key)
 
 # Nachricht mit dem öffentlichen Schlüssel verschlüsseln
-def verschluesseln(nachricht, pub_key):
+def encrypt(nachricht, pub_key):
     return pub_key.encrypt(
         nachricht.encode(),
         padding.OAEP(
             mgf=padding.MGF1(algorithm=hashes.SHA256()),
             algorithm=hashes.SHA256(),
             label=None
         )
```

### Comparing `extrautilities-0.2/PKG-INFO` & `extrautilities-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.2
+Version: 0.3
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit
 Platform: UNKNOWN
```

### Comparing `extrautilities-0.2/README.md` & `extrautilities-0.3/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-0.2/extrautilities.egg-info/PKG-INFO` & `extrautilities-0.3/extrautilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.2
+Version: 0.3
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit
 Platform: UNKNOWN
```

### Comparing `extrautilities-0.2/setup.py` & `extrautilities-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
```

