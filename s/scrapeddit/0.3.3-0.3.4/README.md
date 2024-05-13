# Comparing `tmp/scrapeddit-0.3.3.tar.gz` & `tmp/scrapeddit-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.3.3.tar", last modified: Sat May 11 19:19:21 2024, max compression
+gzip compressed data, was "scrapeddit-0.3.4.tar", last modified: Mon May 13 17:52:10 2024, max compression
```

## Comparing `scrapeddit-0.3.3.tar` & `scrapeddit-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 19:19:21.913448 scrapeddit-0.3.3/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.3.3/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-11 19:19:21.913114 scrapeddit-0.3.3/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4207 2024-05-11 19:15:14.000000 scrapeddit-0.3.3/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 19:19:21.911316 scrapeddit-0.3.3/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.3.3/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.3.3/scrapeddit/authentication.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1048 2024-05-11 19:09:26.000000 scrapeddit-0.3.3/scrapeddit/models.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3549 2024-05-11 13:08:02.000000 scrapeddit-0.3.3/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.3.3/scrapeddit/scrapeonce.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3014 2024-05-11 13:11:08.000000 scrapeddit-0.3.3/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      599 2024-05-11 12:59:46.000000 scrapeddit-0.3.3/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 19:19:21.912760 scrapeddit-0.3.3/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-11 19:19:21.000000 scrapeddit-0.3.3/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      366 2024-05-11 19:19:21.000000 scrapeddit-0.3.3/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 19:19:21.000000 scrapeddit-0.3.3/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 19:19:21.000000 scrapeddit-0.3.3/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 19:19:21.000000 scrapeddit-0.3.3/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 19:19:21.913525 scrapeddit-0.3.3/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      660 2024-05-11 19:15:38.000000 scrapeddit-0.3.3/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 17:52:10.479164 scrapeddit-0.3.4/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.3.4/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-13 17:52:10.478829 scrapeddit-0.3.4/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4207 2024-05-11 19:15:14.000000 scrapeddit-0.3.4/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 17:52:10.477290 scrapeddit-0.3.4/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.3.4/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.3.4/scrapeddit/authentication.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1142 2024-05-12 17:50:33.000000 scrapeddit-0.3.4/scrapeddit/models.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4473 2024-05-13 17:45:04.000000 scrapeddit-0.3.4/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.3.4/scrapeddit/scrapeonce.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3014 2024-05-11 13:11:08.000000 scrapeddit-0.3.4/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      599 2024-05-11 12:59:46.000000 scrapeddit-0.3.4/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 17:52:10.478461 scrapeddit-0.3.4/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-13 17:52:10.000000 scrapeddit-0.3.4/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      366 2024-05-13 17:52:10.000000 scrapeddit-0.3.4/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-13 17:52:10.000000 scrapeddit-0.3.4/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-13 17:52:10.000000 scrapeddit-0.3.4/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-13 17:52:10.000000 scrapeddit-0.3.4/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-13 17:52:10.479231 scrapeddit-0.3.4/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      660 2024-05-13 17:52:00.000000 scrapeddit-0.3.4/setup.py
```

### Comparing `scrapeddit-0.3.3/LICENSE.txt` & `scrapeddit-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.3/PKG-INFO` & `scrapeddit-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simple test package
 Home-page: https://github.com/Mafaz03/scrapeddit
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
```

### Comparing `scrapeddit-0.3.3/README.md` & `scrapeddit-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.3/scrapeddit/authentication.py` & `scrapeddit-0.3.4/scrapeddit/authentication.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.3/scrapeddit/models.py` & `scrapeddit-0.3.4/scrapeddit/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import torchvision
 import torch
 import torchvision.models as models
 
-def get_efficient(device = False):
+def get_efficient(device = False, freeze = False):
     weights = torchvision.models.EfficientNet_B0_Weights.DEFAULT
     if device == True: 
         if torch.backends.mps.is_available(): device = 'mps'
         else: device = 'cuda' if torch.cuda.is_available() else 'cpu'
         model =  torchvision.models.efficientnet_b0(weights=weights).to(device)
     else: model = torchvision.models.efficientnet_b0(weights=weights)
-    for param in model.features.parameters():
-        param.requires_grad = False
+    if freeze == True:
+        for param in model.features.parameters():
+            param.requires_grad = False
     return model
 
-def get_vision_model(model_name='vgg16', pretrained=True, device=None):
+def get_vision_model(model_name='vgg16', pretrained=True, device=None, freeze = False):
     if device == True: 
         if torch.backends.mps.is_available(): device = 'mps'
         else: device = 'cuda' if torch.cuda.is_available() else 'cpu'
         model = models.__dict__[model_name](pretrained=pretrained).to(device)
     else: model = models.__dict__[model_name](pretrained=pretrained)
-    for param in model.features.parameters():
-        param.requires_grad = False
+    if freeze == True:
+        for param in model.features.parameters():
+            param.requires_grad = False
     return model
```

### Comparing `scrapeddit-0.3.3/scrapeddit/scrapeonce.py` & `scrapeddit-0.3.4/scrapeddit/scrapeonce.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.3/scrapeddit/showit.py` & `scrapeddit-0.3.4/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.3/scrapeddit/transforms.py` & `scrapeddit-0.3.4/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.3/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.3.4/scrapeddit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simple test package
 Home-page: https://github.com/Mafaz03/scrapeddit
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
```

### Comparing `scrapeddit-0.3.3/setup.py` & `scrapeddit-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.3.3',
+    version='0.3.4',
     url='https://github.com/Mafaz03/scrapeddit',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

