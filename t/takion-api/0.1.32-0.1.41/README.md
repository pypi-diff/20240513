# Comparing `tmp/takion_api-0.1.32.tar.gz` & `tmp/takion_api-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "takion_api-0.1.32.tar", last modified: Tue Jan 23 01:25:22 2024, max compression
+gzip compressed data, was "takion_api-0.1.41.tar", last modified: Mon May 13 15:02:58 2024, max compression
```

## Comparing `takion_api-0.1.32.tar` & `takion_api-0.1.41.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-01-23 01:25:22.643430 takion_api-0.1.32/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1071 2023-12-12 15:45:49.000000 takion_api-0.1.32/LICENSE
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)    15272 2024-01-23 01:25:22.643095 takion_api-0.1.32/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)    14475 2024-01-22 16:13:02.000000 takion_api-0.1.32/README.md
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2024-01-23 01:25:22.643492 takion_api-0.1.32/setup.cfg
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      930 2024-01-23 01:25:20.000000 takion_api-0.1.32/setup.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-01-23 01:25:22.639763 takion_api-0.1.32/takion_api/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      377 2024-01-22 15:55:32.000000 takion_api-0.1.32/takion_api/__init__.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-01-23 01:25:22.641702 takion_api-0.1.32/takion_api/datadome/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       35 2024-01-22 15:36:31.000000 takion_api-0.1.32/takion_api/datadome/__init__.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     7965 2024-01-22 16:04:50.000000 takion_api-0.1.32/takion_api/datadome/main.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      439 2023-12-12 13:33:24.000000 takion_api-0.1.32/takion_api/exceptions.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-01-23 01:25:22.642542 takion_api-0.1.32/takion_api/incapsula/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       71 2024-01-22 15:55:23.000000 takion_api-0.1.32/takion_api/incapsula/__init__.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     9472 2024-01-23 01:24:49.000000 takion_api-0.1.32/takion_api/incapsula/reese84.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5152 2024-01-22 16:04:40.000000 takion_api-0.1.32/takion_api/incapsula/utmvc.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      254 2024-01-23 01:17:39.000000 takion_api-0.1.32/takion_api/models.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-01-23 01:25:22.641150 takion_api-0.1.32/takion_api.egg-info/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)    15272 2024-01-23 01:25:22.000000 takion_api-0.1.32/takion_api.egg-info/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      419 2024-01-23 01:25:22.000000 takion_api-0.1.32/takion_api.egg-info/SOURCES.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2024-01-23 01:25:22.000000 takion_api-0.1.32/takion_api.egg-info/dependency_links.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      106 2024-01-23 01:25:22.000000 takion_api-0.1.32/takion_api.egg-info/requires.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       11 2024-01-23 01:25:22.000000 takion_api-0.1.32/takion_api.egg-info/top_level.txt
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-05-13 15:02:58.799634 takion_api-0.1.41/
+-rw-------   0 glizzykingdreko   (501) staff       (20)     1071 2023-12-12 15:45:49.000000 takion_api-0.1.41/LICENSE
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)    15272 2024-05-13 15:02:58.799070 takion_api-0.1.41/PKG-INFO
+-rw-------   0 glizzykingdreko   (501) staff       (20)    14475 2024-01-30 22:40:57.000000 takion_api-0.1.41/README.md
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2024-05-13 15:02:58.799729 takion_api-0.1.41/setup.cfg
+-rw-------   0 glizzykingdreko   (501) staff       (20)      930 2024-05-13 14:47:10.000000 takion_api-0.1.41/setup.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-05-13 15:02:58.793381 takion_api-0.1.41/takion_api/
+-rw-------   0 glizzykingdreko   (501) staff       (20)      407 2024-01-30 22:43:06.000000 takion_api-0.1.41/takion_api/__init__.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-05-13 15:02:58.795889 takion_api-0.1.41/takion_api/datadome/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       35 2024-01-30 22:40:57.000000 takion_api-0.1.41/takion_api/datadome/__init__.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     8066 2024-05-13 14:46:53.000000 takion_api-0.1.41/takion_api/datadome/main.py
+-rw-------   0 glizzykingdreko   (501) staff       (20)      439 2023-12-12 13:33:24.000000 takion_api-0.1.41/takion_api/exceptions.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-05-13 15:02:58.797711 takion_api-0.1.41/takion_api/incapsula/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       71 2024-01-22 15:55:23.000000 takion_api-0.1.41/takion_api/incapsula/__init__.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     9538 2024-05-13 14:29:45.000000 takion_api-0.1.41/takion_api/incapsula/reese84.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5237 2024-05-13 14:29:21.000000 takion_api-0.1.41/takion_api/incapsula/utmvc.py
+-rw-------   0 glizzykingdreko   (501) staff       (20)      315 2024-01-30 22:42:25.000000 takion_api-0.1.41/takion_api/models.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2024-05-13 15:02:58.798433 takion_api-0.1.41/takion_api.egg-info/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)    15272 2024-05-13 15:02:58.000000 takion_api-0.1.41/takion_api.egg-info/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      419 2024-05-13 15:02:58.000000 takion_api-0.1.41/takion_api.egg-info/SOURCES.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2024-05-13 15:02:58.000000 takion_api-0.1.41/takion_api.egg-info/dependency_links.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      106 2024-05-13 15:02:58.000000 takion_api-0.1.41/takion_api.egg-info/requires.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       11 2024-05-13 15:02:58.000000 takion_api-0.1.41/takion_api.egg-info/top_level.txt
```

### Comparing `takion_api-0.1.32/LICENSE` & `takion_api-0.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `takion_api-0.1.32/PKG-INFO` & `takion_api-0.1.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: takion_api
-Version: 0.1.32
+Version: 0.1.41
 Summary: Official Python wrapper for TakionAPI services, designed for efficient automation and bypass of advanced antibot systems.
 Home-page: https://github.com/Takion-API-Services/takion-api
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 Keywords: takion-api,takion,datadome,antibot,bypass
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `takion_api-0.1.32/README.md` & `takion_api-0.1.41/README.md`

 * *Files identical despite different names*

### Comparing `takion_api-0.1.32/setup.py` & `takion_api-0.1.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='takion_api',
-    version='0.1.32',
+    version='0.1.41',
     packages=find_packages(),
     install_requires=[
         line.strip() for line in open("requirements.txt", "r").readlines()
     ],
     author='glizzykingdreko',
     author_email='glizzykingdreko@protonmail.com',
     description='Official Python wrapper for TakionAPI services, designed for efficient automation and bypass of advanced antibot systems.',
