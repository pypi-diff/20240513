# Comparing `tmp/gradescope-tool-0.1.0.tar.gz` & `tmp/gradescope_tool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradescope-tool-0.1.0.tar", last modified: Sun May  5 02:01:38 2024, max compression
+gzip compressed data, was "gradescope_tool-0.1.1.tar", last modified: Mon May 13 08:20:06 2024, max compression
```

## Comparing `gradescope-tool-0.1.0.tar` & `gradescope_tool-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-05-05 02:01:38.414529 gradescope-tool-0.1.0/
--rw-r--r--   0 nitro      (501) staff       (20)     1091 2024-04-25 19:40:47.000000 gradescope-tool-0.1.0/LICENSE
--rw-r--r--   0 nitro      (501) staff       (20)     9390 2024-05-05 02:01:38.414625 gradescope-tool-0.1.0/PKG-INFO
--rw-r--r--   0 nitro      (501) staff       (20)     8825 2024-05-05 01:57:29.000000 gradescope-tool-0.1.0/README.md
-drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-05-05 02:01:38.413782 gradescope-tool-0.1.0/gradescope/
--rw-r--r--   0 nitro      (501) staff       (20)      270 2024-04-25 19:38:11.000000 gradescope-tool-0.1.0/gradescope/__init__.py
--rw-r--r--   0 nitro      (501) staff       (20)      441 2024-04-25 22:39:25.000000 gradescope-tool-0.1.0/gradescope/constants.py
--rw-r--r--   0 nitro      (501) staff       (20)     2136 2024-04-25 23:06:44.000000 gradescope-tool-0.1.0/gradescope/dataclass.py
--rw-r--r--   0 nitro      (501) staff       (20)      537 2024-04-25 23:05:16.000000 gradescope-tool-0.1.0/gradescope/errors.py
--rw-r--r--   0 nitro      (501) staff       (20)    15676 2024-04-25 23:06:39.000000 gradescope-tool-0.1.0/gradescope/gradescope.py
--rw-r--r--   0 nitro      (501) staff       (20)     1783 2024-04-25 23:06:41.000000 gradescope-tool-0.1.0/gradescope/utils.py
-drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-05-05 02:01:38.414381 gradescope-tool-0.1.0/gradescope_tool.egg-info/
--rw-r--r--   0 nitro      (501) staff       (20)     9390 2024-05-05 02:01:38.000000 gradescope-tool-0.1.0/gradescope_tool.egg-info/PKG-INFO
--rw-r--r--   0 nitro      (501) staff       (20)      329 2024-05-05 02:01:38.000000 gradescope-tool-0.1.0/gradescope_tool.egg-info/SOURCES.txt
--rw-r--r--   0 nitro      (501) staff       (20)        1 2024-05-05 02:01:38.000000 gradescope-tool-0.1.0/gradescope_tool.egg-info/dependency_links.txt
--rw-r--r--   0 nitro      (501) staff       (20)       11 2024-05-05 02:01:38.000000 gradescope-tool-0.1.0/gradescope_tool.egg-info/top_level.txt
--rw-r--r--   0 nitro      (501) staff       (20)       79 2024-05-05 02:01:38.414900 gradescope-tool-0.1.0/setup.cfg
--rw-r--r--   0 nitro      (501) staff       (20)      812 2024-05-05 01:59:33.000000 gradescope-tool-0.1.0/setup.py
+drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-05-13 08:20:06.315635 gradescope_tool-0.1.1/
+-rw-r--r--   0 nitro      (501) staff       (20)     1091 2024-04-25 19:40:47.000000 gradescope_tool-0.1.1/LICENSE
+-rw-r--r--   0 nitro      (501) staff       (20)     9390 2024-05-13 08:20:06.315460 gradescope_tool-0.1.1/PKG-INFO
+-rw-r--r--   0 nitro      (501) staff       (20)     8825 2024-05-05 01:57:29.000000 gradescope_tool-0.1.1/README.md
+drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-05-13 08:20:06.314270 gradescope_tool-0.1.1/gradescope/
+-rw-r--r--   0 nitro      (501) staff       (20)      270 2024-04-25 19:38:11.000000 gradescope_tool-0.1.1/gradescope/__init__.py
+-rw-r--r--   0 nitro      (501) staff       (20)      435 2024-05-12 23:26:52.000000 gradescope_tool-0.1.1/gradescope/constants.py
+-rw-r--r--   0 nitro      (501) staff       (20)     2136 2024-04-25 23:06:44.000000 gradescope_tool-0.1.1/gradescope/dataclass.py
+-rw-r--r--   0 nitro      (501) staff       (20)      537 2024-04-25 23:05:16.000000 gradescope_tool-0.1.1/gradescope/errors.py
+-rw-r--r--   0 nitro      (501) staff       (20)    15715 2024-05-12 23:31:58.000000 gradescope_tool-0.1.1/gradescope/gradescope.py
+-rw-r--r--   0 nitro      (501) staff       (20)     1783 2024-04-25 23:06:41.000000 gradescope_tool-0.1.1/gradescope/utils.py
+drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-05-13 08:20:06.315227 gradescope_tool-0.1.1/gradescope_tool.egg-info/
+-rw-r--r--   0 nitro      (501) staff       (20)     9390 2024-05-13 08:20:06.000000 gradescope_tool-0.1.1/gradescope_tool.egg-info/PKG-INFO
+-rw-r--r--   0 nitro      (501) staff       (20)      329 2024-05-13 08:20:06.000000 gradescope_tool-0.1.1/gradescope_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 nitro      (501) staff       (20)        1 2024-05-13 08:20:06.000000 gradescope_tool-0.1.1/gradescope_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 nitro      (501) staff       (20)       11 2024-05-13 08:20:06.000000 gradescope_tool-0.1.1/gradescope_tool.egg-info/top_level.txt
+-rw-r--r--   0 nitro      (501) staff       (20)       79 2024-05-13 08:20:06.315861 gradescope_tool-0.1.1/setup.cfg
+-rw-r--r--   0 nitro      (501) staff       (20)      884 2024-05-12 23:38:35.000000 gradescope_tool-0.1.1/setup.py
```

### Comparing `gradescope-tool-0.1.0/LICENSE` & `gradescope_tool-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gradescope-tool-0.1.0/PKG-INFO` & `gradescope_tool-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: gradescope-tool
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for Gradescope to easily retrieve data from your Gradescope Courses.
 Home-page: https://github.com/Teaching-and-Learning-in-Computing/Gradescope
 Author: HyunJun Park, Daniel Song
 Author-email: hyunjup4@uci.edu, djsong1@uci.edu
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
    <img src="./docs/icon.png" width="200" height="200">
    <h1 align="center">GRADESCOPE</h1>
 </p>
