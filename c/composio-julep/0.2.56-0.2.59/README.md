# Comparing `tmp/composio_julep-0.2.56.tar.gz` & `tmp/composio_julep-0.2.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_julep-0.2.56.tar", last modified: Fri May 10 21:15:28 2024, max compression
+gzip compressed data, was "composio_julep-0.2.59.tar", last modified: Mon May 13 09:47:55 2024, max compression
```

## Comparing `composio_julep-0.2.56.tar` & `composio_julep-0.2.59.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 21:15:28.371386 composio_julep-0.2.56/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     4463 2024-05-10 21:15:28.371164 composio_julep-0.2.56/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3933 2024-05-09 11:39:51.000000 composio_julep-0.2.56/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 21:15:28.369855 composio_julep-0.2.56/composio_julep/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      157 2024-05-09 11:39:51.000000 composio_julep-0.2.56/composio_julep/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1619 2024-05-09 11:39:51.000000 composio_julep-0.2.56/composio_julep/julep_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 21:15:28.370894 composio_julep-0.2.56/composio_julep.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     4463 2024-05-10 21:15:28.000000 composio_julep-0.2.56/composio_julep.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      267 2024-05-10 21:15:28.000000 composio_julep-0.2.56/composio_julep.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-05-10 21:15:28.000000 composio_julep-0.2.56/composio_julep.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-10 21:15:28.000000 composio_julep-0.2.56/composio_julep.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       15 2024-05-10 21:15:28.000000 composio_julep-0.2.56/composio_julep.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-10 21:15:28.371443 composio_julep-0.2.56/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      842 2024-05-10 21:13:18.000000 composio_julep-0.2.56/setup.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-13 09:47:55.932307 composio_julep-0.2.59/
+-rw-r--r--   0 sawradip   (501) staff       (20)     4463 2024-05-13 09:47:55.932092 composio_julep-0.2.59/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)     3933 2024-05-02 07:57:45.000000 composio_julep-0.2.59/README.md
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-13 09:47:55.930904 composio_julep-0.2.59/composio_julep/
+-rw-r--r--   0 sawradip   (501) staff       (20)      157 2024-05-02 07:57:45.000000 composio_julep-0.2.59/composio_julep/__init__.py
+-rw-r--r--   0 sawradip   (501) staff       (20)     1619 2024-05-02 07:57:45.000000 composio_julep-0.2.59/composio_julep/julep_toolspec.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-13 09:47:55.931799 composio_julep-0.2.59/composio_julep.egg-info/
+-rw-r--r--   0 sawradip   (501) staff       (20)     4463 2024-05-13 09:47:55.000000 composio_julep-0.2.59/composio_julep.egg-info/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)      267 2024-05-13 09:47:55.000000 composio_julep-0.2.59/composio_julep.egg-info/SOURCES.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-13 09:47:55.000000 composio_julep-0.2.59/composio_julep.egg-info/dependency_links.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-13 09:47:55.000000 composio_julep-0.2.59/composio_julep.egg-info/requires.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       15 2024-05-13 09:47:55.000000 composio_julep-0.2.59/composio_julep.egg-info/top_level.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-13 09:47:55.932346 composio_julep-0.2.59/setup.cfg
+-rw-r--r--   0 sawradip   (501) staff       (20)      842 2024-05-13 09:47:44.000000 composio_julep-0.2.59/setup.py
```

### Comparing `composio_julep-0.2.56/PKG-INFO` & `composio_julep-0.2.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.56
+Version: 0.2.59
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.56
+Requires-Dist: composio_openai===0.2.59
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.56/README.md` & `composio_julep-0.2.59/README.md`

 * *Files identical despite different names*

### Comparing `composio_julep-0.2.56/composio_julep/julep_toolspec.py` & `composio_julep-0.2.59/composio_julep/julep_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_julep-0.2.56/composio_julep.egg-info/PKG-INFO` & `composio_julep-0.2.59/composio_julep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.56
+Version: 0.2.59
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.56
+Requires-Dist: composio_openai===0.2.59
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.56/setup.py` & `composio_julep-0.2.59/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_julep",
-    version="0.2.56",
+    version="0.2.59",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Julep wokflow.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
     install_requires=[
-        "composio_openai===0.2.56",
+        "composio_openai===0.2.59",
         "julep>=0.3.2"
     ],
     include_package_data=True,
 )
```

