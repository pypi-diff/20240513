# Comparing `tmp/lgjsfinance-0.0.2.tar.gz` & `tmp/lgjsfinance-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lgjsfinance-0.0.2.tar", last modified: Mon May 13 07:48:22 2024, max compression
+gzip compressed data, was "lgjsfinance-0.0.3.tar", last modified: Mon May 13 07:54:51 2024, max compression
```

## Comparing `lgjsfinance-0.0.2.tar` & `lgjsfinance-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 07:48:22.884774 lgjsfinance-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-05-13 07:32:41.000000 lgjsfinance-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      759 2024-05-13 07:48:22.882772 lgjsfinance-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-05-13 07:47:19.000000 lgjsfinance-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 07:48:22.812351 lgjsfinance-0.0.2/lgjsfinance/
--rw-rw-rw-   0        0        0      101 2024-05-13 07:48:09.000000 lgjsfinance-0.0.2/lgjsfinance/__init__.py
--rw-rw-rw-   0        0        0     1112 2024-05-13 07:47:35.000000 lgjsfinance-0.0.2/lgjsfinance/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:48:22.881759 lgjsfinance-0.0.2/lgjsfinance.egg-info/
--rw-rw-rw-   0        0        0      759 2024-05-13 07:48:22.000000 lgjsfinance-0.0.2/lgjsfinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2024-05-13 07:48:22.000000 lgjsfinance-0.0.2/lgjsfinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 07:48:22.000000 lgjsfinance-0.0.2/lgjsfinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-13 07:48:22.000000 lgjsfinance-0.0.2/lgjsfinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-13 07:48:22.000000 lgjsfinance-0.0.2/lgjsfinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 07:48:22.885774 lgjsfinance-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      931 2024-05-13 07:47:46.000000 lgjsfinance-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:54:51.129908 lgjsfinance-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-05-13 07:32:41.000000 lgjsfinance-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      759 2024-05-13 07:54:51.124909 lgjsfinance-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-05-13 07:47:19.000000 lgjsfinance-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 07:54:51.063698 lgjsfinance-0.0.3/lgjsfinance/
+-rw-rw-rw-   0        0        0     1112 2024-05-13 07:47:35.000000 lgjsfinance-0.0.3/lgjsfinance/DataRecover.py
+-rw-rw-rw-   0        0        0      101 2024-05-13 07:54:23.000000 lgjsfinance-0.0.3/lgjsfinance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:54:51.122909 lgjsfinance-0.0.3/lgjsfinance.egg-info/
+-rw-rw-rw-   0        0        0      759 2024-05-13 07:54:50.000000 lgjsfinance-0.0.3/lgjsfinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-13 07:54:50.000000 lgjsfinance-0.0.3/lgjsfinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 07:54:50.000000 lgjsfinance-0.0.3/lgjsfinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-13 07:54:50.000000 lgjsfinance-0.0.3/lgjsfinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-13 07:54:50.000000 lgjsfinance-0.0.3/lgjsfinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 07:54:51.129908 lgjsfinance-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      931 2024-05-13 07:54:20.000000 lgjsfinance-0.0.3/setup.py
```

### Comparing `lgjsfinance-0.0.2/LICENSE` & `lgjsfinance-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lgjsfinance-0.0.2/PKG-INFO` & `lgjsfinance-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lgjsfinance
-Version: 0.0.2
+Version: 0.0.3
 Summary: LGJS Finance
 Home-page: https://liamgenjs.vercel.app
 Author: liamgen.js
 Author-email: liamgen.js@proton.me
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lgjsfinance-0.0.2/lgjsfinance/main.py` & `lgjsfinance-0.0.3/lgjsfinance/DataRecover.py`

 * *Files identical despite different names*

### Comparing `lgjsfinance-0.0.2/lgjsfinance.egg-info/PKG-INFO` & `lgjsfinance-0.0.3/lgjsfinance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lgjsfinance
-Version: 0.0.2
+Version: 0.0.3
 Summary: LGJS Finance
 Home-page: https://liamgenjs.vercel.app
 Author: liamgen.js
 Author-email: liamgen.js@proton.me
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lgjsfinance-0.0.2/setup.py` & `lgjsfinance-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='lgjsfinance',
-    version='0.0.2',    
+    version='0.0.3',    
     description='LGJS Finance',
     url='https://liamgenjs.vercel.app',
     author='liamgen.js',
     author_email='liamgen.js@proton.me',
     license='BSD 2-clause',
     packages=['lgjsfinance'],
     install_requires=['yfinance>=0.2.38',
```

