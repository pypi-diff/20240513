# Comparing `tmp/liteium-1.0.2.tar.gz` & `tmp/liteium-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteium-1.0.2.tar", last modified: Sat May 11 18:50:40 2024, max compression
+gzip compressed data, was "liteium-1.0.3.tar", last modified: Mon May 13 02:12:19 2024, max compression
```

## Comparing `liteium-1.0.2.tar` & `liteium-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 18:50:40.840931 liteium-1.0.2/
--rw-rw-rw-   0        0        0      853 2024-05-11 18:50:40.838931 liteium-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      457 2024-05-11 04:46:56.000000 liteium-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 18:50:40.783930 liteium-1.0.2/liteium/
--rw-rw-rw-   0        0        0       19 2024-05-11 18:49:55.000000 liteium-1.0.2/liteium/__init__.py
--rw-rw-rw-   0        0        0     8344 2024-05-11 16:47:38.000000 liteium-1.0.2/liteium/main.py
-drwxrwxrwx   0        0        0        0 2024-05-11 18:50:40.836934 liteium-1.0.2/liteium.egg-info/
--rw-rw-rw-   0        0        0      853 2024-05-11 18:50:40.000000 liteium-1.0.2/liteium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-11 18:50:40.000000 liteium-1.0.2/liteium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 18:50:40.000000 liteium-1.0.2/liteium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-11 18:50:40.000000 liteium-1.0.2/liteium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-11 18:50:40.000000 liteium-1.0.2/liteium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 18:50:40.840931 liteium-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      632 2024-05-11 18:50:15.000000 liteium-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:12:19.878422 liteium-1.0.3/
+-rw-rw-rw-   0        0        0      853 2024-05-13 02:12:19.877424 liteium-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2024-05-11 04:46:56.000000 liteium-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 02:12:19.843451 liteium-1.0.3/liteium/
+-rw-rw-rw-   0        0        0       19 2024-05-11 18:49:55.000000 liteium-1.0.3/liteium/__init__.py
+-rw-rw-rw-   0        0        0    10102 2024-05-13 02:09:51.000000 liteium-1.0.3/liteium/main.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:12:19.875426 liteium-1.0.3/liteium.egg-info/
+-rw-rw-rw-   0        0        0      853 2024-05-13 02:12:19.000000 liteium-1.0.3/liteium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-13 02:12:19.000000 liteium-1.0.3/liteium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:12:19.000000 liteium-1.0.3/liteium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 02:12:19.000000 liteium-1.0.3/liteium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 02:12:19.000000 liteium-1.0.3/liteium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:12:19.878422 liteium-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      632 2024-05-13 02:11:49.000000 liteium-1.0.3/setup.py
```

### Comparing `liteium-1.0.2/PKG-INFO` & `liteium-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteium
-Version: 1.0.2
+Version: 1.0.3
 Summary: Description of your package
 Home-page: https://github.com/XredaX/liteium
 Author: El Bettioui Reda
 Author-email: redaelbettioui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liteium-1.0.2/liteium.egg-info/PKG-INFO` & `liteium-1.0.3/liteium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteium
-Version: 1.0.2
+Version: 1.0.3
 Summary: Description of your package
 Home-page: https://github.com/XredaX/liteium
 Author: El Bettioui Reda
 Author-email: redaelbettioui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liteium-1.0.2/setup.py` & `liteium-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='liteium',
-    version='1.0.2',
+    version='1.0.3',
     description='Description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='El Bettioui Reda',
     author_email='redaelbettioui@gmail.com',
     url='https://github.com/XredaX/liteium',
     packages=find_packages(),
```

