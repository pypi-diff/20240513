# Comparing `tmp/binpolar-0.1.tar.gz` & `tmp/binpolar-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binpolar-0.1.tar", last modified: Mon May 13 04:22:01 2024, max compression
+gzip compressed data, was "binpolar-0.3.tar", last modified: Mon May 13 06:30:13 2024, max compression
```

## Comparing `binpolar-0.1.tar` & `binpolar-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 04:22:01.818644 binpolar-0.1/
--rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 04:22:01.818465 binpolar-0.1/PKG-INFO
--rw-r--r--   0 joycelee   (501) staff       (20)        3 2024-05-13 03:33:09.000000 binpolar-0.1/README.md
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 04:22:01.817589 binpolar-0.1/binpolar/
--rw-r--r--   0 joycelee   (501) staff       (20)      278 2024-05-13 03:26:54.000000 binpolar-0.1/binpolar/__init__.py
--rw-r--r--   0 joycelee   (501) staff       (20)      624 2024-05-13 03:39:52.000000 binpolar-0.1/binpolar/polarity_detector.py
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 04:22:01.818298 binpolar-0.1/binpolar.egg-info/
--rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 04:22:01.000000 binpolar-0.1/binpolar.egg-info/PKG-INFO
--rw-r--r--   0 joycelee   (501) staff       (20)      228 2024-05-13 04:22:01.000000 binpolar-0.1/binpolar.egg-info/SOURCES.txt
--rw-r--r--   0 joycelee   (501) staff       (20)        1 2024-05-13 04:22:01.000000 binpolar-0.1/binpolar.egg-info/dependency_links.txt
--rw-r--r--   0 joycelee   (501) staff       (20)       13 2024-05-13 04:22:01.000000 binpolar-0.1/binpolar.egg-info/requires.txt
--rw-r--r--   0 joycelee   (501) staff       (20)        9 2024-05-13 04:22:01.000000 binpolar-0.1/binpolar.egg-info/top_level.txt
--rw-r--r--   0 joycelee   (501) staff       (20)       38 2024-05-13 04:22:01.818702 binpolar-0.1/setup.cfg
--rw-r--r--   0 joycelee   (501) staff       (20)      853 2024-05-13 03:24:32.000000 binpolar-0.1/setup.py
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:30:13.367291 binpolar-0.3/
+-rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 06:30:13.367093 binpolar-0.3/PKG-INFO
+-rw-r--r--   0 joycelee   (501) staff       (20)        3 2024-05-13 03:33:09.000000 binpolar-0.3/README.md
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:30:13.366094 binpolar-0.3/binpolar/
+-rw-r--r--   0 joycelee   (501) staff       (20)       54 2024-05-13 06:21:47.000000 binpolar-0.3/binpolar/__init__.py
+-rw-r--r--   0 joycelee   (501) staff       (20)     1178 2024-05-13 06:26:35.000000 binpolar-0.3/binpolar/polarity_detector.py
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:30:13.366891 binpolar-0.3/binpolar.egg-info/
+-rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 06:30:13.000000 binpolar-0.3/binpolar.egg-info/PKG-INFO
+-rw-r--r--   0 joycelee   (501) staff       (20)      228 2024-05-13 06:30:13.000000 binpolar-0.3/binpolar.egg-info/SOURCES.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)        1 2024-05-13 06:30:13.000000 binpolar-0.3/binpolar.egg-info/dependency_links.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)       13 2024-05-13 06:30:13.000000 binpolar-0.3/binpolar.egg-info/requires.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)        9 2024-05-13 06:30:13.000000 binpolar-0.3/binpolar.egg-info/top_level.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)       38 2024-05-13 06:30:13.367343 binpolar-0.3/setup.cfg
+-rw-r--r--   0 joycelee   (501) staff       (20)      853 2024-05-13 06:30:00.000000 binpolar-0.3/setup.py
```

### Comparing `binpolar-0.1/PKG-INFO` & `binpolar-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binpolar
-Version: 0.1
+Version: 0.3
 Summary: Binary polarity detection
 Author: Joyce Lee
 Author-email: <leejoy1610@gmail.com>
 Keywords: python,text,polarity
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binpolar-0.1/binpolar.egg-info/PKG-INFO` & `binpolar-0.3/binpolar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binpolar
-Version: 0.1
+Version: 0.3
 Summary: Binary polarity detection
 Author: Joyce Lee
 Author-email: <leejoy1610@gmail.com>
 Keywords: python,text,polarity
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binpolar-0.1/setup.py` & `binpolar-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1'
+VERSION = '0.3'
 DESCRIPTION = 'Binary polarity detection'
 LONG_DESCRIPTION = 'A fine-tuned DistilBERT model for binary polarity detection in text.'
 
 # Setting up
 setup(
     name="binpolar",
     version=VERSION,
```

