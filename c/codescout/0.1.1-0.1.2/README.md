# Comparing `tmp/codescout-0.1.1.tar.gz` & `tmp/codescout-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codescout-0.1.1.tar", last modified: Mon May 13 16:39:28 2024, max compression
+gzip compressed data, was "codescout-0.1.2.tar", last modified: Mon May 13 16:55:18 2024, max compression
```

## Comparing `codescout-0.1.1.tar` & `codescout-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:39:28.306799 codescout-0.1.1/
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)    11357 2024-05-13 14:57:56.000000 codescout-0.1.1/LICENSE
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      757 2024-05-13 16:39:28.306514 codescout-0.1.1/PKG-INFO
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)     3751 2024-05-13 14:57:56.000000 codescout-0.1.1/README.md
-drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:39:28.306094 codescout-0.1.1/codescout.egg-info/
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      757 2024-05-13 16:39:28.304814 codescout-0.1.1/codescout.egg-info/PKG-INFO
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      208 2024-05-13 16:39:28.305142 codescout-0.1.1/codescout.egg-info/SOURCES.txt
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        1 2024-05-13 16:39:28.305338 codescout-0.1.1/codescout.egg-info/dependency_links.txt
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       14 2024-05-13 16:39:28.305661 codescout-0.1.1/codescout.egg-info/requires.txt
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        6 2024-05-13 16:39:28.306128 codescout-0.1.1/codescout.egg-info/top_level.txt
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       38 2024-05-13 16:39:28.306942 codescout-0.1.1/setup.cfg
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)     1018 2024-05-13 16:39:07.000000 codescout-0.1.1/setup.py
-drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:39:28.306284 codescout-0.1.1/tests/
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 15:27:47.000000 codescout-0.1.1/tests/__init__.py
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:55:18.497870 codescout-0.1.2/
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)    11357 2024-05-13 14:57:56.000000 codescout-0.1.2/LICENSE
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       27 2024-05-13 16:55:10.000000 codescout-0.1.2/MANIFEST.in
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      757 2024-05-13 16:55:18.497629 codescout-0.1.2/PKG-INFO
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)     3751 2024-05-13 14:57:56.000000 codescout-0.1.2/README.md
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:55:18.495656 codescout-0.1.2/codescout.egg-info/
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      757 2024-05-13 16:55:18.494881 codescout-0.1.2/codescout.egg-info/PKG-INFO
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      273 2024-05-13 16:55:18.495086 codescout-0.1.2/codescout.egg-info/SOURCES.txt
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        1 2024-05-13 16:55:18.495288 codescout-0.1.2/codescout.egg-info/dependency_links.txt
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       14 2024-05-13 16:55:18.495490 codescout-0.1.2/codescout.egg-info/requires.txt
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        1 2024-05-13 16:55:18.495695 codescout-0.1.2/codescout.egg-info/top_level.txt
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       38 2024-05-13 16:55:18.497920 codescout-0.1.2/setup.cfg
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)     1043 2024-05-13 16:51:31.000000 codescout-0.1.2/setup.py
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:55:18.492872 codescout-0.1.2/src/
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:55:18.496489 codescout-0.1.2/src/codescout/
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 15:21:39.000000 codescout-0.1.2/src/codescout/__init__.py
+-rwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)    20947 2024-05-13 15:13:31.000000 codescout-0.1.2/src/codescout/codescout.py
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:55:18.497135 codescout-0.1.2/tests/
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 15:27:47.000000 codescout-0.1.2/tests/__init__.py
```

### Comparing `codescout-0.1.1/LICENSE` & `codescout-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codescout-0.1.1/PKG-INFO` & `codescout-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codescout
-Version: 0.1.1
+Version: 0.1.2
 Summary: Permet de creer des codes scouts
 Home-page: https://github.com/vinfort/codescout
 Author: Vincent Fortin
 Author-email: vincent.fortin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `codescout-0.1.1/README.md` & `codescout-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `codescout-0.1.1/codescout.egg-info/PKG-INFO` & `codescout-0.1.2/codescout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codescout
-Version: 0.1.1
+Version: 0.1.2
 Summary: Permet de creer des codes scouts
 Home-page: https://github.com/vinfort/codescout
 Author: Vincent Fortin
 Author-email: vincent.fortin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `codescout-0.1.1/setup.py` & `codescout-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='codescout',
-    version='0.1.1',
+    version='0.1.2',
     author='Vincent Fortin',
     author_email='vincent.fortin@gmail.com',
     description='Permet de creer des codes scouts',
     long_description="Cette première version de la librairie codescout permet d'encoder des messages à l'aide du code soleil et du code musical. Développé en préparation du Camporee de la Montérégie 2024. (C) Vincent Fortin 2024. [vincent.fortin@gmail.com](mailto:vincent.fortin@gmail.com)",
     long_description_content_type='text/markdown',
     url='https://github.com/vinfort/codescout',
-    packages=find_packages(),  # Automatically find all packages in the project
+    packages=find_packages(include=['src/codescout']),  # Automatically find all packages in the project
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
     ],
     python_requires='>=3.6',
     install_requires=[
```

