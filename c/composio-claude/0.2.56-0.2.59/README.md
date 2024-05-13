# Comparing `tmp/composio_claude-0.2.56.tar.gz` & `tmp/composio_claude-0.2.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_claude-0.2.56.tar", last modified: Fri May 10 21:15:13 2024, max compression
+gzip compressed data, was "composio_claude-0.2.59.tar", last modified: Mon May 13 09:47:49 2024, max compression
```

## Comparing `composio_claude-0.2.56.tar` & `composio_claude-0.2.59.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 21:15:13.825150 composio_claude-0.2.56/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2561 2024-05-10 21:15:13.824925 composio_claude-0.2.56/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2027 2024-05-09 11:39:51.000000 composio_claude-0.2.56/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 21:15:13.823497 composio_claude-0.2.56/composio_claude/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      157 2024-05-09 11:39:51.000000 composio_claude-0.2.56/composio_claude/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1584 2024-05-09 11:39:51.000000 composio_claude-0.2.56/composio_claude/claude_toolset.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 21:15:13.824688 composio_claude-0.2.56/composio_claude.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2561 2024-05-10 21:15:13.000000 composio_claude-0.2.56/composio_claude.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      274 2024-05-10 21:15:13.000000 composio_claude-0.2.56/composio_claude.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-05-10 21:15:13.000000 composio_claude-0.2.56/composio_claude.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       43 2024-05-10 21:15:13.000000 composio_claude-0.2.56/composio_claude.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       16 2024-05-10 21:15:13.000000 composio_claude-0.2.56/composio_claude.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-10 21:15:13.825197 composio_claude-0.2.56/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      847 2024-05-10 21:13:18.000000 composio_claude-0.2.56/setup.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-13 09:47:49.707373 composio_claude-0.2.59/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2561 2024-05-13 09:47:49.707153 composio_claude-0.2.59/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)     2027 2024-05-13 07:27:09.000000 composio_claude-0.2.59/README.md
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-13 09:47:49.705507 composio_claude-0.2.59/composio_claude/
+-rw-r--r--   0 sawradip   (501) staff       (20)      157 2024-05-13 07:27:09.000000 composio_claude-0.2.59/composio_claude/__init__.py
+-rw-r--r--   0 sawradip   (501) staff       (20)     1584 2024-05-13 07:27:09.000000 composio_claude-0.2.59/composio_claude/claude_toolset.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-13 09:47:49.706858 composio_claude-0.2.59/composio_claude.egg-info/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2561 2024-05-13 09:47:49.000000 composio_claude-0.2.59/composio_claude.egg-info/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)      274 2024-05-13 09:47:49.000000 composio_claude-0.2.59/composio_claude.egg-info/SOURCES.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-13 09:47:49.000000 composio_claude-0.2.59/composio_claude.egg-info/dependency_links.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       43 2024-05-13 09:47:49.000000 composio_claude-0.2.59/composio_claude.egg-info/requires.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       16 2024-05-13 09:47:49.000000 composio_claude-0.2.59/composio_claude.egg-info/top_level.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-13 09:47:49.707414 composio_claude-0.2.59/setup.cfg
+-rw-r--r--   0 sawradip   (501) staff       (20)      847 2024-05-13 09:47:44.000000 composio_claude-0.2.59/setup.py
```

### Comparing `composio_claude-0.2.56/PKG-INFO` & `composio_claude-0.2.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_claude
-Version: 0.2.56
+Version: 0.2.59
 Summary: Use Composio to get an array of tools with your Claude LLMs.
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
 Requires-Dist: anthropic>=0.25.7
 
 ## 🚀🔗 Leveraging Claude with Composio
 
 Facilitate the integration of Claude with Composio to empower Claude models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_claude-0.2.56/README.md` & `composio_claude-0.2.59/README.md`

 * *Files identical despite different names*

### Comparing `composio_claude-0.2.56/composio_claude/claude_toolset.py` & `composio_claude-0.2.59/composio_claude/claude_toolset.py`

 * *Files identical despite different names*

### Comparing `composio_claude-0.2.56/composio_claude.egg-info/PKG-INFO` & `composio_claude-0.2.59/composio_claude.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_claude
-Version: 0.2.56
+Version: 0.2.59
 Summary: Use Composio to get an array of tools with your Claude LLMs.
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
 Requires-Dist: anthropic>=0.25.7
 
 ## 🚀🔗 Leveraging Claude with Composio
 
 Facilitate the integration of Claude with Composio to empower Claude models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_claude-0.2.56/setup.py` & `composio_claude-0.2.59/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_claude",
-    version="0.2.56",
+    version="0.2.59",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Claude LLMs.",
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
         "anthropic>=0.25.7"
     ],
     include_package_data=True,
 )
```

