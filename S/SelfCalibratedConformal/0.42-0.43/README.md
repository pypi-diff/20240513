# Comparing `tmp/SelfCalibratedConformal-0.42.tar.gz` & `tmp/SelfCalibratedConformal-0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SelfCalibratedConformal-0.42.tar", last modified: Sun May 12 19:23:49 2024, max compression
+gzip compressed data, was "SelfCalibratedConformal-0.43.tar", last modified: Mon May 13 03:37:33 2024, max compression
```

## Comparing `SelfCalibratedConformal-0.42.tar` & `SelfCalibratedConformal-0.43.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 19:23:49.802755 SelfCalibratedConformal-0.42/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 19:23:49.761559 SelfCalibratedConformal-0.42/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.42/README.md
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 19:23:49.761372 SelfCalibratedConformal-0.42/SelfCalibratedConformal.egg-info/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 19:23:49.000000 SelfCalibratedConformal-0.42/SelfCalibratedConformal.egg-info/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-12 19:23:49.000000 SelfCalibratedConformal-0.42/SelfCalibratedConformal.egg-info/SOURCES.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 19:23:49.000000 SelfCalibratedConformal-0.42/SelfCalibratedConformal.egg-info/dependency_links.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-12 19:23:49.000000 SelfCalibratedConformal-0.42/SelfCalibratedConformal.egg-info/requires.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 19:23:49.000000 SelfCalibratedConformal-0.42/SelfCalibratedConformal.egg-info/top_level.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-12 19:23:49.802857 SelfCalibratedConformal-0.42/setup.cfg
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      993 2024-05-12 19:23:39.000000 SelfCalibratedConformal-0.42/setup.py
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-13 03:37:33.696081 SelfCalibratedConformal-0.43/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-13 03:37:33.695912 SelfCalibratedConformal-0.43/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.43/README.md
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-13 03:37:33.695728 SelfCalibratedConformal-0.43/SelfCalibratedConformal.egg-info/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-13 03:37:33.000000 SelfCalibratedConformal-0.43/SelfCalibratedConformal.egg-info/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-13 03:37:33.000000 SelfCalibratedConformal-0.43/SelfCalibratedConformal.egg-info/SOURCES.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-13 03:37:33.000000 SelfCalibratedConformal-0.43/SelfCalibratedConformal.egg-info/dependency_links.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-13 03:37:33.000000 SelfCalibratedConformal-0.43/SelfCalibratedConformal.egg-info/requires.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-13 03:37:33.000000 SelfCalibratedConformal-0.43/SelfCalibratedConformal.egg-info/top_level.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-13 03:37:33.696131 SelfCalibratedConformal-0.43/setup.cfg
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      993 2024-05-13 03:37:23.000000 SelfCalibratedConformal-0.43/setup.py
```

### Comparing `SelfCalibratedConformal-0.42/PKG-INFO` & `SelfCalibratedConformal-0.43/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.42
+Version: 0.43
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SelfCalibratedConformal-0.42/SelfCalibratedConformal.egg-info/PKG-INFO` & `SelfCalibratedConformal-0.43/SelfCalibratedConformal.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.42
+Version: 0.43
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SelfCalibratedConformal-0.42/setup.py` & `SelfCalibratedConformal-0.43/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SelfCalibratedConformal',
-    version='0.42',
+    version='0.43',
     packages=find_packages(),
     description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description_content_type='text/markdown',  # assuming your description is in Markdown format
     author='Lars van der Laan',
     author_email='vanderlaanlars@yahoo.com',
     url='https://github.com/Larsvanderlaan/SelfCalibratedConformal',
```

