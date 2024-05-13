# Comparing `tmp/funcnodes_images-0.1.15.tar.gz` & `tmp/funcnodes_images-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_images-0.1.15.tar", max compression
+gzip compressed data, was "funcnodes_images-0.1.16.tar", max compression
```

## Comparing `funcnodes_images-0.1.15.tar` & `funcnodes_images-0.1.16.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1023 2024-04-25 11:41:55.701483 funcnodes_images-0.1.15/funcnodes_images/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-16 17:00:50.731308 funcnodes_images-0.1.15/funcnodes_images/_numpy.py
--rw-r--r--   0        0        0     1127 2024-04-16 16:22:29.320118 funcnodes_images-0.1.15/funcnodes_images/_pillow.py
--rw-r--r--   0        0        0     6585 2024-04-25 11:41:09.164599 funcnodes_images-0.1.15/funcnodes_images/image_nodes.py
--rw-r--r--   0        0        0     5338 2024-04-25 09:46:23.526949 funcnodes_images-0.1.15/funcnodes_images/imagecontainer.py
--rw-r--r--   0        0        0     1305 2024-04-16 16:47:30.447724 funcnodes_images-0.1.15/funcnodes_images/utils.py
--rw-r--r--   0        0        0      488 2024-04-25 11:41:47.027696 funcnodes_images-0.1.15/pyproject.toml
--rw-r--r--   0        0        0      349 2024-04-15 13:38:48.307325 funcnodes_images-0.1.15/README.md
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 funcnodes_images-0.1.15/PKG-INFO
+-rw-r--r--   0        0        0     1023 2024-05-13 05:44:49.553689 funcnodes_images-0.1.16/funcnodes_images/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-16 17:00:50.731308 funcnodes_images-0.1.16/funcnodes_images/_numpy.py
+-rw-r--r--   0        0        0     1127 2024-04-16 16:22:29.320118 funcnodes_images-0.1.16/funcnodes_images/_pillow.py
+-rw-r--r--   0        0        0     6585 2024-04-25 11:41:09.164599 funcnodes_images-0.1.16/funcnodes_images/image_nodes.py
+-rw-r--r--   0        0        0     5338 2024-04-25 09:46:23.526949 funcnodes_images-0.1.16/funcnodes_images/imagecontainer.py
+-rw-r--r--   0        0        0     1305 2024-04-16 16:47:30.447724 funcnodes_images-0.1.16/funcnodes_images/utils.py
+-rw-r--r--   0        0        0      474 2024-05-13 05:44:35.666758 funcnodes_images-0.1.16/pyproject.toml
+-rw-r--r--   0        0        0      349 2024-04-15 13:38:48.307325 funcnodes_images-0.1.16/README.md
+-rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 funcnodes_images-0.1.16/PKG-INFO
```

### Comparing `funcnodes_images-0.1.15/funcnodes_images/__init__.py` & `funcnodes_images-0.1.16/funcnodes_images/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,8 +35,8 @@
     "ImageFormat",
     "nodes",
     "FUNCNODES_RENDER_OPTIONS",
     "NODE_SHELF",
 ]
 
 
-__version__ = "0.1.15"
+__version__ = "0.1.16"
```

### Comparing `funcnodes_images-0.1.15/funcnodes_images/_numpy.py` & `funcnodes_images-0.1.16/funcnodes_images/_numpy.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.15/funcnodes_images/_pillow.py` & `funcnodes_images-0.1.16/funcnodes_images/_pillow.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.15/funcnodes_images/image_nodes.py` & `funcnodes_images-0.1.16/funcnodes_images/image_nodes.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.15/funcnodes_images/imagecontainer.py` & `funcnodes_images-0.1.16/funcnodes_images/imagecontainer.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.15/funcnodes_images/utils.py` & `funcnodes_images-0.1.16/funcnodes_images/utils.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.15/PKG-INFO` & `funcnodes_images-0.1.16/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: funcnodes_images
-Version: 0.1.15
+Version: 0.1.16
 Summary: 
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: funcnodes (>=0.1.42,<1.0.0)
-Requires-Dist: funcnodes-numpy (>=0.1.52,<0.2.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pillow (>=10.3.0,<11.0.0)
+Requires-Dist: funcnodes (>=0.1.42)
+Requires-Dist: funcnodes-numpy (>=0.1,<0.2)
+Requires-Dist: numpy (>=1.26,<2.0)
+Requires-Dist: pillow (>=10.3,<11.0)
 Description-Content-Type: text/markdown
 
 Bassic functionalities to work with images in Funcnodes
 
 Most important is the extendable "ImageFormat" class, which allows for automatic rendering and conversion of different image formats if they are implemented. Each should have their own respective package, e.g. funcnodes_opencv as this is only the basis for them to prevent reimplementations.
```

