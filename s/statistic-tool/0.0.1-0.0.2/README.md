# Comparing `tmp/statistic_tool-0.0.1.tar.gz` & `tmp/statistic_tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statistic_tool-0.0.1.tar", last modified: Fri May  3 08:55:31 2024, max compression
+gzip compressed data, was "statistic_tool-0.0.2.tar", last modified: Mon May 13 13:03:30 2024, max compression
```

## Comparing `statistic_tool-0.0.1.tar` & `statistic_tool-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:55:31.572079 statistic_tool-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-03 08:55:21.000000 statistic_tool-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-03 08:55:31.572079 statistic_tool-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 08:55:21.000000 statistic_tool-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 08:55:21.000000 statistic_tool-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 08:55:31.572079 statistic_tool-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-03 08:55:21.000000 statistic_tool-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:55:31.572079 statistic_tool-0.0.1/statistic_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:55:21.000000 statistic_tool-0.0.1/statistic_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-03 08:55:21.000000 statistic_tool-0.0.1/statistic_tool/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:55:31.572079 statistic_tool-0.0.1/statistic_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-03 08:55:31.000000 statistic_tool-0.0.1/statistic_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-03 08:55:31.000000 statistic_tool-0.0.1/statistic_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 08:55:31.000000 statistic_tool-0.0.1/statistic_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 08:55:31.000000 statistic_tool-0.0.1/statistic_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 08:55:31.000000 statistic_tool-0.0.1/statistic_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:03:30.063705 statistic_tool-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-13 13:03:30.063705 statistic_tool-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:03:30.063705 statistic_tool-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:03:30.063705 statistic_tool-0.0.2/statistic_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/statistic_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/statistic_tool/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-13 13:03:20.000000 statistic_tool-0.0.2/statistic_tool/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:03:30.063705 statistic_tool-0.0.2/statistic_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-13 13:03:30.000000 statistic_tool-0.0.2/statistic_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-13 13:03:30.000000 statistic_tool-0.0.2/statistic_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:03:30.000000 statistic_tool-0.0.2/statistic_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 13:03:30.000000 statistic_tool-0.0.2/statistic_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 13:03:30.000000 statistic_tool-0.0.2/statistic_tool.egg-info/top_level.txt
```

### Comparing `statistic_tool-0.0.1/LICENSE` & `statistic_tool-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statistic_tool-0.0.1/PKG-INFO` & `statistic_tool-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statistic-tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: simple functions for statistic
 Home-page: https://github.com/cheerzhang/statistic_tool
 Author: ZhangLe
 Author-email: zhangle@gmail.com
 Project-URL: Bug Tracker, https://github.com/cheerzhang/statistic_tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `statistic_tool-0.0.1/setup.py` & `statistic_tool-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='statistic-tool',
-    version='0.0.1',
+    version='0.0.2',
     author="ZhangLe",
     author_email="zhangle@gmail.com",
     description="simple functions for statistic",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cheerzhang/statistic_tool",
     project_urls={
```

### Comparing `statistic_tool-0.0.1/statistic_tool.egg-info/PKG-INFO` & `statistic_tool-0.0.2/statistic_tool.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statistic-tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: simple functions for statistic
 Home-page: https://github.com/cheerzhang/statistic_tool
 Author: ZhangLe
 Author-email: zhangle@gmail.com
 Project-URL: Bug Tracker, https://github.com/cheerzhang/statistic_tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

