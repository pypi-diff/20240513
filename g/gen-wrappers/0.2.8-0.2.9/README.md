# Comparing `tmp/gen_wrappers-0.2.8.tar.gz` & `tmp/gen_wrappers-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.2.8.tar", last modified: Sat May 11 17:04:32 2024, max compression
+gzip compressed data, was "gen_wrappers-0.2.9.tar", last modified: Mon May 13 17:49:11 2024, max compression
```

## Comparing `gen_wrappers-0.2.8.tar` & `gen_wrappers-0.2.9.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 17:04:32.151651 gen_wrappers-0.2.8/
--rw-rw-rw-   0        0        0      847 2024-05-11 17:04:32.147841 gen_wrappers-0.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 17:04:31.997471 gen_wrappers-0.2.8/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.8/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 17:04:32.027187 gen_wrappers-0.2.8/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.8/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     6625 2024-05-11 17:01:23.000000 gen_wrappers-0.2.8/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.2.8/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.2.8/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-11 17:04:32.054503 gen_wrappers-0.2.8/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.8/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.2.8/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.8/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3195 2024-05-11 16:54:43.000000 gen_wrappers-0.2.8/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.8/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-11 17:04:32.070832 gen_wrappers-0.2.8/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.8/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9561 2024-05-11 17:02:29.000000 gen_wrappers-0.2.8/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     9193 2024-05-11 14:41:07.000000 gen_wrappers-0.2.8/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.8/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-11 17:04:32.085591 gen_wrappers-0.2.8/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.8/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6345 2024-05-11 17:04:12.000000 gen_wrappers-0.2.8/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.2.8/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.8/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-11 17:04:32.144143 gen_wrappers-0.2.8/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-11 17:04:31.000000 gen_wrappers-0.2.8/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-11 17:04:31.000000 gen_wrappers-0.2.8/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 17:04:31.000000 gen_wrappers-0.2.8/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-11 17:04:31.000000 gen_wrappers-0.2.8/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-11 17:04:31.000000 gen_wrappers-0.2.8/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 17:04:32.152649 gen_wrappers-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-11 17:04:28.000000 gen_wrappers-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.220266 gen_wrappers-0.2.9/
+-rw-rw-rw-   0        0        0      847 2024-05-13 17:49:11.218266 gen_wrappers-0.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.187699 gen_wrappers-0.2.9/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.9/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.192723 gen_wrappers-0.2.9/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.9/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     6625 2024-05-11 17:01:23.000000 gen_wrappers-0.2.9/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.2.9/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.2.9/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.198221 gen_wrappers-0.2.9/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.9/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.2.9/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.9/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.2.9/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.9/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.201220 gen_wrappers-0.2.9/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.9/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9561 2024-05-11 17:02:29.000000 gen_wrappers-0.2.9/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     9193 2024-05-11 14:41:07.000000 gen_wrappers-0.2.9/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.9/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.206223 gen_wrappers-0.2.9/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.9/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6345 2024-05-11 17:04:12.000000 gen_wrappers-0.2.9/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.2.9/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.9/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.208226 gen_wrappers-0.2.9/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.2.9/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     6092 2024-05-13 17:06:45.000000 gen_wrappers-0.2.9/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.216257 gen_wrappers-0.2.9/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-13 17:49:11.000000 gen_wrappers-0.2.9/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-13 17:49:11.000000 gen_wrappers-0.2.9/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 17:49:11.000000 gen_wrappers-0.2.9/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-13 17:49:11.000000 gen_wrappers-0.2.9/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 17:49:11.000000 gen_wrappers-0.2.9/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 17:49:11.220266 gen_wrappers-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-13 17:47:33.000000 gen_wrappers-0.2.9/setup.py
```

### Comparing `gen_wrappers-0.2.8/PKG-INFO` & `gen_wrappers-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.2.8
+Version: 0.2.9
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.2.8/creator/auto/creator_auto.py` & `gen_wrappers-0.2.9/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.8/creator/auto/request_auto.py` & `gen_wrappers-0.2.9/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.8/creator/auto/response_auto.py` & `gen_wrappers-0.2.9/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.8/creator/base/base_app.py` & `gen_wrappers-0.2.9/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.8/creator/base/base_request.py` & `gen_wrappers-0.2.9/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.8/creator/base/base_response.py` & `gen_wrappers-0.2.9/creator/base/base_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import base64
 from enum import Enum
 from typing import List, Optional, Any
 from fastapi.responses import Response
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from creator.base.job_status import JobStatus
 
 
 class ResponseDataType(str, Enum):
     IMAGE = "image"
     VIDEO = "video"
     TEXT = "text"
     AUDIO = "audio"
+    NONE = "none"
 
 
 class ResponseData(BaseModel):
-    data: List[Any]
-    data_type: ResponseDataType
-    total_count: int
+    data: List[Any] = Field(default_factory=list, description="The data to be returned.")
+    data_type: ResponseDataType = Field(ResponseDataType.NONE, description="The type of data being returned.")
+    total_count: int = 0
 
 
 class BaseResponse(BaseModel):
     status: JobStatus = JobStatus.PENDING
     output: Optional[ResponseData] = None
     error_msg: Optional[str] = None
     job_id: Optional[str] = None
```

### Comparing `gen_wrappers-0.2.8/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.2.9/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.8/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.2.9/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.8/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.2.9/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.8/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.2.9/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.8/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.2.9/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.8/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.2.9/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.2.8
+Version: 0.2.9
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.2.8/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.2.9/gen_wrappers.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,12 +13,14 @@
 creator/cmfy/creator_cmfy.py
 creator/cmfy/request_cmfy.py
 creator/cmfy/response_cmfy.py
 creator/fcus_api/__init__.py
 creator/fcus_api/creator_fcus_api.py
 creator/fcus_api/request_fcus_api.py
 creator/fcus_api/response_fcus_api.py
+creator/util/__init__.py
+creator/util/helper.py
 gen_wrappers.egg-info/PKG-INFO
 gen_wrappers.egg-info/SOURCES.txt
 gen_wrappers.egg-info/dependency_links.txt
 gen_wrappers.egg-info/requires.txt
 gen_wrappers.egg-info/top_level.txt
```

### Comparing `gen_wrappers-0.2.8/setup.py` & `gen_wrappers-0.2.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.2.8',
+    version='0.2.9',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

