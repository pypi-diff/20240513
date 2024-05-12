# Comparing `tmp/torch_model_manager-0.3.0.dev7.tar.gz` & `tmp/torch_model_manager-0.3.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.3.0.dev7.tar", last modified: Sun May 12 19:58:16 2024, max compression
+gzip compressed data, was "torch_model_manager-0.3.0.dev8.tar", last modified: Sun May 12 20:02:13 2024, max compression
```

## Comparing `torch_model_manager-0.3.0.dev7.tar` & `torch_model_manager-0.3.0.dev8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:58:16.107188 torch_model_manager-0.3.0.dev7/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8905 2024-05-12 19:58:16.107188 torch_model_manager-0.3.0.dev7/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev7/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-12 19:58:16.107188 torch_model_manager-0.3.0.dev7/setup.cfg
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     1975 2024-05-12 19:58:13.000000 torch_model_manager-0.3.0.dev7/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:58:16.099188 torch_model_manager-0.3.0.dev7/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:58:16.099188 torch_model_manager-0.3.0.dev7/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev7/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev7/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:58:16.099188 torch_model_manager-0.3.0.dev7/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev7/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev7/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:58:16.103188 torch_model_manager-0.3.0.dev7/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      140 2024-05-12 19:04:44.000000 torch_model_manager-0.3.0.dev7/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    31658 2024-05-12 19:39:19.000000 torch_model_manager-0.3.0.dev7/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1672 2024-05-11 19:12:46.000000 torch_model_manager-0.3.0.dev7/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-09 18:52:45.000000 torch_model_manager-0.3.0.dev7/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-11 10:54:45.000000 torch_model_manager-0.3.0.dev7/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:58:16.103188 torch_model_manager-0.3.0.dev7/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8905 2024-05-12 19:58:16.000000 torch_model_manager-0.3.0.dev7/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      622 2024-05-12 19:58:16.000000 torch_model_manager-0.3.0.dev7/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-12 19:58:16.000000 torch_model_manager-0.3.0.dev7/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      116 2024-05-12 19:58:16.000000 torch_model_manager-0.3.0.dev7/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-12 19:58:16.000000 torch_model_manager-0.3.0.dev7/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:58:16.103188 torch_model_manager-0.3.0.dev7/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev7/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8619 2024-05-09 19:01:45.000000 torch_model_manager-0.3.0.dev7/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 20:02:13.289305 torch_model_manager-0.3.0.dev8/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8905 2024-05-12 20:02:13.289305 torch_model_manager-0.3.0.dev8/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev8/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-12 20:02:13.289305 torch_model_manager-0.3.0.dev8/setup.cfg
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     1975 2024-05-12 20:02:10.000000 torch_model_manager-0.3.0.dev8/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 20:02:13.285305 torch_model_manager-0.3.0.dev8/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 20:02:13.285305 torch_model_manager-0.3.0.dev8/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev8/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev8/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 20:02:13.285305 torch_model_manager-0.3.0.dev8/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev8/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev8/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 20:02:13.285305 torch_model_manager-0.3.0.dev8/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       94 2024-05-12 20:02:05.000000 torch_model_manager-0.3.0.dev8/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    31658 2024-05-12 19:39:19.000000 torch_model_manager-0.3.0.dev8/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1672 2024-05-11 19:12:46.000000 torch_model_manager-0.3.0.dev8/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-09 18:52:45.000000 torch_model_manager-0.3.0.dev8/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-11 10:54:45.000000 torch_model_manager-0.3.0.dev8/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 20:02:13.289305 torch_model_manager-0.3.0.dev8/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8905 2024-05-12 20:02:13.000000 torch_model_manager-0.3.0.dev8/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      622 2024-05-12 20:02:13.000000 torch_model_manager-0.3.0.dev8/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-12 20:02:13.000000 torch_model_manager-0.3.0.dev8/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      116 2024-05-12 20:02:13.000000 torch_model_manager-0.3.0.dev8/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-12 20:02:13.000000 torch_model_manager-0.3.0.dev8/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 20:02:13.289305 torch_model_manager-0.3.0.dev8/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev8/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8619 2024-05-09 19:01:45.000000 torch_model_manager-0.3.0.dev8/utils/helpers.py
```

### Comparing `torch_model_manager-0.3.0.dev7/PKG-INFO` & `torch_model_manager-0.3.0.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.3.0.dev7
+Version: 0.3.0.dev8
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.3.0.dev7/README.md` & `torch_model_manager-0.3.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev7/setup.py` & `torch_model_manager-0.3.0.dev8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.3.0.dev7',
+    version='0.3.0.dev8',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.3.0.dev7/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.3.0.dev8/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev7/tests/test_utils/test_helpers.py` & `torch_model_manager-0.3.0.dev8/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev7/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.3.0.dev8/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev7/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.3.0.dev8/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev7/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.3.0.dev8/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev7/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.3.0.dev8/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev7/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.3.0.dev8/torch_model_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.3.0.dev7
+Version: 0.3.0.dev8
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.3.0.dev7/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.3.0.dev8/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev7/utils/helpers.py` & `torch_model_manager-0.3.0.dev8/utils/helpers.py`

 * *Files identical despite different names*

