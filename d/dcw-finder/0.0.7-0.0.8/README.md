# Comparing `tmp/dcw-finder-0.0.7.tar.gz` & `tmp/dcw-finder-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcw-finder-0.0.7.tar", last modified: Mon May 13 18:21:17 2024, max compression
+gzip compressed data, was "dcw-finder-0.0.8.tar", last modified: Mon May 13 18:23:14 2024, max compression
```

## Comparing `dcw-finder-0.0.7.tar` & `dcw-finder-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:21:17.989413 dcw-finder-0.0.7/
--rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:21:17.989176 dcw-finder-0.0.7/PKG-INFO
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:21:17.988874 dcw-finder-0.0.7/dcw_finder.egg-info/
--rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:21:17.000000 dcw-finder-0.0.7/dcw_finder.egg-info/PKG-INFO
--rw-r--r--   0 jrim       (501) staff       (20)      420 2024-05-13 18:21:17.000000 dcw-finder-0.0.7/dcw_finder.egg-info/SOURCES.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 18:21:17.000000 dcw-finder-0.0.7/dcw_finder.egg-info/dependency_links.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 17:52:51.000000 dcw-finder-0.0.7/dcw_finder.egg-info/not-zip-safe
--rw-r--r--   0 jrim       (501) staff       (20)        7 2024-05-13 18:21:17.000000 dcw-finder-0.0.7/dcw_finder.egg-info/requires.txt
--rw-r--r--   0 jrim       (501) staff       (20)        4 2024-05-13 18:21:17.000000 dcw-finder-0.0.7/dcw_finder.egg-info/top_level.txt
--rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-13 18:21:17.989467 dcw-finder-0.0.7/setup.cfg
--rw-r--r--   0 jrim       (501) staff       (20)      650 2024-05-13 18:21:14.000000 dcw-finder-0.0.7/setup.py
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:21:17.988659 dcw-finder-0.0.7/src/
--rw-r--r--   0 jrim       (501) staff       (20)      301 2024-05-13 18:21:07.000000 dcw-finder-0.0.7/src/__init__.py
--rw-r--r--   0 jrim       (501) staff       (20)     7747 2024-05-13 18:17:38.000000 dcw-finder-0.0.7/src/_accessory.py
--rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-13 17:40:31.000000 dcw-finder-0.0.7/src/_blast.py
--rw-r--r--   0 jrim       (501) staff       (20)    11475 2024-05-13 18:17:38.000000 dcw-finder-0.0.7/src/_cluster.py
--rw-r--r--   0 jrim       (501) staff       (20)    10160 2024-05-13 18:20:34.000000 dcw-finder-0.0.7/src/_count.py
--rw-r--r--   0 jrim       (501) staff       (20)    16245 2024-05-13 18:19:55.000000 dcw-finder-0.0.7/src/_info.py
--rw-r--r--   0 jrim       (501) staff       (20)     7793 2024-05-13 18:20:55.000000 dcw-finder-0.0.7/src/_parse.py
--rw-r--r--   0 jrim       (501) staff       (20)     2668 2024-05-13 18:17:38.000000 dcw-finder-0.0.7/src/_profile.py
--rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-13 17:40:31.000000 dcw-finder-0.0.7/src/_search.py
--rw-r--r--   0 jrim       (501) staff       (20)     4184 2024-05-13 18:17:38.000000 dcw-finder-0.0.7/src/_seqlib.py
--rw-r--r--   0 jrim       (501) staff       (20)     4337 2024-05-13 17:40:31.000000 dcw-finder-0.0.7/src/_target.py
--rw-r--r--   0 jrim       (501) staff       (20)     5582 2024-05-13 17:40:31.000000 dcw-finder-0.0.7/src/_utils.py
--rw-r--r--   0 jrim       (501) staff       (20)     6623 2024-05-13 18:20:34.000000 dcw-finder-0.0.7/src/_visualize.py
--rw-r--r--   0 jrim       (501) staff       (20)     1984 2024-05-13 18:17:38.000000 dcw-finder-0.0.7/src/main.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:23:14.968813 dcw-finder-0.0.8/
+-rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:23:14.968577 dcw-finder-0.0.8/PKG-INFO
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:23:14.968314 dcw-finder-0.0.8/dcw_finder.egg-info/
+-rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:23:14.000000 dcw-finder-0.0.8/dcw_finder.egg-info/PKG-INFO
+-rw-r--r--   0 jrim       (501) staff       (20)      420 2024-05-13 18:23:14.000000 dcw-finder-0.0.8/dcw_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 18:23:14.000000 dcw-finder-0.0.8/dcw_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 17:52:51.000000 dcw-finder-0.0.8/dcw_finder.egg-info/not-zip-safe
+-rw-r--r--   0 jrim       (501) staff       (20)        7 2024-05-13 18:23:14.000000 dcw-finder-0.0.8/dcw_finder.egg-info/requires.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        4 2024-05-13 18:23:14.000000 dcw-finder-0.0.8/dcw_finder.egg-info/top_level.txt
+-rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-13 18:23:14.968873 dcw-finder-0.0.8/setup.cfg
+-rw-r--r--   0 jrim       (501) staff       (20)      650 2024-05-13 18:23:12.000000 dcw-finder-0.0.8/setup.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:23:14.968097 dcw-finder-0.0.8/src/
+-rw-r--r--   0 jrim       (501) staff       (20)      301 2024-05-13 18:23:08.000000 dcw-finder-0.0.8/src/__init__.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7747 2024-05-13 18:17:38.000000 dcw-finder-0.0.8/src/_accessory.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-13 17:40:31.000000 dcw-finder-0.0.8/src/_blast.py
+-rw-r--r--   0 jrim       (501) staff       (20)    11475 2024-05-13 18:17:38.000000 dcw-finder-0.0.8/src/_cluster.py
+-rw-r--r--   0 jrim       (501) staff       (20)    10160 2024-05-13 18:20:34.000000 dcw-finder-0.0.8/src/_count.py
+-rw-r--r--   0 jrim       (501) staff       (20)    16245 2024-05-13 18:19:55.000000 dcw-finder-0.0.8/src/_info.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7793 2024-05-13 18:20:55.000000 dcw-finder-0.0.8/src/_parse.py
+-rw-r--r--   0 jrim       (501) staff       (20)     2668 2024-05-13 18:17:38.000000 dcw-finder-0.0.8/src/_profile.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-13 17:40:31.000000 dcw-finder-0.0.8/src/_search.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4184 2024-05-13 18:17:38.000000 dcw-finder-0.0.8/src/_seqlib.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4337 2024-05-13 17:40:31.000000 dcw-finder-0.0.8/src/_target.py
+-rw-r--r--   0 jrim       (501) staff       (20)     5582 2024-05-13 17:40:31.000000 dcw-finder-0.0.8/src/_utils.py
+-rw-r--r--   0 jrim       (501) staff       (20)     6584 2024-05-13 18:22:56.000000 dcw-finder-0.0.8/src/_visualize.py
+-rw-r--r--   0 jrim       (501) staff       (20)     1984 2024-05-13 18:17:38.000000 dcw-finder-0.0.8/src/main.py
```

### Comparing `dcw-finder-0.0.7/setup.py` & `dcw-finder-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dcw-finder',
-    version='0.0.7',
+    version='0.0.8',
     description='Package for detecting dcw gene cluster',
     author='jsrim',
     author_email='comfortindex@naver.com',
     url='https://github.com/jrim42/gene-cluster',
     install_requires=['pandas'],
     packages=find_packages(exclude=[]),
     keywords=[],
