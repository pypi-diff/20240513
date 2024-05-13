# Comparing `tmp/bigjpg-1.1.0.tar.gz` & `tmp/bigjpg-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigjpg-1.1.0.tar", last modified: Wed Feb 14 19:54:15 2024, max compression
+gzip compressed data, was "bigjpg-1.2.0.tar", last modified: Mon May 13 20:14:39 2024, max compression
```

## Comparing `bigjpg-1.1.0.tar` & `bigjpg-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-14 19:54:15.053461 bigjpg-1.1.0/
--rw-rw-rw-   0        0        0      970 2024-02-14 19:54:15.047457 bigjpg-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      723 2024-02-14 19:48:47.000000 bigjpg-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-14 19:54:14.966454 bigjpg-1.1.0/bigjpg/
--rw-rw-rw-   0        0        0      145 2024-02-14 19:47:25.000000 bigjpg-1.1.0/bigjpg/__init__.py
--rw-rw-rw-   0        0        0     2992 2024-02-14 19:49:39.000000 bigjpg-1.1.0/bigjpg/enlarger.py
-drwxrwxrwx   0        0        0        0 2024-02-14 19:54:15.042456 bigjpg-1.1.0/bigjpg/types/
--rw-rw-rw-   0        0        0       81 2024-02-14 19:46:18.000000 bigjpg-1.1.0/bigjpg/types/enlarge_values.py
--rw-rw-rw-   0        0        0       99 2024-02-14 19:45:56.000000 bigjpg-1.1.0/bigjpg/types/noises.py
--rw-rw-rw-   0        0        0       51 2024-02-14 19:46:35.000000 bigjpg-1.1.0/bigjpg/types/styles.py
-drwxrwxrwx   0        0        0        0 2024-02-14 19:54:15.029457 bigjpg-1.1.0/bigjpg.egg-info/
--rw-rw-rw-   0        0        0      970 2024-02-14 19:54:14.000000 bigjpg-1.1.0/bigjpg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2024-02-14 19:54:14.000000 bigjpg-1.1.0/bigjpg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-14 19:54:14.000000 bigjpg-1.1.0/bigjpg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-02-14 19:54:14.000000 bigjpg-1.1.0/bigjpg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-02-14 19:54:14.000000 bigjpg-1.1.0/bigjpg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-14 19:54:15.053461 bigjpg-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      543 2024-02-14 19:51:23.000000 bigjpg-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:14:39.549769 bigjpg-1.2.0/
+-rw-rw-rw-   0        0        0     1037 2024-05-13 20:14:39.545768 bigjpg-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2024-02-14 19:48:47.000000 bigjpg-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 20:14:39.468576 bigjpg-1.2.0/bigjpg/
+-rw-rw-rw-   0        0        0      145 2024-02-14 19:47:25.000000 bigjpg-1.2.0/bigjpg/__init__.py
+-rw-rw-rw-   0        0        0     3247 2024-05-13 20:12:56.000000 bigjpg-1.2.0/bigjpg/enlarger.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:14:39.537767 bigjpg-1.2.0/bigjpg/types/
+-rw-rw-rw-   0        0        0       81 2024-02-14 19:46:18.000000 bigjpg-1.2.0/bigjpg/types/enlarge_values.py
+-rw-rw-rw-   0        0        0       99 2024-02-14 19:45:56.000000 bigjpg-1.2.0/bigjpg/types/noises.py
+-rw-rw-rw-   0        0        0       51 2024-02-14 19:46:35.000000 bigjpg-1.2.0/bigjpg/types/styles.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:14:39.543767 bigjpg-1.2.0/bigjpg.egg-info/
+-rw-rw-rw-   0        0        0     1037 2024-05-13 20:14:38.000000 bigjpg-1.2.0/bigjpg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-13 20:14:38.000000 bigjpg-1.2.0/bigjpg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 20:14:38.000000 bigjpg-1.2.0/bigjpg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-13 20:14:38.000000 bigjpg-1.2.0/bigjpg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-13 20:14:38.000000 bigjpg-1.2.0/bigjpg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 20:14:39.549769 bigjpg-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      547 2024-05-13 20:05:17.000000 bigjpg-1.2.0/setup.py
```

### Comparing `bigjpg-1.1.0/README.md` & `bigjpg-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bigjpg-1.1.0/bigjpg/enlarger.py` & `bigjpg-1.2.0/bigjpg/enlarger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from urllib.request import urlretrieve
 from pydantic import validate_call
+from typing import Any
 from rich import print
 import httpx
 import json
 import time
 
 base_url = "https://bigjpg.com/api"
 
 class BigjpgError(Exception): ...
 
 class BigjpgImage:
     @validate_call
-    def __init__(self, image_url: str) -> None:
-        self._image_url = image_url
+    def __init__(self, image_url: str, file_extension: str) -> None:
+        self._image_url = image_url.replace("?x-oss-process=image/format,jpg&big.jpg", f"?x-oss-process=image/format,{file_extension}&big.{file_extension}")
 
     def get_url(self) -> str:
         return self._image_url
 
     @validate_call
     def download(self, out_path: str) -> None:
         urlretrieve(self._image_url, out_path)
 
 class BigjpgTask:
     @validate_call
     def __init__(self, url: str, task_id: str) -> None:
         self._url = url
         self._task_id = task_id
 
-    def fetch_util_achieve_the_result(self):
+    def fetch_util_achieve_the_result(self, interval: float = .5) -> Any:
         print(f"> [green][b][Bigjpg-info][/b][/green] [yellow]Waiting for image processing...[/yellow]")
 
         while True:
             response = httpx.get(self._url)
             json_response = response.json()
 
             data = json_response[self._task_id]
@@ -40,28 +41,29 @@
 
             if status == "success":
                 return data
 
             elif status == "error":
                 raise BigjpgError("Error processing the image!")
 
-            time.sleep(.5)
+            time.sleep(interval)
 
 class Bigjpg:
     @validate_call
     def __init__(self, api_token: str) -> None:
         self._api_token = api_token
 
     @validate_call
     def enlarge(
         self,
         style: str,
         noise: str,
         enlarge_value: str,
-        image_url: str
+        image_url: str,
+        file_extension: str = "png"
     ) -> BigjpgImage:
 
         url = f"{base_url}/task/"
         config = {
             "style": style,
             "noise": noise,
             "x2": enlarge_value,
@@ -89,10 +91,10 @@
 
         task_id = json_response["tid"]
         task_url = f"{base_url}/task/{task_id}"
         task = BigjpgTask(task_url, task_id)
         task_result = task.fetch_util_achieve_the_result()
         
         image_url = task_result["url"]
-        image = BigjpgImage(image_url)
+        image = BigjpgImage(image_url, file_extension)
 
         return image
```

### Comparing `bigjpg-1.1.0/setup.py` & `bigjpg-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 with open("README.md", "r") as file:
     readme_content = file.read()
 
 setup(
     name = "bigjpg",
-    version = "1.1.0",
+    version = "1.2.0",
     license = "MIT License",
     author = "Marcuth",
     long_description = readme_content,
     long_description_content_type = "text/markdown",
-    author_email = "marcuth2006@gmail.com",
+    author_email = "example@gmail.com",
     keywords = "bigjpg wrapper api",
     description = f"Wrappper for https://bigjpg.com/",
     packages = ["bigjpg", "bigjpg/types"],
-    install_requires = ["requests", "pydantic"],
+    install_requires = ["requests", "pydantic", "rich"],
 )
```

