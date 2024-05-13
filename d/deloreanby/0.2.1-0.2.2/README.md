# Comparing `tmp/deloreanby-0.2.1.tar.gz` & `tmp/deloreanby-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deloreanby-0.2.1.tar", last modified: Fri May 10 21:16:55 2024, max compression
+gzip compressed data, was "deloreanby-0.2.2.tar", last modified: Mon May 13 01:46:28 2024, max compression
```

## Comparing `deloreanby-0.2.1.tar` & `deloreanby-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-10 21:16:55.009483 deloreanby-0.2.1/
--rw-r--r--   0 lulu      (1000) lulu      (1000)     1064 2024-05-10 14:38:37.000000 deloreanby-0.2.1/LICENSE.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)      638 2024-05-10 21:16:55.009483 deloreanby-0.2.1/PKG-INFO
--rw-r--r--   0 lulu      (1000) lulu      (1000)     2340 2024-05-10 14:50:23.000000 deloreanby-0.2.1/README.md
-drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-10 21:16:55.005483 deloreanby-0.2.1/deloreanby/
--rw-r--r--   0 lulu      (1000) lulu      (1000)      296 2024-05-10 21:16:34.000000 deloreanby-0.2.1/deloreanby/__init__.py
--rw-r--r--   0 lulu      (1000) lulu      (1000)     1413 2024-05-10 21:16:37.000000 deloreanby-0.2.1/deloreanby/core.py
-drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-10 21:16:55.009483 deloreanby-0.2.1/deloreanby.egg-info/
--rw-r--r--   0 lulu      (1000) lulu      (1000)      638 2024-05-10 21:16:54.000000 deloreanby-0.2.1/deloreanby.egg-info/PKG-INFO
--rw-r--r--   0 lulu      (1000) lulu      (1000)      241 2024-05-10 21:16:54.000000 deloreanby-0.2.1/deloreanby.egg-info/SOURCES.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)        1 2024-05-10 21:16:54.000000 deloreanby-0.2.1/deloreanby.egg-info/dependency_links.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)       16 2024-05-10 21:16:54.000000 deloreanby-0.2.1/deloreanby.egg-info/requires.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)       11 2024-05-10 21:16:54.000000 deloreanby-0.2.1/deloreanby.egg-info/top_level.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)       38 2024-05-10 21:16:55.009483 deloreanby-0.2.1/setup.cfg
--rw-r--r--   0 lulu      (1000) lulu      (1000)      834 2024-05-10 21:16:32.000000 deloreanby-0.2.1/setup.py
+drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 01:46:28.654411 deloreanby-0.2.2/
+-rw-r--r--   0 lulu      (1000) lulu      (1000)     1064 2024-05-10 21:44:26.000000 deloreanby-0.2.2/LICENSE
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      634 2024-05-13 01:46:28.650411 deloreanby-0.2.2/PKG-INFO
+-rw-r--r--   0 lulu      (1000) lulu      (1000)     2341 2024-05-10 21:44:26.000000 deloreanby-0.2.2/README.md
+drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 01:46:28.650411 deloreanby-0.2.2/deloreanby/
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      296 2024-05-13 01:36:46.000000 deloreanby-0.2.2/deloreanby/__init__.py
+-rw-r--r--   0 lulu      (1000) lulu      (1000)     2080 2024-05-13 01:36:40.000000 deloreanby-0.2.2/deloreanby/core.py
+drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 01:46:28.650411 deloreanby-0.2.2/deloreanby.egg-info/
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      634 2024-05-13 01:46:28.000000 deloreanby-0.2.2/deloreanby.egg-info/PKG-INFO
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      237 2024-05-13 01:46:28.000000 deloreanby-0.2.2/deloreanby.egg-info/SOURCES.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)        1 2024-05-13 01:46:28.000000 deloreanby-0.2.2/deloreanby.egg-info/dependency_links.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)       16 2024-05-13 01:46:28.000000 deloreanby-0.2.2/deloreanby.egg-info/requires.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)       11 2024-05-13 01:46:28.000000 deloreanby-0.2.2/deloreanby.egg-info/top_level.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)       38 2024-05-13 01:46:28.654411 deloreanby-0.2.2/setup.cfg
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      834 2024-05-13 01:36:50.000000 deloreanby-0.2.2/setup.py
```

### Comparing `deloreanby-0.2.1/LICENSE.txt` & `deloreanby-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deloreanby-0.2.1/PKG-INFO` & `deloreanby-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deloreanby
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package that bypasses advertisements to streamline user experiences with content.
 Home-page: https://github.com/KirbyHacks/DeloreanBY
 Author: ! rL⌀w
 Author-email: bytebvrd@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
