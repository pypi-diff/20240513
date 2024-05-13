# Comparing `tmp/velintegrator-1.1.4.tar.gz` & `tmp/velintegrator-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velintegrator-1.1.4.tar", last modified: Tue Oct 24 10:50:21 2023, max compression
+gzip compressed data, was "velintegrator-1.1.5.tar", last modified: Mon May 13 08:57:32 2024, max compression
```

## Comparing `velintegrator-1.1.4.tar` & `velintegrator-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-10-24 10:50:21.504340 velintegrator-1.1.4/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-11 12:42:19.000000 velintegrator-1.1.4/MANIFEST.in
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      957 2023-10-24 10:50:21.504087 velintegrator-1.1.4/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      770 2023-08-24 09:32:57.000000 velintegrator-1.1.4/README.md
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2023-10-24 10:50:21.504390 velintegrator-1.1.4/setup.cfg
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      400 2023-10-24 10:47:37.000000 velintegrator-1.1.4/setup.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-10-24 10:50:21.503250 velintegrator-1.1.4/velintegrator/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 12:42:19.000000 velintegrator-1.1.4/velintegrator/__init__.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      776 2023-09-26 14:18:57.000000 velintegrator-1.1.4/velintegrator/handler.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     4323 2023-10-24 10:47:37.000000 velintegrator-1.1.4/velintegrator/sdk.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-10-24 10:50:21.503858 velintegrator-1.1.4/velintegrator.egg-info/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      957 2023-10-24 10:50:21.000000 velintegrator-1.1.4/velintegrator.egg-info/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2023-10-24 10:50:21.000000 velintegrator-1.1.4/velintegrator.egg-info/SOURCES.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2023-10-24 10:50:21.000000 velintegrator-1.1.4/velintegrator.egg-info/dependency_links.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2023-10-24 10:50:21.000000 velintegrator-1.1.4/velintegrator.egg-info/top_level.txt
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2024-05-13 08:57:32.326769 velintegrator-1.1.5/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-11 12:42:19.000000 velintegrator-1.1.5/MANIFEST.in
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      957 2024-05-13 08:57:32.326592 velintegrator-1.1.5/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      770 2023-08-24 09:32:57.000000 velintegrator-1.1.5/readme.md
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2024-05-13 08:57:32.326807 velintegrator-1.1.5/setup.cfg
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      400 2024-05-13 08:54:57.000000 velintegrator-1.1.5/setup.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2024-05-13 08:57:32.325729 velintegrator-1.1.5/velintegrator/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 12:42:19.000000 velintegrator-1.1.5/velintegrator/__init__.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      776 2023-09-26 14:18:57.000000 velintegrator-1.1.5/velintegrator/handler.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     4344 2024-05-13 08:56:20.000000 velintegrator-1.1.5/velintegrator/sdk.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2024-05-13 08:57:32.326439 velintegrator-1.1.5/velintegrator.egg-info/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      957 2024-05-13 08:57:32.000000 velintegrator-1.1.5/velintegrator.egg-info/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2024-05-13 08:57:32.000000 velintegrator-1.1.5/velintegrator.egg-info/SOURCES.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2024-05-13 08:57:32.000000 velintegrator-1.1.5/velintegrator.egg-info/dependency_links.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2024-05-13 08:57:32.000000 velintegrator-1.1.5/velintegrator.egg-info/top_level.txt
```

### Comparing `velintegrator-1.1.4/PKG-INFO` & `velintegrator-1.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velintegrator
-Version: 1.1.4
+Version: 1.1.5
 Summary: Veli Third Party Integrator
 Author: Dachi
 Author-email: dvadachkoria@veli.store
 Description-Content-Type: text/markdown
 
 VELIntegrator - Package for third-party integrations ;)
```

### Comparing `velintegrator-1.1.4/README.md` & `velintegrator-1.1.5/readme.md`

 * *Files identical despite different names*

### Comparing `velintegrator-1.1.4/velintegrator/handler.py` & `velintegrator-1.1.5/velintegrator/handler.py`

 * *Files identical despite different names*

### Comparing `velintegrator-1.1.4/velintegrator/sdk.py` & `velintegrator-1.1.5/velintegrator/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,21 @@
     headers = {}
     service = None
 
     def __init__(self, model=None):
         self.data = self.set_data(model)
 
     def validate_response(self, response):
-        if response.status_code not in [200, 201, 204]:
-            response_content = "Invalid response, status code: " + str(response.status_code) + " " + \
-                               str(response.json())
-            logger.error(f"{self.service} {response.url} response : {response_content}")
-            return response_content
         try:
+            if response.status_code not in [200, 201, 204]:
+                response_content = "Invalid response, status code: " + str(response.status_code) + " " + \
+                                   str(response.json())
+                logger.error(f"{self.service} {response.url} response : {response_content}")
+                return response_content
+
             response_content = response.json().get('id', response.json())
         except JSONDecodeError:
             response_content = f"Response content: {response.content}, Response: {response}"
         logger.info(f"{self.service} {response.url} response : {response_content}")
         return response_content
 
     def set_data(self, model):
```

### Comparing `velintegrator-1.1.4/velintegrator.egg-info/PKG-INFO` & `velintegrator-1.1.5/velintegrator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velintegrator
-Version: 1.1.4
+Version: 1.1.5
 Summary: Veli Third Party Integrator
 Author: Dachi
 Author-email: dvadachkoria@veli.store
 Description-Content-Type: text/markdown
 
 VELIntegrator - Package for third-party integrations ;)
```

