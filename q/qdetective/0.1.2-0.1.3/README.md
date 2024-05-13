# Comparing `tmp/qdetective-0.1.2.tar.gz` & `tmp/qdetective-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdetective-0.1.2.tar", max compression
+gzip compressed data, was "qdetective-0.1.3.tar", max compression
```

## Comparing `qdetective-0.1.2.tar` & `qdetective-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1075 2023-04-07 06:32:40.671062 qdetective-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      327 2024-05-13 03:37:47.269854 qdetective-0.1.2/pyproject.toml
--rwxr-xr-x   0        0        0     5399 2024-05-13 03:35:28.352348 qdetective-0.1.2/qdetective/__init__.py
--rw-r--r--   0        0        0      525 2024-05-13 03:38:02.026673 qdetective-0.1.2/setup.py
--rw-r--r--   0        0        0      271 2024-05-13 03:38:02.026757 qdetective-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1075 2023-04-07 06:32:40.671062 qdetective-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      326 2024-05-13 04:36:08.197263 qdetective-0.1.3/pyproject.toml
+-rwxr-xr-x   0        0        0     5399 2024-05-13 03:35:28.352348 qdetective-0.1.3/qdetective/__init__.py
+-rw-r--r--   0        0        0      524 2024-05-13 04:36:24.757325 qdetective-0.1.3/setup.py
+-rw-r--r--   0        0        0      470 2024-05-13 04:36:24.757408 qdetective-0.1.3/PKG-INFO
```

### Comparing `qdetective-0.1.2/LICENSE.txt` & `qdetective-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qdetective-0.1.2/qdetective/__init__.py` & `qdetective-0.1.3/qdetective/__init__.py`

 * *Files identical despite different names*

### Comparing `qdetective-0.1.2/setup.py` & `qdetective-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['qdetective']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'qdetective',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '量化大侦探-数据通道',
     'long_description': None,
     'author': 'suliang',
     'author_email': 'suliang_321@sina.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.6,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

