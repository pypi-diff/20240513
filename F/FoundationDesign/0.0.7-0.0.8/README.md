# Comparing `tmp/FoundationDesign-0.0.7.tar.gz` & `tmp/FoundationDesign-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FoundationDesign-0.0.7.tar", last modified: Wed May  1 20:09:07 2024, max compression
+gzip compressed data, was "FoundationDesign-0.0.8.tar", last modified: Mon May 13 20:59:33 2024, max compression
```

## Comparing `FoundationDesign-0.0.7.tar` & `FoundationDesign-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 20:09:07.287370 FoundationDesign-0.0.7/
-drwxrwxrwx   0        0        0        0 2024-05-01 20:09:07.283381 FoundationDesign-0.0.7/FoundationDesign.egg-info/
--rw-rw-rw-   0        0        0     7653 2024-05-01 20:09:07.000000 FoundationDesign-0.0.7/FoundationDesign.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-05-01 20:09:07.000000 FoundationDesign-0.0.7/FoundationDesign.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 20:09:07.000000 FoundationDesign-0.0.7/FoundationDesign.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-01 20:09:07.000000 FoundationDesign-0.0.7/FoundationDesign.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 20:09:07.000000 FoundationDesign-0.0.7/FoundationDesign.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2024-04-29 21:30:46.000000 FoundationDesign-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     7653 2024-05-01 20:09:07.285376 FoundationDesign-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     7010 2024-05-01 18:34:26.000000 FoundationDesign-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 20:09:07.287370 FoundationDesign-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      981 2024-05-01 19:02:28.000000 FoundationDesign-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:09:07.279392 FoundationDesign-0.0.7/tests/
--rw-rw-rw-   0        0        0     2382 2024-04-29 21:31:05.000000 FoundationDesign-0.0.7/tests/test.py
--rw-rw-rw-   0        0        0     1187 2024-04-06 14:37:43.000000 FoundationDesign-0.0.7/tests/test2.py
--rw-rw-rw-   0        0        0     3110 2024-05-01 17:30:05.000000 FoundationDesign-0.0.7/tests/test_PadFoundation.py
--rw-rw-rw-   0        0        0     5573 2024-05-01 16:08:17.000000 FoundationDesign-0.0.7/tests/test_PadFoundationDesign.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:59:33.111822 FoundationDesign-0.0.8/
+drwxrwxrwx   0        0        0        0 2024-05-13 20:59:33.017817 FoundationDesign-0.0.8/FoundationDesign/
+-rw-rw-rw-   0        0        0      604 2024-05-01 15:02:22.000000 FoundationDesign-0.0.8/FoundationDesign/__init__.py
+-rw-rw-rw-   0        0        0   158437 2024-05-01 16:07:45.000000 FoundationDesign-0.0.8/FoundationDesign/combinedfootingdesign.py
+-rw-rw-rw-   0        0        0     6984 2024-03-24 17:03:25.000000 FoundationDesign-0.0.8/FoundationDesign/concretedesignfunc.py
+-rw-rw-rw-   0        0        0     2605 2023-11-25 12:38:34.000000 FoundationDesign-0.0.8/FoundationDesign/datavalidation.py
+-rw-rw-rw-   0        0        0    98781 2024-05-01 18:21:39.000000 FoundationDesign-0.0.8/FoundationDesign/foundationdesign.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:59:33.101317 FoundationDesign-0.0.8/FoundationDesign.egg-info/
+-rw-rw-rw-   0        0        0     7653 2024-05-13 20:59:32.000000 FoundationDesign-0.0.8/FoundationDesign.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-13 20:59:32.000000 FoundationDesign-0.0.8/FoundationDesign.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 20:59:32.000000 FoundationDesign-0.0.8/FoundationDesign.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-13 20:59:32.000000 FoundationDesign-0.0.8/FoundationDesign.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-13 20:59:32.000000 FoundationDesign-0.0.8/FoundationDesign.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-04-29 21:30:46.000000 FoundationDesign-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     7653 2024-05-13 20:59:33.101317 FoundationDesign-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7010 2024-05-01 18:34:26.000000 FoundationDesign-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 20:59:33.111822 FoundationDesign-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      951 2024-05-13 20:55:01.000000 FoundationDesign-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:59:33.101317 FoundationDesign-0.0.8/tests/
+-rw-rw-rw-   0        0        0     2382 2024-04-29 21:31:05.000000 FoundationDesign-0.0.8/tests/test.py
+-rw-rw-rw-   0        0        0     1187 2024-04-06 14:37:43.000000 FoundationDesign-0.0.8/tests/test2.py
+-rw-rw-rw-   0        0        0     3110 2024-05-01 17:30:05.000000 FoundationDesign-0.0.8/tests/test_PadFoundation.py
+-rw-rw-rw-   0        0        0     5573 2024-05-01 16:08:17.000000 FoundationDesign-0.0.8/tests/test_PadFoundationDesign.py
```

### Comparing `FoundationDesign-0.0.7/FoundationDesign.egg-info/PKG-INFO` & `FoundationDesign-0.0.8/FoundationDesign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: FoundationDesign
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python module for structural analysis and design of different foundation types in accordance to the Eurocodes
 Home-page: https://github.com/kunle009/FoundationDesign
 Author: Kunle Yusuf
 Author-email: kunleyusuf858@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: indeterminatebeam==2.2.1
