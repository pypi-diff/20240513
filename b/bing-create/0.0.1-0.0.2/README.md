# Comparing `tmp/bing_create-0.0.1.tar.gz` & `tmp/bing_create-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bing_create-0.0.1.tar", last modified: Mon May 13 15:48:31 2024, max compression
+gzip compressed data, was "bing_create-0.0.2.tar", last modified: Mon May 13 15:55:20 2024, max compression
```

## Comparing `bing_create-0.0.1.tar` & `bing_create-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 15:48:31.614920 bing_create-0.0.1/
--rw-rw-rw-   0        0        0     4540 2024-05-13 15:48:31.613918 bing_create-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3375 2024-05-13 15:37:51.000000 bing_create-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 15:48:31.585082 bing_create-0.0.1/bing_create/
--rw-rw-rw-   0        0        0        0 2024-05-13 08:40:47.000000 bing_create-0.0.1/bing_create/__init__.py
--rw-rw-rw-   0        0        0    10901 2024-05-13 15:42:48.000000 bing_create-0.0.1/bing_create/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:48:31.612410 bing_create-0.0.1/bing_create.egg-info/
--rw-rw-rw-   0        0        0     4540 2024-05-13 15:48:31.000000 bing_create-0.0.1/bing_create.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-13 15:48:31.000000 bing_create-0.0.1/bing_create.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 15:48:31.000000 bing_create-0.0.1/bing_create.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-13 15:48:31.000000 bing_create-0.0.1/bing_create.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-05-13 15:48:31.000000 bing_create-0.0.1/bing_create.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-13 15:48:31.000000 bing_create-0.0.1/bing_create.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 15:48:31.615920 bing_create-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1456 2024-05-13 15:33:39.000000 bing_create-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:55:20.977875 bing_create-0.0.2/
+-rw-rw-rw-   0        0        0     4582 2024-05-13 15:55:20.977875 bing_create-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3417 2024-05-13 15:49:55.000000 bing_create-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 15:55:20.969225 bing_create-0.0.2/bing_create/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:40:47.000000 bing_create-0.0.2/bing_create/__init__.py
+-rw-rw-rw-   0        0        0    10901 2024-05-13 15:42:48.000000 bing_create-0.0.2/bing_create/main.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:55:20.976864 bing_create-0.0.2/bing_create.egg-info/
+-rw-rw-rw-   0        0        0     4582 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-13 15:55:20.000000 bing_create-0.0.2/bing_create.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 15:55:20.978867 bing_create-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1456 2024-05-13 15:54:13.000000 bing_create-0.0.2/setup.py
```

### Comparing `bing_create-0.0.1/PKG-INFO` & `bing_create-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bing_create
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple lightweight AI Image Generator from text description using Bing Image Creator (DALL-E 3)
 Home-page: https://github.com/Waenara/bing-create
 Author: Waenara
 Author-email: WaenaraCat@gmail.com
 Project-URL: Support, https://github.com/Waenara/bing-create/issues
 Keywords: ai dall-e image bing api generator bing_create image-generator ig ic
 Classifier: Intended Audience :: Developers
@@ -40,15 +40,15 @@
 ## Installation
 To install the package you can use pip:
 ```bash
 pip install bing-create
 ```
 or you can clone the repository and install it manually:
 ```bash
-git clone 
+git clone https://github.com/Waenara/bing-create.git
 cd bing_create
 pip install .
 ```
 ## Usage
 ### Getting cookies
 After installing the package as described above you will need to get your **_U** and **SRCHHPGUSR** cookies from [Bing](https://bing.com). You can do this by logging in to [Bing](https://bing.com), opening the developer tools (F12) and going to the console tab. Then you can run the following code:
 ```javascript
```

### Comparing `bing_create-0.0.1/README.md` & `bing_create-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ## Installation
 To install the package you can use pip:
 ```bash
 pip install bing-create
 ```
 or you can clone the repository and install it manually:
 ```bash
-git clone 
+git clone https://github.com/Waenara/bing-create.git
 cd bing_create
 pip install .
 ```
 ## Usage
 ### Getting cookies
 After installing the package as described above you will need to get your **_U** and **SRCHHPGUSR** cookies from [Bing](https://bing.com). You can do this by logging in to [Bing](https://bing.com), opening the developer tools (F12) and going to the console tab. Then you can run the following code:
 ```javascript
```

### Comparing `bing_create-0.0.1/bing_create/main.py` & `bing_create-0.0.2/bing_create/main.py`

 * *Files identical despite different names*

### Comparing `bing_create-0.0.1/bing_create.egg-info/PKG-INFO` & `bing_create-0.0.2/bing_create.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bing-create
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple lightweight AI Image Generator from text description using Bing Image Creator (DALL-E 3)
 Home-page: https://github.com/Waenara/bing-create
 Author: Waenara
 Author-email: WaenaraCat@gmail.com
 Project-URL: Support, https://github.com/Waenara/bing-create/issues
 Keywords: ai dall-e image bing api generator bing_create image-generator ig ic
 Classifier: Intended Audience :: Developers
@@ -40,15 +40,15 @@
 ## Installation
 To install the package you can use pip:
 ```bash
 pip install bing-create
 ```
 or you can clone the repository and install it manually:
 ```bash
-git clone 
+git clone https://github.com/Waenara/bing-create.git
 cd bing_create
 pip install .
 ```
 ## Usage
 ### Getting cookies
 After installing the package as described above you will need to get your **_U** and **SRCHHPGUSR** cookies from [Bing](https://bing.com). You can do this by logging in to [Bing](https://bing.com), opening the developer tools (F12) and going to the console tab. Then you can run the following code:
 ```javascript
```

### Comparing `bing_create-0.0.1/setup.py` & `bing_create-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='bing_create',
-    version='0.0.1',
+    version='0.0.2',
     author='Waenara',
     author_email='WaenaraCat@gmail.com',
     description='A simple lightweight AI Image Generator from text description using Bing Image Creator (DALL-E 3)',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Waenara/bing-create',
     packages=find_packages(),
```

