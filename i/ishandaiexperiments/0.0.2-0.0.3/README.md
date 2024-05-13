# Comparing `tmp/ishandaiexperiments-0.0.2.tar.gz` & `tmp/ishandaiexperiments-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ishandaiexperiments-0.0.2.tar", last modified: Mon May 13 18:32:51 2024, max compression
+gzip compressed data, was "ishandaiexperiments-0.0.3.tar", last modified: Mon May 13 18:43:45 2024, max compression
```

## Comparing `ishandaiexperiments-0.0.2.tar` & `ishandaiexperiments-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 18:32:51.207000 ishandaiexperiments-0.0.2/
--rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 ishandaiexperiments-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 ishandaiexperiments-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 ishandaiexperiments-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      613 2024-05-13 18:32:51.205975 ishandaiexperiments-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-05-13 17:37:56.000000 ishandaiexperiments-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 18:32:51.185403 ishandaiexperiments-0.0.2/exp/
--rw-rw-rw-   0        0        0     2074 2024-05-13 17:36:44.000000 ishandaiexperiments-0.0.2/exp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:32:51.204082 ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/
--rw-rw-rw-   0        0        0      613 2024-05-13 18:32:51.000000 ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-05-13 18:32:51.000000 ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:32:51.000000 ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:32:51.000000 ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 18:32:51.207000 ishandaiexperiments-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-05-13 18:32:21.000000 ishandaiexperiments-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:43:45.634549 ishandaiexperiments-0.0.3/
+-rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 ishandaiexperiments-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 ishandaiexperiments-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 ishandaiexperiments-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      613 2024-05-13 18:43:45.633549 ishandaiexperiments-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-05-13 17:37:56.000000 ishandaiexperiments-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 18:43:45.579533 ishandaiexperiments-0.0.3/ishandaiexperiments/
+-rw-rw-rw-   0        0        0       75 2024-05-13 18:40:39.000000 ishandaiexperiments-0.0.3/ishandaiexperiments/__init__.py
+-rw-rw-rw-   0        0        0     2039 2024-05-13 18:39:31.000000 ishandaiexperiments-0.0.3/ishandaiexperiments/main.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:43:45.628758 ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/
+-rw-rw-rw-   0        0        0      613 2024-05-13 18:43:45.000000 ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-05-13 18:43:45.000000 ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:43:45.000000 ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:43:45.000000 ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 18:43:45.635353 ishandaiexperiments-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-05-13 18:43:14.000000 ishandaiexperiments-0.0.3/setup.py
```

### Comparing `ishandaiexperiments-0.0.2/LICENSE.txt` & `ishandaiexperiments-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ishandaiexperiments-0.0.2/PKG-INFO` & `ishandaiexperiments-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ishandaiexperiments
-Version: 0.0.2
+Version: 0.0.3
 Summary: dai experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ishandaiexperiments-0.0.2/exp/__init__.py` & `ishandaiexperiments-0.0.3/ishandaiexperiments/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,10 +50,8 @@
             reader = easyocr.Reader(['en'])
             result = reader.readtext(cropped_image)
             result
 
             result[0][1]
             """
     
-    print(code)
-
-print(number_plate_detection())
+    print(code)
```

### Comparing `ishandaiexperiments-0.0.2/ishandaiexperiments.egg-info/PKG-INFO` & `ishandaiexperiments-0.0.3/ishandaiexperiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ishandaiexperiments
-Version: 0.0.2
+Version: 0.0.3
 Summary: dai experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ishandaiexperiments-0.0.2/setup.py` & `ishandaiexperiments-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ishandaiexperiments',
-  version='0.0.2',
+  version='0.0.3',
   description='dai experiments',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='S Ishan',
   author_email='is9678@srmist.edu.in',
   license='MIT', 
   classifiers=classifiers,
```

