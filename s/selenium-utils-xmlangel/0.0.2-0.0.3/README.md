# Comparing `tmp/selenium_utils_xmlangel-0.0.2.tar.gz` & `tmp/selenium_utils_xmlangel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_utils_xmlangel-0.0.2.tar", last modified: Mon May 13 14:36:29 2024, max compression
+gzip compressed data, was "selenium_utils_xmlangel-0.0.3.tar", last modified: Mon May 13 14:42:22 2024, max compression
```

## Comparing `selenium_utils_xmlangel-0.0.2.tar` & `selenium_utils_xmlangel-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dicky      (501) staff       (20)        0 2024-05-13 14:36:29.471184 selenium_utils_xmlangel-0.0.2/
--rw-r--r--   0 dicky      (501) staff       (20)      567 2024-05-13 14:36:29.470998 selenium_utils_xmlangel-0.0.2/PKG-INFO
--rw-r--r--   0 dicky      (501) staff       (20)       46 2024-05-13 13:33:22.000000 selenium_utils_xmlangel-0.0.2/README.md
-drwxr-xr-x   0 dicky      (501) staff       (20)        0 2024-05-13 14:36:29.469971 selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel/
--rw-r--r--   0 dicky      (501) staff       (20)       21 2024-05-13 14:33:39.000000 selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel/__init__.py
--rw-r--r--   0 dicky      (501) staff       (20)      634 2024-05-13 14:33:42.000000 selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel/compare-image.py
-drwxr-xr-x   0 dicky      (501) staff       (20)        0 2024-05-13 14:36:29.470823 selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel.egg-info/
--rw-r--r--   0 dicky      (501) staff       (20)      567 2024-05-13 14:36:29.000000 selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel.egg-info/PKG-INFO
--rw-r--r--   0 dicky      (501) staff       (20)      375 2024-05-13 14:36:29.000000 selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel.egg-info/SOURCES.txt
--rw-r--r--   0 dicky      (501) staff       (20)        1 2024-05-13 14:36:29.000000 selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel.egg-info/dependency_links.txt
--rw-r--r--   0 dicky      (501) staff       (20)        1 2024-05-13 14:36:29.000000 selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel.egg-info/not-zip-safe
--rw-r--r--   0 dicky      (501) staff       (20)       27 2024-05-13 14:36:29.000000 selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel.egg-info/requires.txt
--rw-r--r--   0 dicky      (501) staff       (20)       24 2024-05-13 14:36:29.000000 selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel.egg-info/top_level.txt
--rw-r--r--   0 dicky      (501) staff       (20)       38 2024-05-13 14:36:29.471227 selenium_utils_xmlangel-0.0.2/setup.cfg
--rw-r--r--   0 dicky      (501) staff       (20)      756 2024-05-13 14:33:25.000000 selenium_utils_xmlangel-0.0.2/setup.py
+drwxr-xr-x   0 dicky      (501) staff       (20)        0 2024-05-13 14:42:22.825349 selenium_utils_xmlangel-0.0.3/
+-rw-r--r--   0 dicky      (501) staff       (20)      567 2024-05-13 14:42:22.825168 selenium_utils_xmlangel-0.0.3/PKG-INFO
+-rw-r--r--   0 dicky      (501) staff       (20)       46 2024-05-13 13:33:22.000000 selenium_utils_xmlangel-0.0.3/README.md
+drwxr-xr-x   0 dicky      (501) staff       (20)        0 2024-05-13 14:42:22.824129 selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel/
+-rw-r--r--   0 dicky      (501) staff       (20)       21 2024-05-13 14:41:33.000000 selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel/__init__.py
+-rw-r--r--   0 dicky      (501) staff       (20)      634 2024-05-13 14:40:41.000000 selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel/compare_image.py
+drwxr-xr-x   0 dicky      (501) staff       (20)        0 2024-05-13 14:42:22.824985 selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel.egg-info/
+-rw-r--r--   0 dicky      (501) staff       (20)      567 2024-05-13 14:42:22.000000 selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel.egg-info/PKG-INFO
+-rw-r--r--   0 dicky      (501) staff       (20)      375 2024-05-13 14:42:22.000000 selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel.egg-info/SOURCES.txt
+-rw-r--r--   0 dicky      (501) staff       (20)        1 2024-05-13 14:42:22.000000 selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel.egg-info/dependency_links.txt
+-rw-r--r--   0 dicky      (501) staff       (20)        1 2024-05-13 14:36:29.000000 selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel.egg-info/not-zip-safe
+-rw-r--r--   0 dicky      (501) staff       (20)       27 2024-05-13 14:42:22.000000 selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel.egg-info/requires.txt
+-rw-r--r--   0 dicky      (501) staff       (20)       24 2024-05-13 14:42:22.000000 selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel.egg-info/top_level.txt
+-rw-r--r--   0 dicky      (501) staff       (20)       38 2024-05-13 14:42:22.825399 selenium_utils_xmlangel-0.0.3/setup.cfg
+-rw-r--r--   0 dicky      (501) staff       (20)      756 2024-05-13 14:41:43.000000 selenium_utils_xmlangel-0.0.3/setup.py
```

### Comparing `selenium_utils_xmlangel-0.0.2/PKG-INFO` & `selenium_utils_xmlangel-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_utils_xmlangel
-Version: 0.0.2
+Version: 0.0.3
 Summary: PYPI selenium-utils package creation written by xmlangel
 Home-page: https://github.com/xmlangel/selenium-utils-xmlangel
 Author: xmlangel
 Author-email: kwangmyung.kim@gmail.com
 Keywords: selenium,xmlangel,utils
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel/compare-image.py` & `selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel/compare_image.py`

 * *Files identical despite different names*

### Comparing `selenium_utils_xmlangel-0.0.2/selenium_utils_xmlangel.egg-info/PKG-INFO` & `selenium_utils_xmlangel-0.0.3/selenium_utils_xmlangel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_utils_xmlangel
-Version: 0.0.2
+Version: 0.0.3
 Summary: PYPI selenium-utils package creation written by xmlangel
 Home-page: https://github.com/xmlangel/selenium-utils-xmlangel
 Author: xmlangel
 Author-email: kwangmyung.kim@gmail.com
 Keywords: selenium,xmlangel,utils
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `selenium_utils_xmlangel-0.0.2/setup.py` & `selenium_utils_xmlangel-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selenium_utils_xmlangel',
-    version='0.0.2',
+    version='0.0.3',
     description='PYPI selenium-utils package creation written by xmlangel',
     author='xmlangel',
     author_email='kwangmyung.kim@gmail.com',
     url='https://github.com/xmlangel/selenium-utils-xmlangel',
     install_requires=['opencv-python', 'scikit-image', ],
     packages=find_packages(exclude=[]),
     keywords=['selenium', 'xmlangel', 'utils'],
```

