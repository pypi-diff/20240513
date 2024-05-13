# Comparing `tmp/ishandaiexperiments-0.0.1.tar.gz` & `tmp/ishandaiexperiments-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ishandaiexperiments-0.0.1.tar", last modified: Mon May 13 17:48:57 2024, max compression
+gzip compressed data, was "ishandaiexperiments-0.0.2.tar", last modified: Mon May 13 18:32:51 2024, max compression
```

## Comparing `ishandaiexperiments-0.0.1.tar` & `ishandaiexperiments-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 17:48:57.941956 ishandaiexperiments-0.0.1/
--rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 ishandaiexperiments-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 ishandaiexperiments-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 ishandaiexperiments-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      613 2024-05-13 17:48:57.941287 ishandaiexperiments-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-05-13 17:37:56.000000 ishandaiexperiments-0.0.1/README.txt
--rw-rw-rw-   0        0        0     2074 2024-05-13 17:36:44.000000 ishandaiexperiments-0.0.1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:48:57.938934 ishandaiexperiments-0.0.1/ishandaiexperiments.egg-info/
--rw-rw-rw-   0        0        0      613 2024-05-13 17:48:57.000000 ishandaiexperiments-0.0.1/ishandaiexperiments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-05-13 17:48:57.000000 ishandaiexperiments-0.0.1/ishandaiexperiments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 17:48:57.000000 ishandaiexperiments-0.0.1/ishandaiexperiments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 17:48:57.000000 ishandaiexperiments-0.0.1/ishandaiexperiments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 17:48:57.942469 ishandaiexperiments-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      682 2024-05-13 17:42:16.000000 ishandaiexperiments-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:32:51.207000 ishandaiexperiments-0.0.2/
+-rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 ishandaiexperiments-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 ishandaiexperiments-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 ishandaiexperiments-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      613 2024-05-13 18:32:51.205975 ishandaiexperiments-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-05-13 17:37:56.000000 ishandaiexperiments-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 18:32:51.185403 ishandaiexperiments-0.0.2/exp/
+-rw-rw-rw-   0        0        0     2074 2024-05-13 17:36:44.000000 ishandaiexperiments-0.0.2/exp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:32:51.204082 ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/
+-rw-rw-rw-   0        0        0      613 2024-05-13 18:32:51.000000 ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-05-13 18:32:51.000000 ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:32:51.000000 ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:32:51.000000 ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 18:32:51.207000 ishandaiexperiments-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-05-13 18:32:21.000000 ishandaiexperiments-0.0.2/setup.py
```

### Comparing `ishandaiexperiments-0.0.1/LICENSE.txt` & `ishandaiexperiments-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ishandaiexperiments-0.0.1/PKG-INFO` & `ishandaiexperiments-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ishandaiexperiments
-Version: 0.0.1
+Version: 0.0.2
 Summary: dai experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ishandaiexperiments-0.0.1/__init__.py` & `ishandaiexperiments-0.0.2/exp/__init__.py`

 * *Files identical despite different names*

### Comparing `ishandaiexperiments-0.0.1/ishandaiexperiments.egg-info/PKG-INFO` & `ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ishandaiexperiments
-Version: 0.0.1
+Version: 0.0.2
 Summary: dai experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ishandaiexperiments-0.0.1/setup.py` & `ishandaiexperiments-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,19 +6,20 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ishandaiexperiments',
-  version='0.0.1',
+  version='0.0.2',
   description='dai experiments',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='S Ishan',
   author_email='is9678@srmist.edu.in',
   license='MIT', 
   classifiers=classifiers,
   keywords='dai', 
-  packages=find_packages(),
+  packages=find_packages('exp'),
+  include_package_data= True,
   install_requires=[''] 
 )
```

