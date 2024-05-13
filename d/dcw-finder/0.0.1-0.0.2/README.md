# Comparing `tmp/dcw-finder-0.0.1.tar.gz` & `tmp/dcw-finder-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcw-finder-0.0.1.tar", last modified: Mon May 13 17:45:34 2024, max compression
+gzip compressed data, was "dcw-finder-0.0.2.tar", last modified: Mon May 13 17:52:51 2024, max compression
```

## Comparing `dcw-finder-0.0.1.tar` & `dcw-finder-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 17:45:34.192678 dcw-finder-0.0.1/
--rw-r--r--   0 jrim       (501) staff       (20)      469 2024-05-13 17:45:34.192438 dcw-finder-0.0.1/PKG-INFO
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 17:45:34.192163 dcw-finder-0.0.1/dcw_finder.egg-info/
--rw-r--r--   0 jrim       (501) staff       (20)      469 2024-05-13 17:45:34.000000 dcw-finder-0.0.1/dcw_finder.egg-info/PKG-INFO
--rw-r--r--   0 jrim       (501) staff       (20)      407 2024-05-13 17:45:34.000000 dcw-finder-0.0.1/dcw_finder.egg-info/SOURCES.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 17:45:34.000000 dcw-finder-0.0.1/dcw_finder.egg-info/dependency_links.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 17:45:34.000000 dcw-finder-0.0.1/dcw_finder.egg-info/not-zip-safe
--rw-r--r--   0 jrim       (501) staff       (20)       13 2024-05-13 17:45:34.000000 dcw-finder-0.0.1/dcw_finder.egg-info/requires.txt
--rw-r--r--   0 jrim       (501) staff       (20)        4 2024-05-13 17:45:34.000000 dcw-finder-0.0.1/dcw_finder.egg-info/top_level.txt
--rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-13 17:45:34.192736 dcw-finder-0.0.1/setup.cfg
--rw-r--r--   0 jrim       (501) staff       (20)      658 2024-05-13 17:44:08.000000 dcw-finder-0.0.1/setup.py
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 17:45:34.191960 dcw-finder-0.0.1/src/
--rw-r--r--   0 jrim       (501) staff       (20)       22 2024-05-13 17:45:02.000000 dcw-finder-0.0.1/src/__init__.py
--rw-r--r--   0 jrim       (501) staff       (20)     7746 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/_accessory.py
--rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/_blast.py
--rw-r--r--   0 jrim       (501) staff       (20)    11473 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/_cluster.py
--rw-r--r--   0 jrim       (501) staff       (20)    10164 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/_count.py
--rw-r--r--   0 jrim       (501) staff       (20)     7797 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/_parse.py
--rw-r--r--   0 jrim       (501) staff       (20)     2667 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/_profile.py
--rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/_search.py
--rw-r--r--   0 jrim       (501) staff       (20)     4183 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/_seqlib.py
--rw-r--r--   0 jrim       (501) staff       (20)     4337 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/_target.py
--rw-r--r--   0 jrim       (501) staff       (20)     5582 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/_utils.py
--rw-r--r--   0 jrim       (501) staff       (20)     6629 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/_visualize.py
--rw-r--r--   0 jrim       (501) staff       (20)     1971 2024-05-13 17:40:31.000000 dcw-finder-0.0.1/src/main.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 17:52:51.447030 dcw-finder-0.0.2/
+-rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 17:52:51.446821 dcw-finder-0.0.2/PKG-INFO
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 17:52:51.446560 dcw-finder-0.0.2/dcw_finder.egg-info/
+-rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 17:52:51.000000 dcw-finder-0.0.2/dcw_finder.egg-info/PKG-INFO
+-rw-r--r--   0 jrim       (501) staff       (20)      407 2024-05-13 17:52:51.000000 dcw-finder-0.0.2/dcw_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 17:52:51.000000 dcw-finder-0.0.2/dcw_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 17:52:51.000000 dcw-finder-0.0.2/dcw_finder.egg-info/not-zip-safe
+-rw-r--r--   0 jrim       (501) staff       (20)        7 2024-05-13 17:52:51.000000 dcw-finder-0.0.2/dcw_finder.egg-info/requires.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        4 2024-05-13 17:52:51.000000 dcw-finder-0.0.2/dcw_finder.egg-info/top_level.txt
+-rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-13 17:52:51.447083 dcw-finder-0.0.2/setup.cfg
+-rw-r--r--   0 jrim       (501) staff       (20)      650 2024-05-13 17:52:16.000000 dcw-finder-0.0.2/setup.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 17:52:51.446350 dcw-finder-0.0.2/src/
+-rw-r--r--   0 jrim       (501) staff       (20)       22 2024-05-13 17:52:19.000000 dcw-finder-0.0.2/src/__init__.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7746 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/_accessory.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/_blast.py
+-rw-r--r--   0 jrim       (501) staff       (20)    11473 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/_cluster.py
+-rw-r--r--   0 jrim       (501) staff       (20)    10164 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/_count.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7797 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/_parse.py
+-rw-r--r--   0 jrim       (501) staff       (20)     2667 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/_profile.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/_search.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4183 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/_seqlib.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4337 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/_target.py
+-rw-r--r--   0 jrim       (501) staff       (20)     5582 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/_utils.py
+-rw-r--r--   0 jrim       (501) staff       (20)     6629 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/_visualize.py
+-rw-r--r--   0 jrim       (501) staff       (20)     1971 2024-05-13 17:40:31.000000 dcw-finder-0.0.2/src/main.py
```

### Comparing `dcw-finder-0.0.1/setup.py` & `dcw-finder-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dcw-finder',
-    version='0.0.1',
-    description='package for detecting dcw gene cluster',
+    version='0.0.2',
+    description='Package for detecting dcw gene cluster',
     author='jsrim',
     author_email='comfortindex@naver.com',
     url='https://github.com/jrim42/gene-cluster',
-    install_requires=['conda', 'pandas'],
+    install_requires=['pandas'],
     packages=find_packages(exclude=[]),
     keywords=[],
     python_requires='>=3.6',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-)
+)
```

### Comparing `dcw-finder-0.0.1/src/_accessory.py` & `dcw-finder-0.0.2/src/_accessory.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.1/src/_blast.py` & `dcw-finder-0.0.2/src/_blast.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.1/src/_cluster.py` & `dcw-finder-0.0.2/src/_cluster.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.1/src/_count.py` & `dcw-finder-0.0.2/src/_count.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.1/src/_parse.py` & `dcw-finder-0.0.2/src/_parse.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.1/src/_profile.py` & `dcw-finder-0.0.2/src/_profile.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.1/src/_search.py` & `dcw-finder-0.0.2/src/_search.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.1/src/_seqlib.py` & `dcw-finder-0.0.2/src/_seqlib.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.1/src/_target.py` & `dcw-finder-0.0.2/src/_target.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.1/src/_utils.py` & `dcw-finder-0.0.2/src/_utils.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.1/src/_visualize.py` & `dcw-finder-0.0.2/src/_visualize.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.1/src/main.py` & `dcw-finder-0.0.2/src/main.py`

 * *Files identical despite different names*