```

### Comparing `gradescope-tool-0.1.0/README.md` & `gradescope_tool-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gradescope-tool-0.1.0/gradescope/dataclass.py` & `gradescope_tool-0.1.1/gradescope/dataclass.py`

 * *Files identical despite different names*

### Comparing `gradescope-tool-0.1.0/gradescope/errors.py` & `gradescope_tool-0.1.1/gradescope/errors.py`

 * *Files identical despite different names*

### Comparing `gradescope-tool-0.1.0/gradescope/gradescope.py` & `gradescope_tool-0.1.1/gradescope/gradescope.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,14 +350,15 @@
 
         Raises:
             NotLoggedInError: If the user is not logged in.
         '''
         if not self.logged_in: raise NotLoggedInError
 
         response = self.session.get(url)
+        self._response_check(response)
         with open(path, 'wb') as file:
             file.write(response.content)
 
     def _response_check(self, response: requests.Response) -> bool:
         '''
         Checks the response status code and raises an error if it's not 200.
```

### Comparing `gradescope-tool-0.1.0/gradescope/utils.py` & `gradescope_tool-0.1.1/gradescope/utils.py`

 * *Files identical despite different names*

### Comparing `gradescope-tool-0.1.0/gradescope_tool.egg-info/PKG-INFO` & `gradescope_tool-0.1.1/gradescope_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: gradescope-tool
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for Gradescope to easily retrieve data from your Gradescope Courses.
 Home-page: https://github.com/Teaching-and-Learning-in-Computing/Gradescope
 Author: HyunJun Park, Daniel Song
 Author-email: hyunjup4@uci.edu, djsong1@uci.edu
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
    <img src="./docs/icon.png" width="200" height="200">
    <h1 align="center">GRADESCOPE</h1>
 </p>
```