```

### Comparing `dcw-finder-0.0.7/src/_accessory.py` & `dcw-finder-0.0.8/src/_accessory.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.7/src/_blast.py` & `dcw-finder-0.0.8/src/_blast.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.7/src/_cluster.py` & `dcw-finder-0.0.8/src/_cluster.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.7/src/_count.py` & `dcw-finder-0.0.8/src/_count.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.7/src/_info.py` & `dcw-finder-0.0.8/src/_info.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.7/src/_parse.py` & `dcw-finder-0.0.8/src/_parse.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.7/src/_profile.py` & `dcw-finder-0.0.8/src/_profile.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.7/src/_search.py` & `dcw-finder-0.0.8/src/_search.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.7/src/_seqlib.py` & `dcw-finder-0.0.8/src/_seqlib.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.7/src/_target.py` & `dcw-finder-0.0.8/src/_target.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.7/src/_utils.py` & `dcw-finder-0.0.8/src/_utils.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.7/src/_visualize.py` & `dcw-finder-0.0.8/src/_visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.patches as mpatches
 from matplotlib.font_manager import FontProperties
 from matplotlib.colors import LinearSegmentedColormap
 
-import sys
-sys.path.append('../info/')
 from _info import target_color
 
 #------------------------------------------------------------
 def visualize_cluster_type(output_dir, df):
   x = np.arange(len(df))
   width = 0.3
```

### Comparing `dcw-finder-0.0.7/src/main.py` & `dcw-finder-0.0.8/src/main.py`

 * *Files identical despite different names*

