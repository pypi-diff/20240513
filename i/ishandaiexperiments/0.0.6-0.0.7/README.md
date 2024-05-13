# Comparing `tmp/ishandaiexperiments-0.0.6.tar.gz` & `tmp/ishandaiexperiments-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ishandaiexperiments-0.0.6.tar", last modified: Mon May 13 19:42:20 2024, max compression
+gzip compressed data, was "ishandaiexperiments-0.0.7.tar", last modified: Mon May 13 19:46:58 2024, max compression
```

## Comparing `ishandaiexperiments-0.0.6.tar` & `ishandaiexperiments-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 19:42:20.593609 ishandaiexperiments-0.0.6/
--rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 ishandaiexperiments-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 ishandaiexperiments-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 ishandaiexperiments-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      613 2024-05-13 19:42:20.591754 ishandaiexperiments-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-05-13 17:37:56.000000 ishandaiexperiments-0.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 19:42:20.527569 ishandaiexperiments-0.0.6/ishandaiexperiments/
--rw-rw-rw-   0        0        0       44 2024-05-13 19:26:19.000000 ishandaiexperiments-0.0.6/ishandaiexperiments/__init__.py
--rw-rw-rw-   0        0        0     4264 2024-05-13 19:41:56.000000 ishandaiexperiments-0.0.6/ishandaiexperiments/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 19:42:20.588656 ishandaiexperiments-0.0.6/ishandaiexperiments.egg-info/
--rw-rw-rw-   0        0        0      613 2024-05-13 19:42:20.000000 ishandaiexperiments-0.0.6/ishandaiexperiments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-05-13 19:42:20.000000 ishandaiexperiments-0.0.6/ishandaiexperiments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 19:42:20.000000 ishandaiexperiments-0.0.6/ishandaiexperiments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-13 19:42:20.000000 ishandaiexperiments-0.0.6/ishandaiexperiments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 19:42:20.594402 ishandaiexperiments-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      713 2024-05-13 19:42:11.000000 ishandaiexperiments-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:46:58.357147 ishandaiexperiments-0.0.7/
+-rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 ishandaiexperiments-0.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 ishandaiexperiments-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 ishandaiexperiments-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      613 2024-05-13 19:46:58.355216 ishandaiexperiments-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-05-13 17:37:56.000000 ishandaiexperiments-0.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 19:46:58.309316 ishandaiexperiments-0.0.7/ishandaiexperiments/
+-rw-rw-rw-   0        0        0       79 2024-05-13 19:45:11.000000 ishandaiexperiments-0.0.7/ishandaiexperiments/__init__.py
+-rw-rw-rw-   0        0        0     4264 2024-05-13 19:41:56.000000 ishandaiexperiments-0.0.7/ishandaiexperiments/main.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:46:58.352211 ishandaiexperiments-0.0.7/ishandaiexperiments.egg-info/
+-rw-rw-rw-   0        0        0      613 2024-05-13 19:46:57.000000 ishandaiexperiments-0.0.7/ishandaiexperiments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-05-13 19:46:58.000000 ishandaiexperiments-0.0.7/ishandaiexperiments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 19:46:57.000000 ishandaiexperiments-0.0.7/ishandaiexperiments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-13 19:46:57.000000 ishandaiexperiments-0.0.7/ishandaiexperiments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 19:46:58.357905 ishandaiexperiments-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      713 2024-05-13 19:46:54.000000 ishandaiexperiments-0.0.7/setup.py
```

### Comparing `ishandaiexperiments-0.0.6/LICENSE.txt` & `ishandaiexperiments-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ishandaiexperiments-0.0.6/PKG-INFO` & `ishandaiexperiments-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ishandaiexperiments
-Version: 0.0.6
+Version: 0.0.7
 Summary: dai experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ishandaiexperiments-0.0.6/ishandaiexperiments/main.py` & `ishandaiexperiments-0.0.7/ishandaiexperiments/main.py`

 * *Files identical despite different names*

### Comparing `ishandaiexperiments-0.0.6/ishandaiexperiments.egg-info/PKG-INFO` & `ishandaiexperiments-0.0.7/ishandaiexperiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ishandaiexperiments
-Version: 0.0.6
+Version: 0.0.7
 Summary: dai experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ishandaiexperiments-0.0.6/setup.py` & `ishandaiexperiments-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ishandaiexperiments',
-  version='0.0.6',
+  version='0.0.7',
   description='dai experiments',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='S Ishan',
   author_email='is9678@srmist.edu.in',
   license='MIT', 
   classifiers=classifiers,
```

