# Comparing `tmp/pixeloe-0.0.8.tar.gz` & `tmp/pixeloe-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixeloe-0.0.8.tar", last modified: Thu Apr 11 02:59:08 2024, max compression
+gzip compressed data, was "pixeloe-0.0.9.tar", last modified: Thu Apr 11 03:13:44 2024, max compression
```

## Comparing `pixeloe-0.0.8.tar` & `pixeloe-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 02:59:08.951105 pixeloe-0.0.8/
--rw-r--r--   0 kblueleaf   (501) staff       (20)    11344 2024-03-29 05:43:29.000000 pixeloe-0.0.8/LICENSE
--rw-r--r--   0 kblueleaf   (501) staff       (20)      407 2024-04-11 02:59:08.950801 pixeloe-0.0.8/PKG-INFO
--rw-r--r--   0 kblueleaf   (501) staff       (20)     7517 2024-04-11 02:57:31.000000 pixeloe-0.0.8/README.md
-drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 02:59:08.947085 pixeloe-0.0.8/pixeloe/
--rw-r--r--   0 kblueleaf   (501) staff       (20)        0 2024-04-11 02:57:08.000000 pixeloe-0.0.8/pixeloe/__init__.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     3637 2024-04-06 13:40:12.000000 pixeloe-0.0.8/pixeloe/cli.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     2193 2024-04-06 13:44:10.000000 pixeloe-0.0.8/pixeloe/color.py
-drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 02:59:08.950133 pixeloe-0.0.8/pixeloe/downscale/
--rw-r--r--   0 kblueleaf   (501) staff       (20)      363 2024-03-31 16:49:46.000000 pixeloe-0.0.8/pixeloe/downscale/__init__.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     1113 2024-04-06 13:42:55.000000 pixeloe-0.0.8/pixeloe/downscale/center.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     1554 2024-04-06 13:42:55.000000 pixeloe-0.0.8/pixeloe/downscale/contrast_based.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)      894 2024-04-06 13:42:55.000000 pixeloe-0.0.8/pixeloe/downscale/conventional.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     1772 2024-04-06 13:42:55.000000 pixeloe-0.0.8/pixeloe/downscale/k_centroid.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     3189 2024-04-06 13:42:41.000000 pixeloe-0.0.8/pixeloe/outline.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     1915 2024-04-06 13:39:38.000000 pixeloe-0.0.8/pixeloe/pixelize.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)      903 2024-04-06 13:59:07.000000 pixeloe-0.0.8/pixeloe/utils.py
-drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 02:59:08.950508 pixeloe-0.0.8/pixeloe.egg-info/
--rw-r--r--   0 kblueleaf   (501) staff       (20)      407 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/PKG-INFO
--rw-r--r--   0 kblueleaf   (501) staff       (20)      512 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/SOURCES.txt
--rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/dependency_links.txt
--rw-r--r--   0 kblueleaf   (501) staff       (20)       96 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/entry_points.txt
--rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2024-03-29 05:49:33.000000 pixeloe-0.0.8/pixeloe.egg-info/not-zip-safe
--rw-r--r--   0 kblueleaf   (501) staff       (20)       27 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/requires.txt
--rw-r--r--   0 kblueleaf   (501) staff       (20)        8 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/top_level.txt
--rw-r--r--   0 kblueleaf   (501) staff       (20)       38 2024-04-11 02:59:08.951166 pixeloe-0.0.8/setup.cfg
--rw-r--r--   0 kblueleaf   (501) staff       (20)      699 2024-04-11 02:59:04.000000 pixeloe-0.0.8/setup.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 03:13:44.823011 pixeloe-0.0.9/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    11344 2024-03-29 05:43:29.000000 pixeloe-0.0.9/LICENSE
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      407 2024-04-11 03:13:44.822724 pixeloe-0.0.9/PKG-INFO
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     7517 2024-04-11 02:57:31.000000 pixeloe-0.0.9/README.md
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 03:13:44.818971 pixeloe-0.0.9/pixeloe/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        0 2024-04-11 02:57:08.000000 pixeloe-0.0.9/pixeloe/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     3637 2024-04-06 13:40:12.000000 pixeloe-0.0.9/pixeloe/cli.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     2193 2024-04-06 13:44:10.000000 pixeloe-0.0.9/pixeloe/color.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 03:13:44.822081 pixeloe-0.0.9/pixeloe/downscale/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      363 2024-03-31 16:49:46.000000 pixeloe-0.0.9/pixeloe/downscale/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1113 2024-04-06 13:42:55.000000 pixeloe-0.0.9/pixeloe/downscale/center.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1554 2024-04-06 13:42:55.000000 pixeloe-0.0.9/pixeloe/downscale/contrast_based.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      894 2024-04-06 13:42:55.000000 pixeloe-0.0.9/pixeloe/downscale/conventional.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1772 2024-04-06 13:42:55.000000 pixeloe-0.0.9/pixeloe/downscale/k_centroid.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     3189 2024-04-06 13:42:41.000000 pixeloe-0.0.9/pixeloe/outline.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1915 2024-04-06 13:39:38.000000 pixeloe-0.0.9/pixeloe/pixelize.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1103 2024-04-11 03:13:10.000000 pixeloe-0.0.9/pixeloe/utils.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 03:13:44.822421 pixeloe-0.0.9/pixeloe.egg-info/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      407 2024-04-11 03:13:44.000000 pixeloe-0.0.9/pixeloe.egg-info/PKG-INFO
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      512 2024-04-11 03:13:44.000000 pixeloe-0.0.9/pixeloe.egg-info/SOURCES.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2024-04-11 03:13:44.000000 pixeloe-0.0.9/pixeloe.egg-info/dependency_links.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       96 2024-04-11 03:13:44.000000 pixeloe-0.0.9/pixeloe.egg-info/entry_points.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2024-03-29 05:49:33.000000 pixeloe-0.0.9/pixeloe.egg-info/not-zip-safe
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       27 2024-04-11 03:13:44.000000 pixeloe-0.0.9/pixeloe.egg-info/requires.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        8 2024-04-11 03:13:44.000000 pixeloe-0.0.9/pixeloe.egg-info/top_level.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       38 2024-04-11 03:13:44.823080 pixeloe-0.0.9/setup.cfg
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      699 2024-04-11 03:13:44.000000 pixeloe-0.0.9/setup.py
```

### Comparing `pixeloe-0.0.8/LICENSE` & `pixeloe-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.8/README.md` & `pixeloe-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.8/pixeloe/cli.py` & `pixeloe-0.0.9/pixeloe/cli.py`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.8/pixeloe/color.py` & `pixeloe-0.0.9/pixeloe/color.py`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.8/pixeloe/downscale/center.py` & `pixeloe-0.0.9/pixeloe/downscale/center.py`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.8/pixeloe/downscale/contrast_based.py` & `pixeloe-0.0.9/pixeloe/downscale/contrast_based.py`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.8/pixeloe/downscale/conventional.py` & `pixeloe-0.0.9/pixeloe/downscale/conventional.py`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.8/pixeloe/downscale/k_centroid.py` & `pixeloe-0.0.9/pixeloe/downscale/k_centroid.py`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.8/pixeloe/outline.py` & `pixeloe-0.0.9/pixeloe/outline.py`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.8/pixeloe/pixelize.py` & `pixeloe-0.0.9/pixeloe/pixelize.py`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.8/pixeloe.egg-info/SOURCES.txt` & `pixeloe-0.0.9/pixeloe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.8/setup.py` & `pixeloe-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pixeloe import cli
 
 
 setup(
     name="pixeloe",
     packages=find_packages(),
-    version="0.0.8",
+    version="0.0.9",
     url="https://github.com/KohakuBlueleaf/PixelOE",
     description="Detail-Oriented Pixelization based on Contrast-Aware Outline Expansion.",
     license="Apache License 2.0",
     author="Shih-Ying Yeh(KohakuBlueLeaf)",
     author_email="apolloyeh0123@gmail.com",
     zip_safe=False,
     install_requires=["opencv-python", "numpy", "pillow"],
```

