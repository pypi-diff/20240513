# Comparing `tmp/codescout-0.1.tar.gz` & `tmp/codescout-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codescout-0.1.tar", last modified: Mon May 13 16:33:48 2024, max compression
+gzip compressed data, was "codescout-0.1.1.tar", last modified: Mon May 13 16:39:28 2024, max compression
```

## Comparing `codescout-0.1.tar` & `codescout-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:33:48.658897 codescout-0.1/
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)    11357 2024-05-13 14:57:56.000000 codescout-0.1/LICENSE
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      755 2024-05-13 16:33:48.658667 codescout-0.1/PKG-INFO
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)     3751 2024-05-13 14:57:56.000000 codescout-0.1/README.md
-drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:33:48.658164 codescout-0.1/codescout.egg-info/
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      755 2024-05-13 16:33:48.657294 codescout-0.1/codescout.egg-info/PKG-INFO
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      208 2024-05-13 16:33:48.657627 codescout-0.1/codescout.egg-info/SOURCES.txt
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        1 2024-05-13 16:33:48.657806 codescout-0.1/codescout.egg-info/dependency_links.txt
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       11 2024-05-13 16:33:48.657989 codescout-0.1/codescout.egg-info/requires.txt
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        6 2024-05-13 16:33:48.658288 codescout-0.1/codescout.egg-info/top_level.txt
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       38 2024-05-13 16:33:48.658944 codescout-0.1/setup.cfg
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)     1013 2024-05-13 16:27:12.000000 codescout-0.1/setup.py
-drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:33:48.658443 codescout-0.1/tests/
--rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 15:27:47.000000 codescout-0.1/tests/__init__.py
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:39:28.306799 codescout-0.1.1/
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)    11357 2024-05-13 14:57:56.000000 codescout-0.1.1/LICENSE
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      757 2024-05-13 16:39:28.306514 codescout-0.1.1/PKG-INFO
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)     3751 2024-05-13 14:57:56.000000 codescout-0.1.1/README.md
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:39:28.306094 codescout-0.1.1/codescout.egg-info/
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      757 2024-05-13 16:39:28.304814 codescout-0.1.1/codescout.egg-info/PKG-INFO
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)      208 2024-05-13 16:39:28.305142 codescout-0.1.1/codescout.egg-info/SOURCES.txt
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        1 2024-05-13 16:39:28.305338 codescout-0.1.1/codescout.egg-info/dependency_links.txt
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       14 2024-05-13 16:39:28.305661 codescout-0.1.1/codescout.egg-info/requires.txt
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        6 2024-05-13 16:39:28.306128 codescout-0.1.1/codescout.egg-info/top_level.txt
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)       38 2024-05-13 16:39:28.306942 codescout-0.1.1/setup.cfg
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)     1018 2024-05-13 16:39:07.000000 codescout-0.1.1/setup.py
+drwxr-xr-x   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 16:39:28.306284 codescout-0.1.1/tests/
+-rw-r--r--   0 vfo001   (67203) eccc_rpnenv (66080)        0 2024-05-13 15:27:47.000000 codescout-0.1.1/tests/__init__.py
```

### Comparing `codescout-0.1/LICENSE` & `codescout-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codescout-0.1/PKG-INFO` & `codescout-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codescout
-Version: 0.1
+Version: 0.1.1
 Summary: Permet de creer des codes scouts
 Home-page: https://github.com/vinfort/codescout
 Author: Vincent Fortin
 Author-email: vincent.fortin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `codescout-0.1/README.md` & `codescout-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `codescout-0.1/codescout.egg-info/PKG-INFO` & `codescout-0.1.1/codescout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codescout
-Version: 0.1
+Version: 0.1.1
 Summary: Permet de creer des codes scouts
 Home-page: https://github.com/vinfort/codescout
 Author: Vincent Fortin
 Author-email: vincent.fortin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `codescout-0.1/setup.py` & `codescout-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='codescout',
-    version='0.1',
+    version='0.1.1',
     author='Vincent Fortin',
     author_email='vincent.fortin@gmail.com',
     description='Permet de creer des codes scouts',
     long_description="Cette première version de la librairie codescout permet d'encoder des messages à l'aide du code soleil et du code musical. Développé en préparation du Camporee de la Montérégie 2024. (C) Vincent Fortin 2024. [vincent.fortin@gmail.com](mailto:vincent.fortin@gmail.com)",
     long_description_content_type='text/markdown',
     url='https://github.com/vinfort/codescout',
     packages=find_packages(),  # Automatically find all packages in the project
@@ -14,10 +14,10 @@
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
     ],
     python_requires='>=3.6',
     install_requires=[
         # List of dependencies required by your package
-        'PIL>=5.1.1',
+        'pillow>=5.1.1',
     ],
 )
```

