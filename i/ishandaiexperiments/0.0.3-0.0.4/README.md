# Comparing `tmp/ishandaiexperiments-0.0.3.tar.gz` & `tmp/ishandaiexperiments-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ishandaiexperiments-0.0.3.tar", last modified: Mon May 13 18:43:45 2024, max compression
+gzip compressed data, was "ishandaiexperiments-0.0.4.tar", last modified: Mon May 13 18:46:53 2024, max compression
```

## Comparing `ishandaiexperiments-0.0.3.tar` & `ishandaiexperiments-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 18:43:45.634549 ishandaiexperiments-0.0.3/
--rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 ishandaiexperiments-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 ishandaiexperiments-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 ishandaiexperiments-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      613 2024-05-13 18:43:45.633549 ishandaiexperiments-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-05-13 17:37:56.000000 ishandaiexperiments-0.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 18:43:45.579533 ishandaiexperiments-0.0.3/ishandaiexperiments/
--rw-rw-rw-   0        0        0       75 2024-05-13 18:40:39.000000 ishandaiexperiments-0.0.3/ishandaiexperiments/__init__.py
--rw-rw-rw-   0        0        0     2039 2024-05-13 18:39:31.000000 ishandaiexperiments-0.0.3/ishandaiexperiments/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:43:45.628758 ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/
--rw-rw-rw-   0        0        0      613 2024-05-13 18:43:45.000000 ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-05-13 18:43:45.000000 ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:43:45.000000 ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:43:45.000000 ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 18:43:45.635353 ishandaiexperiments-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-05-13 18:43:14.000000 ishandaiexperiments-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:46:53.564439 ishandaiexperiments-0.0.4/
+-rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 ishandaiexperiments-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 ishandaiexperiments-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 ishandaiexperiments-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      613 2024-05-13 18:46:53.563083 ishandaiexperiments-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-05-13 17:37:56.000000 ishandaiexperiments-0.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 18:46:53.523011 ishandaiexperiments-0.0.4/ishandaiexperiments/
+-rw-rw-rw-   0        0        0       75 2024-05-13 18:40:39.000000 ishandaiexperiments-0.0.4/ishandaiexperiments/__init__.py
+-rw-rw-rw-   0        0        0     2039 2024-05-13 18:39:31.000000 ishandaiexperiments-0.0.4/ishandaiexperiments/main.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:46:53.559724 ishandaiexperiments-0.0.4/ishandaiexperiments.egg-info/
+-rw-rw-rw-   0        0        0      613 2024-05-13 18:46:53.000000 ishandaiexperiments-0.0.4/ishandaiexperiments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-05-13 18:46:53.000000 ishandaiexperiments-0.0.4/ishandaiexperiments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:46:53.000000 ishandaiexperiments-0.0.4/ishandaiexperiments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:46:53.000000 ishandaiexperiments-0.0.4/ishandaiexperiments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 18:46:53.565312 ishandaiexperiments-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      715 2024-05-13 18:46:45.000000 ishandaiexperiments-0.0.4/setup.py
```

### Comparing `ishandaiexperiments-0.0.3/LICENSE.txt` & `ishandaiexperiments-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ishandaiexperiments-0.0.3/PKG-INFO` & `ishandaiexperiments-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ishandaiexperiments
-Version: 0.0.3
+Version: 0.0.4
 Summary: dai experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ishandaiexperiments-0.0.3/ishandaiexperiments/main.py` & `ishandaiexperiments-0.0.4/ishandaiexperiments/main.py`

 * *Files identical despite different names*

### Comparing `ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/PKG-INFO` & `ishandaiexperiments-0.0.4/ishandaiexperiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ishandaiexperiments
-Version: 0.0.3
+Version: 0.0.4
 Summary: dai experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ishandaiexperiments-0.0.3/setup.py` & `ishandaiexperiments-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ishandaiexperiments',
-  version='0.0.3',
+  version='0.0.4',
   description='dai experiments',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='S Ishan',
   author_email='is9678@srmist.edu.in',
   license='MIT', 
   classifiers=classifiers,
   keywords='dai', 
-  packages=find_packages('exp'),
+  packages=find_packages(''),
   include_package_data= True,
   install_requires=[''] 
 )
```

