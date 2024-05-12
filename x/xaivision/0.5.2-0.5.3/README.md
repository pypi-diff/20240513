# Comparing `tmp/xaivision-0.5.2.tar.gz` & `tmp/xaivision-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaivision-0.5.2.tar", max compression
+gzip compressed data, was "xaivision-0.5.3.tar", max compression
```

## Comparing `xaivision-0.5.2.tar` & `xaivision-0.5.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1114 2024-04-11 11:21:56.989947 xaivision-0.5.2/README.md
--rw-r--r--   0        0        0      265 2024-05-12 21:30:01.090229 xaivision-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       61 2024-04-13 15:44:32.244089 xaivision-0.5.2/xaivision/__init__.py
--rw-r--r--   0        0        0     2847 2024-04-13 21:30:38.041957 xaivision-0.5.2/xaivision/nmf_func.py
--rw-r--r--   0        0        0    13145 2024-04-18 14:10:52.763794 xaivision-0.5.2/xaivision/utils.py
--rw-r--r--   0        0        0    14137 2024-05-12 21:29:51.617075 xaivision-0.5.2/xaivision/xai_tools.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 xaivision-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-04-11 11:21:56.989947 xaivision-0.5.3/README.md
+-rw-r--r--   0        0        0      265 2024-05-12 21:39:19.907314 xaivision-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-04-13 15:44:32.244089 xaivision-0.5.3/xaivision/__init__.py
+-rw-r--r--   0        0        0     2847 2024-04-13 21:30:38.041957 xaivision-0.5.3/xaivision/nmf_func.py
+-rw-r--r--   0        0        0    13145 2024-04-18 14:10:52.763794 xaivision-0.5.3/xaivision/utils.py
+-rw-r--r--   0        0        0    14199 2024-05-12 21:39:12.564805 xaivision-0.5.3/xaivision/xai_tools.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 xaivision-0.5.3/PKG-INFO
```

### Comparing `xaivision-0.5.2/README.md` & `xaivision-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `xaivision-0.5.2/xaivision/nmf_func.py` & `xaivision-0.5.3/xaivision/nmf_func.py`

 * *Files identical despite different names*

### Comparing `xaivision-0.5.2/xaivision/utils.py` & `xaivision-0.5.3/xaivision/utils.py`

 * *Files identical despite different names*

### Comparing `xaivision-0.5.2/xaivision/xai_tools.py` & `xaivision-0.5.3/xaivision/xai_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,18 +200,18 @@
 def zero_non_largest_components(image, largest_component_pixels):
     """
     Zeros out pixels in the image that do not belong to the largest connected
     component.
 
     Args:
     - image (list): A binary image represented as a list of lists,
-      where each inner list represents a row of pixels and each pixel
-      has a value of either 0 or 1.
+                    where each inner list represents a row of pixels and each
+                    pixel has a value of either 0 or 1.
     - largest_component_pixels (set): A set of pixel coordinates belonging
-      to the largest connected component.
+                                        to the largest connected component.
 
     Returns:
     - list: The modified binary image with non-largest component pixels zeroed
             out.
     """
 
     height = len(image)
```

### Comparing `xaivision-0.5.2/PKG-INFO` & `xaivision-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xaivision
-Version: 0.5.2
+Version: 0.5.3
 Summary: 
 Author: philorfa
 Author-email: phil.orfa@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