```

### Comparing `takion_api-0.1.32/takion_api/datadome/main.py` & `takion_api-0.1.41/takion_api/datadome/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from requests import post
 from requests.models import Response
 from typing import Optional, Dict
 
 from ..exceptions import BadResponseException, IpBanException
 from ..models import CookieRequest
+from ..models import TakionAPI
 
-class TakionAPIDatadome:
-    BASE_URL = "https://takionapi.tech/datadome/{}?api_key={}"
+class TakionAPIDatadome(TakionAPI):
+    BASE_URL = "{}/{}?api_key={}"
+    DOMAIN: "datadome.takionapi.tech"
     api_key: str
     challenge_type: Optional[str]
 
     @staticmethod
     def is_challenge(response: Response) -> bool:
         """
         # Got Flagged by Datadome?
@@ -135,15 +137,16 @@
 
         ### Raises
         - `BadResponseException`: If the challenge URL could not be parsed from the response
         '''
         try:
             res = post(
                 self.BASE_URL.format(
-                    "build-url",
+                    self.DOMAIN,
+                    "build",
                     self.api_key,
                 ),
                 json={
                     "html": response.text,
                     "cid": cookie,
                     "referrer": url,
                 },
@@ -189,15 +192,16 @@
             raise ValueError("Challenge type not set")
         elif not self.challenge_type and challenge_type in ["interstitial", "geetest"]:
             self.challenge_type = challenge_type
         
         try:
             res = post(
                 self.BASE_URL.format(
-                    self.challenge_type,
+                    self.DOMAIN,
+                    "solve",
                     self.api_key,
                 ),
                 json={
                     "html": response.text,
                 },
                 headers={
                     "User-Agent": user_agent,
```

### Comparing `takion_api-0.1.32/takion_api/incapsula/reese84.py` & `takion_api-0.1.41/takion_api/incapsula/reese84.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from requests import get, post
 from requests.models import Response
 from typing import Optional, Dict
 from json import dumps
 
 from ..exceptions import BadResponseException
-from ..models import CookieRequest, IncapsulaGeeTest
+from ..models import CookieRequest, IncapsulaGeeTest, TakionAPI
 
-class TakionAPIReese84:
-    BASE_URL = "https://takionapi.tech/incapsula/payload/{}?api_key={}"
+class TakionAPIReese84(TakionAPI):
+    BASE_URL = "{}/incapsula{}?api_key={}"
+    DOMAIN = "incapsula.takionapi.tech"
     api_key: str
 
     @staticmethod
     def is_challenge(response: Response) -> bool:
         """
         # Reese84 cookie needed?
         ## Check if the response has been blocked by Incapsula
@@ -215,14 +216,15 @@
 
         ### Raises
         - `BadResponseException`: If the challenge could not be solved
         '''
         try:
             res = get(
                 self.BASE_URL.format(
+                    self.DOMAIN,
                     website_domain,
                     self.api_key,
                 ),
                 headers={
                     "User-Agent": user_agent,
                 }
             ).json()
```

### Comparing `takion_api-0.1.32/takion_api/incapsula/utmvc.py` & `takion_api-0.1.41/takion_api/incapsula/utmvc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from requests import post, get
 from requests.models import Response
 from requests.cookies import RequestsCookieJar
 from re import search
 from typing import Optional, Union
 
 from ..exceptions import BadResponseException
+from ..models import TakionAPI
 
-class TakionAPIUtmvc:
-    BASE_URL = "https://takionapi.tech/incapsula/utmvc?api_key={}"
+class TakionAPIUtmvc(TakionAPI):
+    BASE_URL = "{}/utmvc?api_key={}"
+    DOMAIN = "incapsula.takionapi.tech"
     api_key: str
 
     @staticmethod
     def is_challenge(response: Response) -> Union[bool, str]:
         """
         # Utmvc cookie needed?
         ## Check if the response has the utmvc script in it
@@ -123,14 +125,15 @@
         if not self.challenge_url:
             return False
         
         content = self.get_challenge_url(user_agent)
         try:
             res = post(
                 self.BASE_URL.format(
+                    self.DOMAIN,
                     self.api_key,
                 ),
                 json={
                     "content": content,
                     "cookies": [[name, value] for name, value in cookies.items()]
                 },
                 headers={
```

### Comparing `takion_api-0.1.32/takion_api.egg-info/PKG-INFO` & `takion_api-0.1.41/takion_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: takion-api
-Version: 0.1.32
+Name: takion_api
+Version: 0.1.41
 Summary: Official Python wrapper for TakionAPI services, designed for efficient automation and bypass of advanced antibot systems.
 Home-page: https://github.com/Takion-API-Services/takion-api
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 Keywords: takion-api,takion,datadome,antibot,bypass
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