-Requires-Dist: numpy==1.24.4
-Requires-Dist: plotly==5.15.0
+Requires-Dist: numpy>=1.24.4
+Requires-Dist: plotly>=5.15.0
 
 
 # FoundationDesign
 
 [![PyPi](https://img.shields.io/pypi/v/FoundationDesign.svg)](https://pypi.org/project/FoundationDesign/)
 ![PyPI - License](https://img.shields.io/pypi/l/FoundationDesign)
 [![Downloads](https://static.pepy.tech/badge/foundationdesign)](https://pepy.tech/project/foundationdesign)
```

### Comparing `FoundationDesign-0.0.7/LICENSE` & `FoundationDesign-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FoundationDesign-0.0.7/PKG-INFO` & `FoundationDesign-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: FoundationDesign
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python module for structural analysis and design of different foundation types in accordance to the Eurocodes
 Home-page: https://github.com/kunle009/FoundationDesign
 Author: Kunle Yusuf
 Author-email: kunleyusuf858@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: indeterminatebeam==2.2.1
-Requires-Dist: numpy==1.24.4
-Requires-Dist: plotly==5.15.0
+Requires-Dist: numpy>=1.24.4
+Requires-Dist: plotly>=5.15.0
 
 
 # FoundationDesign
 
 [![PyPi](https://img.shields.io/pypi/v/FoundationDesign.svg)](https://pypi.org/project/FoundationDesign/)
 ![PyPI - License](https://img.shields.io/pypi/l/FoundationDesign)
 [![Downloads](https://static.pepy.tech/badge/foundationdesign)](https://pepy.tech/project/foundationdesign)
```

### Comparing `FoundationDesign-0.0.7/README.md` & `FoundationDesign-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `FoundationDesign-0.0.7/setup.py` & `FoundationDesign-0.0.8/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 import os
 
 
 # store readme.md files
 with open("README.md", "r") as fh:
     long_description = fh.read()
 # read the requirements
 with open("requirements.txt", "r") as fh:
     requirements = [line.strip() for line in fh]
 
 setup(
     name="FoundationDesign",
-    packages=find_packages("FoundationDesign"),
-    version="0.0.7",
+    packages=["FoundationDesign"],
+    version="0.0.8",
     author="Kunle Yusuf",
     author_email="kunleyusuf858@gmail.com",
     description="A python module for structural analysis and design of different foundation types in accordance to the Eurocodes",
-    url = 'https://github.com/kunle009/FoundationDesign',
+    url="https://github.com/kunle009/FoundationDesign",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `FoundationDesign-0.0.7/tests/test.py` & `FoundationDesign-0.0.8/tests/test.py`

 * *Files identical despite different names*

### Comparing `FoundationDesign-0.0.7/tests/test2.py` & `FoundationDesign-0.0.8/tests/test2.py`

 * *Files identical despite different names*

### Comparing `FoundationDesign-0.0.7/tests/test_PadFoundation.py` & `FoundationDesign-0.0.8/tests/test_PadFoundation.py`

 * *Files identical despite different names*

### Comparing `FoundationDesign-0.0.7/tests/test_PadFoundationDesign.py` & `FoundationDesign-0.0.8/tests/test_PadFoundationDesign.py`

 * *Files identical despite different names*

