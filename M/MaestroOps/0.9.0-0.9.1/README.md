# Comparing `tmp/maestroops-0.9.0.tar.gz` & `tmp/maestroops-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestroops-0.9.0.tar", last modified: Tue Apr 23 19:15:35 2024, max compression
+gzip compressed data, was "maestroops-0.9.1.tar", last modified: Mon May 13 13:51:56 2024, max compression
```

## Comparing `maestroops-0.9.0.tar` & `maestroops-0.9.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.844902 maestroops-0.9.0/
--rw-r--r--   0 mperttula   (502) staff       (20)     1081 2024-02-27 16:30:05.000000 maestroops-0.9.0/LICENSE
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.842962 maestroops-0.9.0/MaestroOps.egg-info/
--rw-r--r--   0 mperttula   (502) staff       (20)      285 2024-04-23 19:15:35.000000 maestroops-0.9.0/MaestroOps.egg-info/PKG-INFO
--rw-r--r--   0 mperttula   (502) staff       (20)      648 2024-04-23 19:15:35.000000 maestroops-0.9.0/MaestroOps.egg-info/SOURCES.txt
--rw-r--r--   0 mperttula   (502) staff       (20)        1 2024-04-23 19:15:35.000000 maestroops-0.9.0/MaestroOps.egg-info/dependency_links.txt
--rw-r--r--   0 mperttula   (502) staff       (20)       17 2024-04-23 19:15:35.000000 maestroops-0.9.0/MaestroOps.egg-info/requires.txt
--rw-r--r--   0 mperttula   (502) staff       (20)        8 2024-04-23 19:15:35.000000 maestroops-0.9.0/MaestroOps.egg-info/top_level.txt
--rw-r--r--   0 mperttula   (502) staff       (20)      285 2024-04-23 19:15:35.843952 maestroops-0.9.0/PKG-INFO
--rw-r--r--   0 mperttula   (502) staff       (20)      115 2024-02-27 16:30:05.000000 maestroops-0.9.0/README.md
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.671670 maestroops-0.9.0/maestro/
--rw-r--r--   0 mperttula   (502) staff       (20)       46 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/__init__.py
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.743088 maestroops-0.9.0/maestro/aws/
--rw-r--r--   0 mperttula   (502) staff       (20)       84 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/__init__.py
--rw-r--r--   0 mperttula   (502) staff       (20)    30006 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/cf_stack.py
--rw-r--r--   0 mperttula   (502) staff       (20)    20046 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/dynamodb.py
--rw-r--r--   0 mperttula   (502) staff       (20)     9237 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/parameter_store.py
--rw-r--r--   0 mperttula   (502) staff       (20)    11716 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/r53.py
--rw-r--r--   0 mperttula   (502) staff       (20)    13344 2024-04-23 19:13:16.000000 maestroops-0.9.0/maestro/aws/s3.py
--rw-r--r--   0 mperttula   (502) staff       (20)    10701 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/ssm_documents.py
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.785483 maestroops-0.9.0/maestro/core/
--rw-r--r--   0 mperttula   (502) staff       (20)       39 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/core/__init__.py
--rw-r--r--   0 mperttula   (502) staff       (20)     1487 2024-02-27 16:30:09.000000 maestroops-0.9.0/maestro/core/execute.py
--rw-r--r--   0 mperttula   (502) staff       (20)     2554 2024-02-27 16:30:09.000000 maestroops-0.9.0/maestro/core/ioc.py
--rw-r--r--   0 mperttula   (502) staff       (20)     4583 2024-02-27 16:30:09.000000 maestroops-0.9.0/maestro/core/module.py
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.799343 maestroops-0.9.0/maestro/jenkins/
--rw-r--r--   0 mperttula   (502) staff       (20)       19 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/jenkins/__init__.py
--rw-r--r--   0 mperttula   (502) staff       (20)     6683 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/jenkins/jobs.py
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.841928 maestroops-0.9.0/maestro/tools/
--rw-r--r--   0 mperttula   (502) staff       (20)       37 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/tools/__init__.py
--rw-r--r--   0 mperttula   (502) staff       (20)     1713 2024-04-23 19:13:16.000000 maestroops-0.9.0/maestro/tools/file.py
--rw-r--r--   0 mperttula   (502) staff       (20)      742 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/tools/os_tools.py
--rw-r--r--   0 mperttula   (502) staff       (20)     3425 2024-02-27 16:30:09.000000 maestroops-0.9.0/maestro/tools/path.py
--rw-r--r--   0 mperttula   (502) staff       (20)      423 2024-02-27 16:30:09.000000 maestroops-0.9.0/maestro/tools/string.py
--rw-r--r--   0 mperttula   (502) staff       (20)       38 2024-04-23 19:15:35.845073 maestroops-0.9.0/setup.cfg
--rw-r--r--   0 mperttula   (502) staff       (20)      424 2024-04-23 19:13:16.000000 maestroops-0.9.0/setup.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:51:56.047397 maestroops-0.9.1/
+-rw-r--r--   0 mperttula   (502) staff       (20)     1081 2024-02-27 16:30:05.000000 maestroops-0.9.1/LICENSE
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:51:56.045683 maestroops-0.9.1/MaestroOps.egg-info/
+-rw-r--r--   0 mperttula   (502) staff       (20)      290 2024-05-13 13:51:55.000000 maestroops-0.9.1/MaestroOps.egg-info/PKG-INFO
+-rw-r--r--   0 mperttula   (502) staff       (20)      648 2024-05-13 13:51:55.000000 maestroops-0.9.1/MaestroOps.egg-info/SOURCES.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)        1 2024-05-13 13:51:55.000000 maestroops-0.9.1/MaestroOps.egg-info/dependency_links.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)       22 2024-05-13 13:51:55.000000 maestroops-0.9.1/MaestroOps.egg-info/requires.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)        8 2024-05-13 13:51:55.000000 maestroops-0.9.1/MaestroOps.egg-info/top_level.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)      290 2024-05-13 13:51:56.046613 maestroops-0.9.1/PKG-INFO
+-rw-r--r--   0 mperttula   (502) staff       (20)      115 2024-02-27 16:30:05.000000 maestroops-0.9.1/README.md
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:51:55.755114 maestroops-0.9.1/maestro/
+-rw-r--r--   0 mperttula   (502) staff       (20)       46 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/__init__.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:51:55.892740 maestroops-0.9.1/maestro/aws/
+-rw-r--r--   0 mperttula   (502) staff       (20)       84 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/aws/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    30006 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/aws/cf_stack.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    20046 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/aws/dynamodb.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     9237 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/aws/parameter_store.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    11716 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/aws/r53.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    13344 2024-04-23 19:13:16.000000 maestroops-0.9.1/maestro/aws/s3.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    10701 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/aws/ssm_documents.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:51:55.945994 maestroops-0.9.1/maestro/core/
+-rw-r--r--   0 mperttula   (502) staff       (20)       39 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/core/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     1487 2024-02-27 16:30:09.000000 maestroops-0.9.1/maestro/core/execute.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     2554 2024-02-27 16:30:09.000000 maestroops-0.9.1/maestro/core/ioc.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     4583 2024-02-27 16:30:09.000000 maestroops-0.9.1/maestro/core/module.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:51:55.985995 maestroops-0.9.1/maestro/jenkins/
+-rw-r--r--   0 mperttula   (502) staff       (20)       19 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/jenkins/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     6683 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/jenkins/jobs.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:51:56.044589 maestroops-0.9.1/maestro/tools/
+-rw-r--r--   0 mperttula   (502) staff       (20)       37 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/tools/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     1713 2024-04-23 19:13:16.000000 maestroops-0.9.1/maestro/tools/file.py
+-rw-r--r--   0 mperttula   (502) staff       (20)      742 2024-02-27 16:30:05.000000 maestroops-0.9.1/maestro/tools/os_tools.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     3425 2024-02-27 16:30:09.000000 maestroops-0.9.1/maestro/tools/path.py
+-rw-r--r--   0 mperttula   (502) staff       (20)      423 2024-02-27 16:30:09.000000 maestroops-0.9.1/maestro/tools/string.py
+-rw-r--r--   0 mperttula   (502) staff       (20)       38 2024-05-13 13:51:56.047546 maestroops-0.9.1/setup.cfg
+-rw-r--r--   0 mperttula   (502) staff       (20)      429 2024-05-13 13:51:20.000000 maestroops-0.9.1/setup.py
```

### Comparing `maestroops-0.9.0/LICENSE` & `maestroops-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/MaestroOps.egg-info/SOURCES.txt` & `maestroops-0.9.1/MaestroOps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/aws/cf_stack.py` & `maestroops-0.9.1/maestro/aws/cf_stack.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/aws/dynamodb.py` & `maestroops-0.9.1/maestro/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/aws/parameter_store.py` & `maestroops-0.9.1/maestro/aws/parameter_store.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/aws/r53.py` & `maestroops-0.9.1/maestro/aws/r53.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/aws/s3.py` & `maestroops-0.9.1/maestro/aws/s3.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/aws/ssm_documents.py` & `maestroops-0.9.1/maestro/aws/ssm_documents.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/core/execute.py` & `maestroops-0.9.1/maestro/core/execute.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/core/ioc.py` & `maestroops-0.9.1/maestro/core/ioc.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/core/module.py` & `maestroops-0.9.1/maestro/core/module.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/jenkins/jobs.py` & `maestroops-0.9.1/maestro/jenkins/jobs.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/tools/file.py` & `maestroops-0.9.1/maestro/tools/file.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/tools/os_tools.py` & `maestroops-0.9.1/maestro/tools/os_tools.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.0/maestro/tools/path.py` & `maestroops-0.9.1/maestro/tools/path.py`

 * *Files identical despite different names*

