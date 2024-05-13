# Comparing `tmp/torch_contour-0.0.3.tar.gz` & `tmp/torch_contour-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_contour-0.0.3.tar", last modified: Mon May 13 12:17:16 2024, max compression
+gzip compressed data, was "torch_contour-0.0.4.tar", last modified: Mon May 13 12:44:46 2024, max compression
```

## Comparing `torch_contour-0.0.3.tar` & `torch_contour-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-13 12:17:16.750321 torch_contour-0.0.3/
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     1068 2023-12-06 15:01:07.000000 torch_contour-0.0.3/LICENSE
--rw-r--r--   0 antoine   (1001) antoine   (1001)     2104 2024-05-13 12:17:16.750321 torch_contour-0.0.3/PKG-INFO
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     1207 2024-05-13 12:03:31.000000 torch_contour-0.0.3/README.md
--rw-rw-r--   0 antoine   (1001) antoine   (1001)      138 2023-12-06 15:01:07.000000 torch_contour-0.0.3/pyproject.toml
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     1054 2024-05-13 12:17:16.750321 torch_contour-0.0.3/setup.cfg
--rw-rw-r--   0 antoine   (1001) antoine   (1001)       53 2023-12-06 15:01:07.000000 torch_contour-0.0.3/setup.py
-drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-13 12:17:16.750321 torch_contour-0.0.3/torch_contour/
--rw-rw-r--   0 antoine   (1001) antoine   (1001)      146 2024-05-13 12:17:04.000000 torch_contour-0.0.3/torch_contour/__init__.py
--rw-rw-r--   0 antoine   (1001) antoine   (1001)        0 2023-12-06 15:01:07.000000 torch_contour-0.0.3/torch_contour/py.typed
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     2983 2024-05-13 12:07:20.000000 torch_contour-0.0.3/torch_contour/torch_contour.py
-drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-13 12:17:16.750321 torch_contour-0.0.3/torch_contour.egg-info/
--rw-r--r--   0 antoine   (1001) antoine   (1001)     2104 2024-05-13 12:17:16.000000 torch_contour-0.0.3/torch_contour.egg-info/PKG-INFO
--rw-rw-r--   0 antoine   (1001) antoine   (1001)      315 2024-05-13 12:17:16.000000 torch_contour-0.0.3/torch_contour.egg-info/SOURCES.txt
--rw-rw-r--   0 antoine   (1001) antoine   (1001)        1 2024-05-13 12:17:16.000000 torch_contour-0.0.3/torch_contour.egg-info/dependency_links.txt
--rw-rw-r--   0 antoine   (1001) antoine   (1001)        6 2024-05-13 12:17:16.000000 torch_contour-0.0.3/torch_contour.egg-info/requires.txt
--rw-rw-r--   0 antoine   (1001) antoine   (1001)       14 2024-05-13 12:17:16.000000 torch_contour-0.0.3/torch_contour.egg-info/top_level.txt
+drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-13 12:44:46.343956 torch_contour-0.0.4/
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     1068 2023-12-06 15:01:07.000000 torch_contour-0.0.4/LICENSE
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     2104 2024-05-13 12:44:46.343956 torch_contour-0.0.4/PKG-INFO
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     1207 2024-05-13 12:03:31.000000 torch_contour-0.0.4/README.md
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)      138 2023-12-06 15:01:07.000000 torch_contour-0.0.4/pyproject.toml
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     1054 2024-05-13 12:44:46.343956 torch_contour-0.0.4/setup.cfg
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)       53 2023-12-06 15:01:07.000000 torch_contour-0.0.4/setup.py
+drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-13 12:44:46.343956 torch_contour-0.0.4/torch_contour/
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)      146 2024-05-13 12:43:51.000000 torch_contour-0.0.4/torch_contour/__init__.py
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)        0 2023-12-06 15:01:07.000000 torch_contour-0.0.4/torch_contour/py.typed
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     5118 2024-05-13 12:43:06.000000 torch_contour-0.0.4/torch_contour/torch_contour.py
+drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-13 12:44:46.343956 torch_contour-0.0.4/torch_contour.egg-info/
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     2104 2024-05-13 12:44:46.000000 torch_contour-0.0.4/torch_contour.egg-info/PKG-INFO
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)      315 2024-05-13 12:44:46.000000 torch_contour-0.0.4/torch_contour.egg-info/SOURCES.txt
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)        1 2024-05-13 12:44:46.000000 torch_contour-0.0.4/torch_contour.egg-info/dependency_links.txt
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)        6 2024-05-13 12:44:46.000000 torch_contour-0.0.4/torch_contour.egg-info/requires.txt
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)       14 2024-05-13 12:44:46.000000 torch_contour-0.0.4/torch_contour.egg-info/top_level.txt
```

### Comparing `torch_contour-0.0.3/LICENSE` & `torch_contour-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_contour-0.0.3/PKG-INFO` & `torch_contour-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_contour
-Version: 0.0.3
+Version: 0.0.4
 Summary: Differentiable contour to mask and contour to distance map implementation with PyTorch
 Home-page: https://github.com/antoinehabis/torch_contour
 Author: Antoine Habis
 Author-email: antoine.habis.tlcm@gmail.com
 License: MIT
 Keywords: differentiable contour processing,pytorch,machine learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `torch_contour-0.0.3/README.md` & `torch_contour-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `torch_contour-0.0.3/setup.cfg` & `torch_contour-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `torch_contour-0.0.3/torch_contour.egg-info/PKG-INFO` & `torch_contour-0.0.4/torch_contour.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_contour
-Version: 0.0.3
+Version: 0.0.4
 Summary: Differentiable contour to mask and contour to distance map implementation with PyTorch
 Home-page: https://github.com/antoinehabis/torch_contour
 Author: Antoine Habis
 Author-email: antoine.habis.tlcm@gmail.com
 License: MIT
 Keywords: differentiable contour processing,pytorch,machine learning
 Classifier: Development Status :: 4 - Beta
```

