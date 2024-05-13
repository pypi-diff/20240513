# Comparing `tmp/dreamhack-1.1.4.tar.gz` & `tmp/dreamhack-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamhack-1.1.4.tar", last modified: Mon May 13 18:55:36 2024, max compression
+gzip compressed data, was "dreamhack-1.1.5.tar", last modified: Mon May 13 18:56:43 2024, max compression
```

## Comparing `dreamhack-1.1.4.tar` & `dreamhack-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 18:55:36.521979 dreamhack-1.1.4/
--rw-r--r--   0 runner    (1000) runner    (1000)     2503 2024-05-13 18:55:36.521979 dreamhack-1.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 18:55:36.517979 dreamhack-1.1.4/dreamhack/
--rw-r--r--   0 runner    (1000) runner    (1000)     2187 2024-05-13 18:30:56.000000 dreamhack-1.1.4/dreamhack/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.1.4/dreamhack/colorcodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.1.4/dreamhack/downloads.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.1.4/dreamhack/encryption.py
--rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-05-13 15:44:44.000000 dreamhack-1.1.4/dreamhack/filepaths.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.1.4/dreamhack/gui.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.1.4/dreamhack/logging.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.1.4/dreamhack/networking.py
--rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.1.4/dreamhack/randoms.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5726 2024-05-13 18:26:44.000000 dreamhack-1.1.4/dreamhack/registry.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7702 2024-05-13 18:55:10.000000 dreamhack-1.1.4/dreamhack/windows.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.1.4/dreamhack/zipfiles.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 18:55:36.521979 dreamhack-1.1.4/dreamhack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2503 2024-05-13 18:55:36.000000 dreamhack-1.1.4/dreamhack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-13 18:55:36.000000 dreamhack-1.1.4/dreamhack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-13 18:55:36.000000 dreamhack-1.1.4/dreamhack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      123 2024-05-13 18:55:36.000000 dreamhack-1.1.4/dreamhack.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-13 18:55:36.000000 dreamhack-1.1.4/dreamhack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-13 18:55:36.521979 dreamhack-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     2767 2024-05-13 18:31:33.000000 dreamhack-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 18:56:43.361889 dreamhack-1.1.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2541 2024-05-13 18:56:43.361889 dreamhack-1.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 18:56:43.361889 dreamhack-1.1.5/dreamhack/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2187 2024-05-13 18:30:56.000000 dreamhack-1.1.5/dreamhack/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.1.5/dreamhack/colorcodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.1.5/dreamhack/downloads.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.1.5/dreamhack/encryption.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-05-13 15:44:44.000000 dreamhack-1.1.5/dreamhack/filepaths.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.1.5/dreamhack/gui.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.1.5/dreamhack/logging.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.1.5/dreamhack/networking.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.1.5/dreamhack/randoms.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5726 2024-05-13 18:26:44.000000 dreamhack-1.1.5/dreamhack/registry.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7702 2024-05-13 18:55:10.000000 dreamhack-1.1.5/dreamhack/windows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.1.5/dreamhack/zipfiles.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 18:56:43.361889 dreamhack-1.1.5/dreamhack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2541 2024-05-13 18:56:43.000000 dreamhack-1.1.5/dreamhack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-13 18:56:43.000000 dreamhack-1.1.5/dreamhack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-13 18:56:43.000000 dreamhack-1.1.5/dreamhack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      123 2024-05-13 18:56:43.000000 dreamhack-1.1.5/dreamhack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-13 18:56:43.000000 dreamhack-1.1.5/dreamhack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-13 18:56:43.361889 dreamhack-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2807 2024-05-13 18:56:41.000000 dreamhack-1.1.5/setup.py
```

### Comparing `dreamhack-1.1.4/PKG-INFO` & `dreamhack-1.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.1.4
+Version: 1.1.5
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -22,14 +22,19 @@
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: 
 
+v1.1.5: 
+
+- Fixed error with pyuac 
+
+
 v1.1.4: 
 
 - Added a new function to update a python package 
 
 
 v1.1.3:
```

### Comparing `dreamhack-1.1.4/dreamhack/__init__.py` & `dreamhack-1.1.5/dreamhack/__init__.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack/colorcodes.py` & `dreamhack-1.1.5/dreamhack/colorcodes.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack/downloads.py` & `dreamhack-1.1.5/dreamhack/downloads.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack/encryption.py` & `dreamhack-1.1.5/dreamhack/encryption.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack/filepaths.py` & `dreamhack-1.1.5/dreamhack/filepaths.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack/gui.py` & `dreamhack-1.1.5/dreamhack/gui.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack/logging.py` & `dreamhack-1.1.5/dreamhack/logging.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack/networking.py` & `dreamhack-1.1.5/dreamhack/networking.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack/randoms.py` & `dreamhack-1.1.5/dreamhack/randoms.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack/registry.py` & `dreamhack-1.1.5/dreamhack/registry.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack/windows.py` & `dreamhack-1.1.5/dreamhack/windows.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack/zipfiles.py` & `dreamhack-1.1.5/dreamhack/zipfiles.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.1.4/dreamhack.egg-info/PKG-INFO` & `dreamhack-1.1.5/dreamhack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.1.4
+Version: 1.1.5
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -22,14 +22,19 @@
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: 
 
+v1.1.5: 
+
+- Fixed error with pyuac 
+
+
 v1.1.4: 
 
 - Added a new function to update a python package 
 
 
 v1.1.3:
```

### Comparing `dreamhack-1.1.4/setup.py` & `dreamhack-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
 #type:ignore
 
-VERSION = '1.1.4' 
+VERSION = '1.1.5' 
 DESCRIPTION = 'The ultimate PyPi package for cyber-security and many other things.'
 LONG_DESCRIPTION = '''The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 *DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes. 
 
 RELEASE NOTES: \n
+v1.1.5: \n
+- Fixed error with pyuac \n
+
 v1.1.4: \n
 - Added a new function to update a python package \n
 
 v1.1.3: \n
 - Added new error detection to registry class \n
 - Added a few new features \n
```