-License-File: LICENSE.txt
+License-File: LICENSE
```

### Comparing `deloreanby-0.2.1/README.md` & `deloreanby-0.2.2/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -89,8 +89,8 @@
 ### License
 Distributed under the MIT License. See `LICENSE` for more information.
 
 ### Credits and Acknowledgments
 Special thanks to Woozy for the initial concept and to all beta testers who provided essential feedback.
 
 ### Contact
-Contact me rlow._. on discord for more information
+Contact me rlow._. on discord for more information
```

### Comparing `deloreanby-0.2.1/deloreanby/core.py` & `deloreanby-0.2.2/deloreanby/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,28 +5,42 @@
 class DeloreanPremium():
     async def get(self, *, url, api_key, advanced_mode=False):
         async with aiohttp.ClientSession() as session:
             async with session.get(f"https://dlr-api.woozym.workers.dev/?url={quote(url)}", headers={"x-api-key": api_key}) as response:
                 if response.status != 200:
                     return await response.text()
                 try:
-                    r = json.loads(await response.text())
+                    r = await response.json()
                     if advanced_mode:
                         return r
                     return r["result"]
                 except Exception as e:
                     print(e)
                     return "API is currently offline or down. Please try again later."
                 
 class DeloreanFree():
     async def get(self, *, url):
         async with aiohttp.ClientSession() as session:
             async with session.get(f"https://delorean-free-api.woozym.workers.dev/api/linkvertise?url={quote(url)}") as response:
                 if response.status != 200:
                     return await response.text()
                 try:
-                    r = json.loads(await response.text())
+                    r = await response.json()
                     return r["result"]
                 except Exception as e:
                     print(e)
                     return "API is currently offline or down. Please try again later."
-                
+                
+class DeloreanOwner():
+    async def get(self, url, api_key,advanced_mode=True):
+        async with aiohttp.ClientSession() as session:
+            async with session.get(f"http://localhost:4685/?url={quote(url)}", headers={"x-api-key": api_key}) as response:
+                if response.status != 200:
+                    return await response.text()
+                try:
+                    r = await response.json()
+                    if advanced_mode:
+                        return r
+                    return r["result"]
+                except Exception as e:
+                    print(e)
+                    return "API is currently offline or down. Please try again later."
```

### Comparing `deloreanby-0.2.1/deloreanby.egg-info/PKG-INFO` & `deloreanby-0.2.2/deloreanby.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deloreanby
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package that bypasses advertisements to streamline user experiences with content.
 Home-page: https://github.com/KirbyHacks/DeloreanBY
 Author: ! rL⌀w
 Author-email: bytebvrd@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
-License-File: LICENSE.txt
+License-File: LICENSE
```

### Comparing `deloreanby-0.2.1/setup.py` & `deloreanby-0.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='deloreanby',
-    version='0.2.1',    
+    version='0.2.2',    
     description='A Python package that bypasses advertisements to streamline user experiences with content.',
     url='https://github.com/KirbyHacks/DeloreanBY',
     author='! rL⌀w',
     author_email='bytebvrd@gmail.com',
     license='MIT',
     packages=['deloreanby'],
     install_requires=['urllib3',
```

