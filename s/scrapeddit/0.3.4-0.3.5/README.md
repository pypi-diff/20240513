# Comparing `tmp/scrapeddit-0.3.4.tar.gz` & `tmp/scrapeddit-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.3.4.tar", last modified: Mon May 13 17:52:10 2024, max compression
+gzip compressed data, was "scrapeddit-0.3.5.tar", last modified: Mon May 13 18:00:18 2024, max compression
```

## Comparing `scrapeddit-0.3.4.tar` & `scrapeddit-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 17:52:10.479164 scrapeddit-0.3.4/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.3.4/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-13 17:52:10.478829 scrapeddit-0.3.4/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4207 2024-05-11 19:15:14.000000 scrapeddit-0.3.4/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 17:52:10.477290 scrapeddit-0.3.4/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.3.4/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.3.4/scrapeddit/authentication.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1142 2024-05-12 17:50:33.000000 scrapeddit-0.3.4/scrapeddit/models.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4473 2024-05-13 17:45:04.000000 scrapeddit-0.3.4/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.3.4/scrapeddit/scrapeonce.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3014 2024-05-11 13:11:08.000000 scrapeddit-0.3.4/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      599 2024-05-11 12:59:46.000000 scrapeddit-0.3.4/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 17:52:10.478461 scrapeddit-0.3.4/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-13 17:52:10.000000 scrapeddit-0.3.4/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      366 2024-05-13 17:52:10.000000 scrapeddit-0.3.4/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-13 17:52:10.000000 scrapeddit-0.3.4/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-13 17:52:10.000000 scrapeddit-0.3.4/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-13 17:52:10.000000 scrapeddit-0.3.4/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-13 17:52:10.479231 scrapeddit-0.3.4/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      660 2024-05-13 17:52:00.000000 scrapeddit-0.3.4/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 18:00:18.073301 scrapeddit-0.3.5/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.3.5/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-13 18:00:18.072975 scrapeddit-0.3.5/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4207 2024-05-11 19:15:14.000000 scrapeddit-0.3.5/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 18:00:18.071278 scrapeddit-0.3.5/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.3.5/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.3.5/scrapeddit/authentication.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1142 2024-05-12 17:50:33.000000 scrapeddit-0.3.5/scrapeddit/models.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4454 2024-05-13 17:58:46.000000 scrapeddit-0.3.5/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.3.5/scrapeddit/scrapeonce.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3014 2024-05-11 13:11:08.000000 scrapeddit-0.3.5/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      599 2024-05-11 12:59:46.000000 scrapeddit-0.3.5/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-13 18:00:18.072660 scrapeddit-0.3.5/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     4507 2024-05-13 18:00:18.000000 scrapeddit-0.3.5/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      366 2024-05-13 18:00:18.000000 scrapeddit-0.3.5/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-13 18:00:18.000000 scrapeddit-0.3.5/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-13 18:00:18.000000 scrapeddit-0.3.5/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-13 18:00:18.000000 scrapeddit-0.3.5/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-13 18:00:18.073380 scrapeddit-0.3.5/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      660 2024-05-13 18:00:07.000000 scrapeddit-0.3.5/setup.py
```

### Comparing `scrapeddit-0.3.4/LICENSE.txt` & `scrapeddit-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.4/PKG-INFO` & `scrapeddit-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simple test package
 Home-page: https://github.com/Mafaz03/scrapeddit
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
```

### Comparing `scrapeddit-0.3.4/README.md` & `scrapeddit-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.4/scrapeddit/authentication.py` & `scrapeddit-0.3.5/scrapeddit/authentication.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.4/scrapeddit/models.py` & `scrapeddit-0.3.5/scrapeddit/models.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.4/scrapeddit/redditdl.py` & `scrapeddit-0.3.5/scrapeddit/redditdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,15 @@
           pil_image = Image.open(BytesIO(response.content))
           self.collated_ds.append([pil_image, r])
         except: pass
 
     z = [i[1] for i in self.collated_ds]
     self.ds_count = dict(Counter(z))
 
-    if upsample: 
-      print(f"Before upsample, size of dataset: {len(self.collated_ds)}")
-      self.collated_ds = upsample(self.collated_ds)
-      print(f"After upsample, size of dataset: {len(self.collated_ds)}")
+    if upsample: self.collated_ds = upsampling(self.collated_ds)
 
   def __call__(self):
     print(f"Out of {len(self.subreddit) * self.limit}, {len(self.collated_ds)} were able to scrape")
     plt.bar(self.ds_count.keys(), self.ds_count.values())
     plt.title('Distribution of Data Sources')
     plt.xlabel('Data Sources')
     plt.ylabel('Count')
@@ -100,15 +97,16 @@
       img_tensor = self.transform(pil_image)
       if img_tensor.shape[0] == 3: img_tensor = img_tensor.permute(1, 2, 0)
       np_image = np.array(img_tensor)
       return {'image': np_image, 'y': y}
     except UnidentifiedImageError:
       return None
 
-def upsample(collated_ds):
+def upsampling(collated_ds):
+  print(f"\nBefore upsample, size of dataset: {len(collated_ds)}")
   labels = [i[1] for i in collated_ds]
   labels_idx = {}
   for i, label in enumerate(labels):
     if label not in labels_idx:
       labels_idx[label] = []
     labels_idx[label].append(i)
 
@@ -118,8 +116,9 @@
   for i in to_sample:
     temp = []
     for k, j in enumerate(collated_ds):
       if collated_ds[k][1] == i:
         temp.append(collated_ds[k])
     extra_sample = random.choices(temp, k=count_dict[max_key]-count_dict[i])
     collated_ds += extra_sample
+  print(f"After upsample, size of dataset: {len(collated_ds)}")
   return collated_ds
```

### Comparing `scrapeddit-0.3.4/scrapeddit/scrapeonce.py` & `scrapeddit-0.3.5/scrapeddit/scrapeonce.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.4/scrapeddit/showit.py` & `scrapeddit-0.3.5/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.4/scrapeddit/transforms.py` & `scrapeddit-0.3.5/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.4/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.3.5/scrapeddit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simple test package
 Home-page: https://github.com/Mafaz03/scrapeddit
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
```

### Comparing `scrapeddit-0.3.4/setup.py` & `scrapeddit-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.3.4',
+    version='0.3.5',
     url='https://github.com/Mafaz03/scrapeddit',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

