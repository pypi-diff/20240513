# Comparing `tmp/loopquest-0.2.4.tar.gz` & `tmp/loopquest-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopquest-0.2.4.tar", last modified: Sat May 11 19:47:33 2024, max compression
+gzip compressed data, was "loopquest-0.2.5.tar", last modified: Mon May 13 19:19:58 2024, max compression
```

## Comparing `loopquest-0.2.4.tar` & `loopquest-0.2.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-11 19:47:33.693883 loopquest-0.2.4/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.4/LICENSE
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-11 19:47:33.693883 loopquest-0.2.4/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5418 2024-04-29 17:12:15.000000 loopquest-0.2.4/README.md
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-11 19:47:33.665883 loopquest-0.2.4/loopquest/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.4/loopquest/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1517 2024-05-08 05:44:07.000000 loopquest-0.2.4/loopquest/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9495 2024-05-08 05:56:32.000000 loopquest-0.2.4/loopquest/crud.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1933 2024-04-19 04:43:26.000000 loopquest-0.2.4/loopquest/datasets.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-11 19:47:33.673883 loopquest-0.2.4/loopquest/env/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.4/loopquest/env/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4768 2024-05-08 06:15:15.000000 loopquest-0.2.4/loopquest/env/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6492 2024-05-11 19:42:13.000000 loopquest-0.2.4/loopquest/env/gym_wrappers.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.4/loopquest/env/space_utils.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6293 2024-05-10 17:45:41.000000 loopquest-0.2.4/loopquest/eval.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-11 19:47:33.673883 loopquest-0.2.4/loopquest/policy/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.4/loopquest/policy/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      321 2024-05-08 05:05:33.000000 loopquest-0.2.4/loopquest/policy/base.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.4/loopquest/policy/sb3_policy.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     2001 2024-05-03 04:41:02.000000 loopquest-0.2.4/loopquest/private_api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5717 2024-05-09 02:52:37.000000 loopquest-0.2.4/loopquest/schema.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.4/loopquest/typing.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.4/loopquest/ui.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4740 2024-05-03 05:20:31.000000 loopquest-0.2.4/loopquest/utils.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-11 19:47:33.673883 loopquest-0.2.4/loopquest.egg-info/
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-11 19:47:33.000000 loopquest-0.2.4/loopquest.egg-info/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-11 19:47:33.000000 loopquest-0.2.4/loopquest.egg-info/SOURCES.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-11 19:47:33.000000 loopquest-0.2.4/loopquest.egg-info/dependency_links.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-11 19:47:33.000000 loopquest-0.2.4/loopquest.egg-info/requires.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-11 19:47:33.000000 loopquest-0.2.4/loopquest.egg-info/top_level.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-11 19:47:33.693883 loopquest-0.2.4/setup.cfg
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-11 19:46:30.000000 loopquest-0.2.4/setup.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-13 19:19:58.233238 loopquest-0.2.5/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.5/LICENSE
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-13 19:19:58.233238 loopquest-0.2.5/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5418 2024-04-29 17:12:15.000000 loopquest-0.2.5/README.md
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-13 19:19:58.233238 loopquest-0.2.5/loopquest/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.5/loopquest/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1517 2024-05-08 05:44:07.000000 loopquest-0.2.5/loopquest/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9495 2024-05-08 05:56:32.000000 loopquest-0.2.5/loopquest/crud.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1933 2024-04-19 04:43:26.000000 loopquest-0.2.5/loopquest/datasets.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-13 19:19:58.233238 loopquest-0.2.5/loopquest/env/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.5/loopquest/env/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4768 2024-05-08 06:15:15.000000 loopquest-0.2.5/loopquest/env/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6492 2024-05-11 19:42:13.000000 loopquest-0.2.5/loopquest/env/gym_wrappers.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.5/loopquest/env/space_utils.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6293 2024-05-10 17:45:41.000000 loopquest-0.2.5/loopquest/eval.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-13 19:19:58.233238 loopquest-0.2.5/loopquest/policy/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.5/loopquest/policy/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      321 2024-05-08 05:05:33.000000 loopquest-0.2.5/loopquest/policy/base.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.5/loopquest/policy/sb3_policy.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     2001 2024-05-03 04:41:02.000000 loopquest-0.2.5/loopquest/private_api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5798 2024-05-13 18:34:45.000000 loopquest-0.2.5/loopquest/schema.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.5/loopquest/typing.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.5/loopquest/ui.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4740 2024-05-03 05:20:31.000000 loopquest-0.2.5/loopquest/utils.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-13 19:19:58.233238 loopquest-0.2.5/loopquest.egg-info/
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-13 19:19:58.000000 loopquest-0.2.5/loopquest.egg-info/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-13 19:19:58.000000 loopquest-0.2.5/loopquest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-13 19:19:58.000000 loopquest-0.2.5/loopquest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-13 19:19:58.000000 loopquest-0.2.5/loopquest.egg-info/requires.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-13 19:19:58.000000 loopquest-0.2.5/loopquest.egg-info/top_level.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-13 19:19:58.233238 loopquest-0.2.5/setup.cfg
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-13 19:18:30.000000 loopquest-0.2.5/setup.py
```

### Comparing `loopquest-0.2.4/LICENSE` & `loopquest-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/PKG-INFO` & `loopquest-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `loopquest-0.2.4/README.md` & `loopquest-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/loopquest/api.py` & `loopquest-0.2.5/loopquest/api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/loopquest/crud.py` & `loopquest-0.2.5/loopquest/crud.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/loopquest/datasets.py` & `loopquest-0.2.5/loopquest/datasets.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/loopquest/env/api.py` & `loopquest-0.2.5/loopquest/env/api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/loopquest/env/gym_wrappers.py` & `loopquest-0.2.5/loopquest/env/gym_wrappers.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/loopquest/env/space_utils.py` & `loopquest-0.2.5/loopquest/env/space_utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/loopquest/eval.py` & `loopquest-0.2.5/loopquest/eval.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/loopquest/policy/sb3_policy.py` & `loopquest-0.2.5/loopquest/policy/sb3_policy.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/loopquest/private_api.py` & `loopquest-0.2.5/loopquest/private_api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/loopquest/schema.py` & `loopquest-0.2.5/loopquest/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,16 @@
     image_urls: Optional[List[str]] = []
     termnated: Optional[bool] = False
     truncated: Optional[bool] = False
     # This is deprecated by Gymnasium, but we still keep it for backward
     # compatibility.
     done: Optional[bool] = False
     info: Optional[Dict[str, Any]] = None  # JSON string of step info
+    human_score: Optional[int] = None
+    human_annotation: Optional[str] = None
 
 
 class Step(StepCreate):
     id: str
     creation_time: datetime.datetime
     update_time: Optional[datetime.datetime] = None
```

### Comparing `loopquest-0.2.4/loopquest/utils.py` & `loopquest-0.2.5/loopquest/utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/loopquest.egg-info/PKG-INFO` & `loopquest-0.2.5/loopquest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `loopquest-0.2.4/loopquest.egg-info/SOURCES.txt` & `loopquest-0.2.5/loopquest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.4/setup.py` & `loopquest-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="loopquest",
-    version="0.2.4",
+    version="0.2.5",
     description="A Production Tool for Embodied AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="LoopMind",
     author_email="contactus@loopmind.ai",
     url="https://github.com/LoopMind-AI/loopquest",
     packages=find_packages(),
```

