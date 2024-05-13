# Comparing `tmp/scrapeddit-0.3.5.tar.gz` & `tmp/scrapeddit-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.3.5.tar", last modified: Mon May 13 18:00:18 2024, max compression
+gzip compressed data, was "scrapeddit-0.3.6.tar", last modified: Mon May 13 18:10:17 2024, max compression
```

## Comparing `scrapeddit-0.3.5.tar` & `scrapeddit-0.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 18:00:18.073301 scrapeddit-0.3.5/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.3.5/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-13 18:00:18.072975 scrapeddit-0.3.5/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4207 2024-05-11 19:15:14.000000 scrapeddit-0.3.5/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 18:00:18.071278 scrapeddit-0.3.5/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.3.5/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.3.5/scrapeddit/authentication.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1142 2024-05-12 17:50:33.000000 scrapeddit-0.3.5/scrapeddit/models.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4454 2024-05-13 17:58:46.000000 scrapeddit-0.3.5/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.3.5/scrapeddit/scrapeonce.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3014 2024-05-11 13:11:08.000000 scrapeddit-0.3.5/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      599 2024-05-11 12:59:46.000000 scrapeddit-0.3.5/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 18:00:18.072660 scrapeddit-0.3.5/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-13 18:00:18.000000 scrapeddit-0.3.5/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      366 2024-05-13 18:00:18.000000 scrapeddit-0.3.5/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-13 18:00:18.000000 scrapeddit-0.3.5/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-13 18:00:18.000000 scrapeddit-0.3.5/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-13 18:00:18.000000 scrapeddit-0.3.5/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-13 18:00:18.073380 scrapeddit-0.3.5/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      660 2024-05-13 18:00:07.000000 scrapeddit-0.3.5/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 18:10:17.385887 scrapeddit-0.3.6/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.3.6/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-13 18:10:17.385585 scrapeddit-0.3.6/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4207 2024-05-11 19:15:14.000000 scrapeddit-0.3.6/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 18:10:17.384044 scrapeddit-0.3.6/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.3.6/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.3.6/scrapeddit/authentication.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1142 2024-05-12 17:50:33.000000 scrapeddit-0.3.6/scrapeddit/models.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4455 2024-05-13 18:09:23.000000 scrapeddit-0.3.6/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.3.6/scrapeddit/scrapeonce.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3014 2024-05-11 13:11:08.000000 scrapeddit-0.3.6/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      599 2024-05-11 12:59:46.000000 scrapeddit-0.3.6/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 18:10:17.385248 scrapeddit-0.3.6/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-13 18:10:17.000000 scrapeddit-0.3.6/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      366 2024-05-13 18:10:17.000000 scrapeddit-0.3.6/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-13 18:10:17.000000 scrapeddit-0.3.6/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-13 18:10:17.000000 scrapeddit-0.3.6/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-13 18:10:17.000000 scrapeddit-0.3.6/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-13 18:10:17.385956 scrapeddit-0.3.6/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      660 2024-05-13 18:10:09.000000 scrapeddit-0.3.6/setup.py
```

### Comparing `scrapeddit-0.3.5/LICENSE.txt` & `scrapeddit-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.5/PKG-INFO` & `scrapeddit-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.3.5
+Version: 0.3.6
 Summary: Simple test package
 Home-page: https://github.com/Mafaz03/scrapeddit
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
```

### Comparing `scrapeddit-0.3.5/README.md` & `scrapeddit-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.5/scrapeddit/authentication.py` & `scrapeddit-0.3.6/scrapeddit/authentication.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.5/scrapeddit/models.py` & `scrapeddit-0.3.6/scrapeddit/models.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.5/scrapeddit/redditdl.py` & `scrapeddit-0.3.6/scrapeddit/redditdl.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     plt.ylabel('Count')
     plt.xticks(rotation=45, ha='right')
     plt.grid(axis='y', linestyle='--', alpha=0.7)
     plt.tight_layout()
     plt.show()
 
   def __len__(self):
-    return len(self.collted_ds)
+    return len(self.collated_ds)
 
   def __getitem__(self, idx):
     pil_image, y = self.collated_ds[idx]
     try:
       pil_image.thumbnail((self.max_size, self.max_size), Image.LANCZOS)
       if pil_image.mode != 'RGB': pil_image = pil_image.convert('RGB')
       img_tensor = self.transform(pil_image)
```

### Comparing `scrapeddit-0.3.5/scrapeddit/scrapeonce.py` & `scrapeddit-0.3.6/scrapeddit/scrapeonce.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.5/scrapeddit/showit.py` & `scrapeddit-0.3.6/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.5/scrapeddit/transforms.py` & `scrapeddit-0.3.6/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.5/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.3.6/scrapeddit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.3.5
+Version: 0.3.6
 Summary: Simple test package
 Home-page: https://github.com/Mafaz03/scrapeddit
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
```

### Comparing `scrapeddit-0.3.5/setup.py` & `scrapeddit-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.3.5',
+    version='0.3.6',
     url='https://github.com/Mafaz03/scrapeddit',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

