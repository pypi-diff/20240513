# Comparing `tmp/bing_create-0.0.2.tar.gz` & `tmp/bing_create-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bing_create-0.0.2.tar", last modified: Mon May 13 15:55:20 2024, max compression
+gzip compressed data, was "bing_create-0.0.3.tar", last modified: Mon May 13 16:04:27 2024, max compression
```

## Comparing `bing_create-0.0.2.tar` & `bing_create-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 15:55:20.977875 bing_create-0.0.2/
--rw-rw-rw-   0        0        0     4582 2024-05-13 15:55:20.977875 bing_create-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3417 2024-05-13 15:49:55.000000 bing_create-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 15:55:20.969225 bing_create-0.0.2/bing_create/
--rw-rw-rw-   0        0        0        0 2024-05-13 08:40:47.000000 bing_create-0.0.2/bing_create/__init__.py
--rw-rw-rw-   0        0        0    10901 2024-05-13 15:42:48.000000 bing_create-0.0.2/bing_create/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:55:20.976864 bing_create-0.0.2/bing_create.egg-info/
--rw-rw-rw-   0        0        0     4582 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 15:55:20.978867 bing_create-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1456 2024-05-13 15:54:13.000000 bing_create-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:04:27.603973 bing_create-0.0.3/
+-rw-rw-rw-   0        0        0     4582 2024-05-13 16:04:27.602898 bing_create-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3417 2024-05-13 15:49:55.000000 bing_create-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 16:04:27.585155 bing_create-0.0.3/bing_create/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:40:47.000000 bing_create-0.0.3/bing_create/__init__.py
+-rw-rw-rw-   0        0        0    10901 2024-05-13 15:42:48.000000 bing_create-0.0.3/bing_create/main.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:04:27.602393 bing_create-0.0.3/bing_create.egg-info/
+-rw-rw-rw-   0        0        0     4582 2024-05-13 16:04:27.000000 bing_create-0.0.3/bing_create.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-13 16:04:27.000000 bing_create-0.0.3/bing_create.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 16:04:27.000000 bing_create-0.0.3/bing_create.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-13 16:04:27.000000 bing_create-0.0.3/bing_create.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-05-13 16:04:27.000000 bing_create-0.0.3/bing_create.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-13 16:04:27.000000 bing_create-0.0.3/bing_create.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 16:04:27.603973 bing_create-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1512 2024-05-13 16:04:23.000000 bing_create-0.0.3/setup.py
```

### Comparing `bing_create-0.0.2/PKG-INFO` & `bing_create-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bing_create
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple lightweight AI Image Generator from text description using Bing Image Creator (DALL-E 3)
 Home-page: https://github.com/Waenara/bing-create
 Author: Waenara
 Author-email: WaenaraCat@gmail.com
 Project-URL: Support, https://github.com/Waenara/bing-create/issues
 Keywords: ai dall-e image bing api generator bing_create image-generator ig ic
 Classifier: Intended Audience :: Developers
```

### Comparing `bing_create-0.0.2/README.md` & `bing_create-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bing_create-0.0.2/bing_create/main.py` & `bing_create-0.0.3/bing_create/main.py`

 * *Files identical despite different names*

### Comparing `bing_create-0.0.2/bing_create.egg-info/PKG-INFO` & `bing_create-0.0.3/bing_create.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bing-create
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple lightweight AI Image Generator from text description using Bing Image Creator (DALL-E 3)
 Home-page: https://github.com/Waenara/bing-create
 Author: Waenara
 Author-email: WaenaraCat@gmail.com
 Project-URL: Support, https://github.com/Waenara/bing-create/issues
 Keywords: ai dall-e image bing api generator bing_create image-generator ig ic
 Classifier: Intended Audience :: Developers
```

### Comparing `bing_create-0.0.2/setup.py` & `bing_create-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from setuptools import setup, find_packages
 setup(
     name='bing_create',
-    version='0.0.2',
+    version='0.0.3',
     author='Waenara',
     author_email='WaenaraCat@gmail.com',
     description='A simple lightweight AI Image Generator from text description using Bing Image Creator (DALL-E 3)',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Waenara/bing-create',
     packages=find_packages(),
-    install_requires=open('requirements.txt').readlines(),
+    install_requires=[
+        'setuptools~=68.2.0',
+        'aiofiles~=23.2.1',
+        'httpx~=0.27.0'
+    ],
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
@@ -28,9 +32,9 @@
         'Support': 'https://github.com/Waenara/bing-create/issues'
     },
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
             'bing_create = bing_create.main:main',
         ],
-    },
+    }
 )
```

