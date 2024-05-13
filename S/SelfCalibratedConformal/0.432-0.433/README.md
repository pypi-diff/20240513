# Comparing `tmp/SelfCalibratedConformal-0.432.tar.gz` & `tmp/SelfCalibratedConformal-0.433.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SelfCalibratedConformal-0.432.tar", last modified: Mon May 13 03:53:36 2024, max compression
+gzip compressed data, was "dist/SelfCalibratedConformal-0.433.tar", last modified: Mon May 13 03:54:45 2024, max compression
```

## Comparing `SelfCalibratedConformal-0.432.tar` & `SelfCalibratedConformal-0.433.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-13 03:53:36.000000 SelfCalibratedConformal-0.432/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      595 2024-05-13 03:53:36.000000 SelfCalibratedConformal-0.432/PKG-INFO
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-13 03:53:36.000000 SelfCalibratedConformal-0.432/SelfCalibratedConformal.egg-info/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      595 2024-05-13 03:53:36.000000 SelfCalibratedConformal-0.432/SelfCalibratedConformal.egg-info/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-13 03:53:36.000000 SelfCalibratedConformal-0.432/SelfCalibratedConformal.egg-info/SOURCES.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-13 03:53:36.000000 SelfCalibratedConformal-0.432/SelfCalibratedConformal.egg-info/requires.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-13 03:53:36.000000 SelfCalibratedConformal-0.432/SelfCalibratedConformal.egg-info/top_level.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-13 03:53:36.000000 SelfCalibratedConformal-0.432/SelfCalibratedConformal.egg-info/dependency_links.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.432/README.md
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      994 2024-05-13 03:53:32.000000 SelfCalibratedConformal-0.432/setup.py
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-13 03:53:36.000000 SelfCalibratedConformal-0.432/setup.cfg
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-13 03:54:45.000000 SelfCalibratedConformal-0.433/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      595 2024-05-13 03:54:45.000000 SelfCalibratedConformal-0.433/PKG-INFO
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-13 03:54:45.000000 SelfCalibratedConformal-0.433/SelfCalibratedConformal.egg-info/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      595 2024-05-13 03:54:45.000000 SelfCalibratedConformal-0.433/SelfCalibratedConformal.egg-info/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-13 03:54:45.000000 SelfCalibratedConformal-0.433/SelfCalibratedConformal.egg-info/SOURCES.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-13 03:54:45.000000 SelfCalibratedConformal-0.433/SelfCalibratedConformal.egg-info/requires.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-13 03:54:45.000000 SelfCalibratedConformal-0.433/SelfCalibratedConformal.egg-info/top_level.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-13 03:54:45.000000 SelfCalibratedConformal-0.433/SelfCalibratedConformal.egg-info/dependency_links.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.433/README.md
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      994 2024-05-13 03:54:41.000000 SelfCalibratedConformal-0.433/setup.py
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-13 03:54:45.000000 SelfCalibratedConformal-0.433/setup.cfg
```

### Comparing `SelfCalibratedConformal-0.432/PKG-INFO` & `SelfCalibratedConformal-0.433/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.432
+Version: 0.433
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 License: UNKNOWN
 Description: A Python implementation of Self-Calibrated Conformal Prediction
 Platform: UNKNOWN
```

### Comparing `SelfCalibratedConformal-0.432/SelfCalibratedConformal.egg-info/PKG-INFO` & `SelfCalibratedConformal-0.433/SelfCalibratedConformal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.432
+Version: 0.433
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 License: UNKNOWN
 Description: A Python implementation of Self-Calibrated Conformal Prediction
 Platform: UNKNOWN
```

### Comparing `SelfCalibratedConformal-0.432/setup.py` & `SelfCalibratedConformal-0.433/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SelfCalibratedConformal',
-    version='0.432',
+    version='0.433',
     packages=find_packages(),
     description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description_content_type='text/markdown',  # assuming your description is in Markdown format
     author='Lars van der Laan',
     author_email='vanderlaanlars@yahoo.com',
     url='https://github.com/Larsvanderlaan/SelfCalibratedConformal',
```

