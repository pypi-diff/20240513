# Comparing `tmp/furrow1k-0.1.9.tar.gz` & `tmp/furrow1k-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furrow1k-0.1.9.tar", max compression
+gzip compressed data, was "furrow1k-1.0.0.tar", max compression
```

## Comparing `furrow1k-0.1.9.tar` & `furrow1k-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1068 2024-05-05 22:35:02.889442 furrow1k-0.1.9/LICENSE
--rw-r--r--   0        0        0      657 2024-05-05 22:35:02.901477 furrow1k-0.1.9/README.md
--rw-r--r--   0        0        0      415 2024-05-06 02:38:20.671228 furrow1k-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      110 2024-05-05 22:35:02.934491 furrow1k-0.1.9/src/furrow1k/__init__.py
--rw-r--r--   0        0        0      839 2024-05-06 02:38:12.938312 furrow1k-0.1.9/src/furrow1k/furrow1k.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 furrow1k-0.1.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1068 2024-05-05 22:35:02.889442 furrow1k-1.0.0/LICENSE
+-rw-r--r--   0        0        0      657 2024-05-05 22:35:02.901477 furrow1k-1.0.0/README.md
+-rw-r--r--   0        0        0      475 2024-05-13 03:13:02.990240 furrow1k-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-05-05 22:35:02.934491 furrow1k-1.0.0/src/furrow1k/__init__.py
+-rw-r--r--   0        0        0     6818 2024-05-13 02:44:45.928917 furrow1k-1.0.0/src/furrow1k/furrow1k.py
+-rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 furrow1k-1.0.0/PKG-INFO
```

### Comparing `furrow1k-0.1.9/LICENSE` & `furrow1k-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `furrow1k-0.1.9/README.md` & `furrow1k-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `furrow1k-0.1.9/PKG-INFO` & `furrow1k-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: furrow1k
-Version: 0.1.9
+Version: 1.0.0
 Summary: Help calculate percentage of salary to contribute to 401k
 License: MIT
 Author: Frank Cao
 Requires-Python: >=3.12.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # furrow1k
 
 Help calculate percentage of salary to contribute to 401k
 
 ## Installation
```

