# Comparing `tmp/dcw-finder-0.0.4.tar.gz` & `tmp/dcw-finder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcw-finder-0.0.4.tar", last modified: Mon May 13 18:07:32 2024, max compression
+gzip compressed data, was "dcw-finder-0.0.5.tar", last modified: Mon May 13 18:09:49 2024, max compression
```

## Comparing `dcw-finder-0.0.4.tar` & `dcw-finder-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:07:32.254353 dcw-finder-0.0.4/
--rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:07:32.254145 dcw-finder-0.0.4/PKG-INFO
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:07:32.253919 dcw-finder-0.0.4/dcw_finder.egg-info/
--rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:07:32.000000 dcw-finder-0.0.4/dcw_finder.egg-info/PKG-INFO
--rw-r--r--   0 jrim       (501) staff       (20)      407 2024-05-13 18:07:32.000000 dcw-finder-0.0.4/dcw_finder.egg-info/SOURCES.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 18:07:32.000000 dcw-finder-0.0.4/dcw_finder.egg-info/dependency_links.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 17:52:51.000000 dcw-finder-0.0.4/dcw_finder.egg-info/not-zip-safe
--rw-r--r--   0 jrim       (501) staff       (20)        7 2024-05-13 18:07:32.000000 dcw-finder-0.0.4/dcw_finder.egg-info/requires.txt
--rw-r--r--   0 jrim       (501) staff       (20)        4 2024-05-13 18:07:32.000000 dcw-finder-0.0.4/dcw_finder.egg-info/top_level.txt
--rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-13 18:07:32.254404 dcw-finder-0.0.4/setup.cfg
--rw-r--r--   0 jrim       (501) staff       (20)      650 2024-05-13 18:07:30.000000 dcw-finder-0.0.4/setup.py
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:07:32.253710 dcw-finder-0.0.4/src/
--rw-r--r--   0 jrim       (501) staff       (20)      269 2024-05-13 18:07:25.000000 dcw-finder-0.0.4/src/__init__.py
--rw-r--r--   0 jrim       (501) staff       (20)     7746 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/_accessory.py
--rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/_blast.py
--rw-r--r--   0 jrim       (501) staff       (20)    11473 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/_cluster.py
--rw-r--r--   0 jrim       (501) staff       (20)    10164 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/_count.py
--rw-r--r--   0 jrim       (501) staff       (20)     7797 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/_parse.py
--rw-r--r--   0 jrim       (501) staff       (20)     2667 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/_profile.py
--rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/_search.py
--rw-r--r--   0 jrim       (501) staff       (20)     4183 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/_seqlib.py
--rw-r--r--   0 jrim       (501) staff       (20)     4337 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/_target.py
--rw-r--r--   0 jrim       (501) staff       (20)     5582 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/_utils.py
--rw-r--r--   0 jrim       (501) staff       (20)     6629 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/_visualize.py
--rw-r--r--   0 jrim       (501) staff       (20)     1971 2024-05-13 17:40:31.000000 dcw-finder-0.0.4/src/main.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:09:49.658986 dcw-finder-0.0.5/
+-rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:09:49.658774 dcw-finder-0.0.5/PKG-INFO
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:09:49.658528 dcw-finder-0.0.5/dcw_finder.egg-info/
+-rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:09:49.000000 dcw-finder-0.0.5/dcw_finder.egg-info/PKG-INFO
+-rw-r--r--   0 jrim       (501) staff       (20)      407 2024-05-13 18:09:49.000000 dcw-finder-0.0.5/dcw_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 18:09:49.000000 dcw-finder-0.0.5/dcw_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 17:52:51.000000 dcw-finder-0.0.5/dcw_finder.egg-info/not-zip-safe
+-rw-r--r--   0 jrim       (501) staff       (20)        7 2024-05-13 18:09:49.000000 dcw-finder-0.0.5/dcw_finder.egg-info/requires.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        4 2024-05-13 18:09:49.000000 dcw-finder-0.0.5/dcw_finder.egg-info/top_level.txt
+-rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-13 18:09:49.659044 dcw-finder-0.0.5/setup.cfg
+-rw-r--r--   0 jrim       (501) staff       (20)      650 2024-05-13 18:09:46.000000 dcw-finder-0.0.5/setup.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:09:49.658334 dcw-finder-0.0.5/src/
+-rw-r--r--   0 jrim       (501) staff       (20)      280 2024-05-13 18:09:42.000000 dcw-finder-0.0.5/src/__init__.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7746 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_accessory.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_blast.py
+-rw-r--r--   0 jrim       (501) staff       (20)    11473 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_cluster.py
+-rw-r--r--   0 jrim       (501) staff       (20)    10164 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_count.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7797 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_parse.py
+-rw-r--r--   0 jrim       (501) staff       (20)     2667 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_profile.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_search.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4183 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_seqlib.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4337 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_target.py
+-rw-r--r--   0 jrim       (501) staff       (20)     5582 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_utils.py
+-rw-r--r--   0 jrim       (501) staff       (20)     6629 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_visualize.py
+-rw-r--r--   0 jrim       (501) staff       (20)     1971 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/main.py
```

### Comparing `dcw-finder-0.0.4/setup.py` & `dcw-finder-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dcw-finder',
-    version='0.0.4',
+    version='0.0.5',
     description='Package for detecting dcw gene cluster',
     author='jsrim',
     author_email='comfortindex@naver.com',
     url='https://github.com/jrim42/gene-cluster',
     install_requires=['pandas'],
     packages=find_packages(exclude=[]),
     keywords=[],
```

### Comparing `dcw-finder-0.0.4/src/_accessory.py` & `dcw-finder-0.0.5/src/_accessory.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.4/src/_blast.py` & `dcw-finder-0.0.5/src/_blast.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.4/src/_cluster.py` & `dcw-finder-0.0.5/src/_cluster.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.4/src/_count.py` & `dcw-finder-0.0.5/src/_count.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.4/src/_parse.py` & `dcw-finder-0.0.5/src/_parse.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.4/src/_profile.py` & `dcw-finder-0.0.5/src/_profile.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.4/src/_search.py` & `dcw-finder-0.0.5/src/_search.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.4/src/_seqlib.py` & `dcw-finder-0.0.5/src/_seqlib.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.4/src/_target.py` & `dcw-finder-0.0.5/src/_target.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.4/src/_utils.py` & `dcw-finder-0.0.5/src/_utils.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.4/src/_visualize.py` & `dcw-finder-0.0.5/src/_visualize.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.4/src/main.py` & `dcw-finder-0.0.5/src/main.py`

 * *Files identical despite different names*

