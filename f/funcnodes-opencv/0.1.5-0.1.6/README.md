# Comparing `tmp/funcnodes_opencv-0.1.5.tar.gz` & `tmp/funcnodes_opencv-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_opencv-0.1.5.tar", max compression
+gzip compressed data, was "funcnodes_opencv-0.1.6.tar", max compression
```

## Comparing `funcnodes_opencv-0.1.5.tar` & `funcnodes_opencv-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      572 2024-05-13 05:19:43.219778 funcnodes_opencv-0.1.5/funcnodes_opencv/__init__.py
--rw-r--r--   0        0        0      923 2024-05-10 03:41:57.002216 funcnodes_opencv-0.1.5/funcnodes_opencv/colormodes.py
--rw-r--r--   0        0        0     1333 2024-05-10 09:30:00.771338 funcnodes_opencv-0.1.5/funcnodes_opencv/components.py
--rw-r--r--   0        0        0     6490 2024-05-10 06:28:01.061816 funcnodes_opencv-0.1.5/funcnodes_opencv/filter.py
--rw-r--r--   0        0        0     8347 2024-05-10 03:41:23.858486 funcnodes_opencv-0.1.5/funcnodes_opencv/image_operations.py
--rw-r--r--   0        0        0     2818 2024-05-10 06:50:49.080766 funcnodes_opencv-0.1.5/funcnodes_opencv/imageformat.py
--rw-r--r--   0        0        0     5813 2024-05-13 05:02:48.256439 funcnodes_opencv-0.1.5/funcnodes_opencv/masks.py
--rw-r--r--   0        0        0      903 2024-05-10 09:28:17.466933 funcnodes_opencv-0.1.5/funcnodes_opencv/utils.py
--rw-r--r--   0        0        0      404 2024-05-13 05:20:08.370239 funcnodes_opencv-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_opencv-0.1.5/README.md
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 funcnodes_opencv-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      572 2024-05-13 05:39:55.662489 funcnodes_opencv-0.1.6/funcnodes_opencv/__init__.py
+-rw-r--r--   0        0        0      923 2024-05-10 03:41:57.002216 funcnodes_opencv-0.1.6/funcnodes_opencv/colormodes.py
+-rw-r--r--   0        0        0     1333 2024-05-10 09:30:00.771338 funcnodes_opencv-0.1.6/funcnodes_opencv/components.py
+-rw-r--r--   0        0        0     6490 2024-05-10 06:28:01.061816 funcnodes_opencv-0.1.6/funcnodes_opencv/filter.py
+-rw-r--r--   0        0        0     8347 2024-05-10 03:41:23.858486 funcnodes_opencv-0.1.6/funcnodes_opencv/image_operations.py
+-rw-r--r--   0        0        0     2818 2024-05-10 06:50:49.080766 funcnodes_opencv-0.1.6/funcnodes_opencv/imageformat.py
+-rw-r--r--   0        0        0     5813 2024-05-13 05:02:48.256439 funcnodes_opencv-0.1.6/funcnodes_opencv/masks.py
+-rw-r--r--   0        0        0      903 2024-05-10 09:28:17.466933 funcnodes_opencv-0.1.6/funcnodes_opencv/utils.py
+-rw-r--r--   0        0        0      408 2024-05-13 05:39:41.814443 funcnodes_opencv-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_opencv-0.1.6/README.md
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 funcnodes_opencv-0.1.6/PKG-INFO
```

### Comparing `funcnodes_opencv-0.1.5/funcnodes_opencv/__init__.py` & `funcnodes_opencv-0.1.6/funcnodes_opencv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from . import image_operations, masks, colormodes, filter, components
 import funcnodes as fn
 import funcnodes_numpy as fnnp  # noqa: F401 # for type hinting
 
 __all__ = ["OpenCVImageFormat", "image_operations", "masks"]
 
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 
 NODE_SHELF = fn.Shelf(
     name="OpenCV",
     description="OpenCV image processing nodes.",
     subshelves=[
         image_operations.NODE_SHELF,
```

### Comparing `funcnodes_opencv-0.1.5/funcnodes_opencv/colormodes.py` & `funcnodes_opencv-0.1.6/funcnodes_opencv/colormodes.py`

 * *Files identical despite different names*

### Comparing `funcnodes_opencv-0.1.5/funcnodes_opencv/components.py` & `funcnodes_opencv-0.1.6/funcnodes_opencv/components.py`

 * *Files identical despite different names*

### Comparing `funcnodes_opencv-0.1.5/funcnodes_opencv/filter.py` & `funcnodes_opencv-0.1.6/funcnodes_opencv/filter.py`

 * *Files identical despite different names*

### Comparing `funcnodes_opencv-0.1.5/funcnodes_opencv/image_operations.py` & `funcnodes_opencv-0.1.6/funcnodes_opencv/image_operations.py`

 * *Files identical despite different names*

### Comparing `funcnodes_opencv-0.1.5/funcnodes_opencv/imageformat.py` & `funcnodes_opencv-0.1.6/funcnodes_opencv/imageformat.py`

 * *Files identical despite different names*

### Comparing `funcnodes_opencv-0.1.5/funcnodes_opencv/masks.py` & `funcnodes_opencv-0.1.6/funcnodes_opencv/masks.py`

 * *Files identical despite different names*

### Comparing `funcnodes_opencv-0.1.5/funcnodes_opencv/utils.py` & `funcnodes_opencv-0.1.6/funcnodes_opencv/utils.py`

 * *Files identical despite different names*

### Comparing `funcnodes_opencv-0.1.5/PKG-INFO` & `funcnodes_opencv-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: funcnodes-opencv
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: funcnodes (>=0.2,<0.3)
-Requires-Dist: funcnodes-numpy
-Requires-Dist: funcnodes_images (>=0.1.15,<0.2.0)
-Requires-Dist: opencv-python-headless (>=4.9.0.80,<5.0.0.0)
+Requires-Dist: funcnodes (>=0.2.6)
+Requires-Dist: funcnodes-numpy (>=0.1.57)
+Requires-Dist: funcnodes_images (>0.1.5)
+Requires-Dist: opencv-python-headless (>=4.9,<5.0)
 Description-Content-Type: text/markdown
```

