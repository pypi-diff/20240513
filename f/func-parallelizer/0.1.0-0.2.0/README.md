# Comparing `tmp/func_parallelizer-0.1.0.tar.gz` & `tmp/func_parallelizer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_parallelizer-0.1.0.tar", last modified: Mon May 13 16:11:29 2024, max compression
+gzip compressed data, was "func_parallelizer-0.2.0.tar", last modified: Mon May 13 16:26:58 2024, max compression
```

## Comparing `func_parallelizer-0.1.0.tar` & `func_parallelizer-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 16:11:29.151443 func_parallelizer-0.1.0/
--rw-r--r--   0 vikashg    (501) staff       (20)      448 2024-05-13 16:11:29.151774 func_parallelizer-0.1.0/PKG-INFO
--rw-r--r--   0 vikashg    (501) staff       (20)     2225 2024-05-12 17:47:47.000000 func_parallelizer-0.1.0/README.md
-drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 16:11:29.150470 func_parallelizer-0.1.0/func_parallelizer/
--rw-r--r--   0 vikashg    (501) staff       (20)       58 2024-05-12 17:29:31.000000 func_parallelizer-0.1.0/func_parallelizer/__init__.py
--rw-r--r--   0 vikashg    (501) staff       (20)      942 2024-05-13 16:05:35.000000 func_parallelizer-0.1.0/func_parallelizer/func_parallelizer.py
-drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 16:11:29.151321 func_parallelizer-0.1.0/func_parallelizer.egg-info/
--rw-r--r--   0 vikashg    (501) staff       (20)      448 2024-05-13 16:11:29.000000 func_parallelizer-0.1.0/func_parallelizer.egg-info/PKG-INFO
--rw-r--r--   0 vikashg    (501) staff       (20)      301 2024-05-13 16:11:29.000000 func_parallelizer-0.1.0/func_parallelizer.egg-info/SOURCES.txt
--rw-r--r--   0 vikashg    (501) staff       (20)        1 2024-05-13 16:11:29.000000 func_parallelizer-0.1.0/func_parallelizer.egg-info/dependency_links.txt
--rw-r--r--   0 vikashg    (501) staff       (20)        1 2024-05-13 16:11:29.000000 func_parallelizer-0.1.0/func_parallelizer.egg-info/not-zip-safe
--rw-r--r--   0 vikashg    (501) staff       (20)       18 2024-05-13 16:11:29.000000 func_parallelizer-0.1.0/func_parallelizer.egg-info/top_level.txt
--rw-r--r--   0 vikashg    (501) staff       (20)       38 2024-05-13 16:11:29.154565 func_parallelizer-0.1.0/setup.cfg
--rw-r--r--   0 vikashg    (501) staff       (20)      610 2024-05-13 16:10:38.000000 func_parallelizer-0.1.0/setup.py
+drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 16:26:58.778116 func_parallelizer-0.2.0/
+-rw-r--r--   0 vikashg    (501) staff       (20)      352 2024-05-13 16:26:58.778210 func_parallelizer-0.2.0/PKG-INFO
+-rw-r--r--   0 vikashg    (501) staff       (20)     2225 2024-05-12 17:47:47.000000 func_parallelizer-0.2.0/README.md
+drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 16:26:58.777112 func_parallelizer-0.2.0/func_parallelizer/
+-rw-r--r--   0 vikashg    (501) staff       (20)       58 2024-05-12 17:29:31.000000 func_parallelizer-0.2.0/func_parallelizer/__init__.py
+-rw-r--r--   0 vikashg    (501) staff       (20)      942 2024-05-13 16:05:35.000000 func_parallelizer-0.2.0/func_parallelizer/func_parallelizer.py
+drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 16:26:58.777990 func_parallelizer-0.2.0/func_parallelizer.egg-info/
+-rw-r--r--   0 vikashg    (501) staff       (20)      352 2024-05-13 16:26:58.000000 func_parallelizer-0.2.0/func_parallelizer.egg-info/PKG-INFO
+-rw-r--r--   0 vikashg    (501) staff       (20)      301 2024-05-13 16:26:58.000000 func_parallelizer-0.2.0/func_parallelizer.egg-info/SOURCES.txt
+-rw-r--r--   0 vikashg    (501) staff       (20)        1 2024-05-13 16:26:58.000000 func_parallelizer-0.2.0/func_parallelizer.egg-info/dependency_links.txt
+-rw-r--r--   0 vikashg    (501) staff       (20)        1 2024-05-13 16:11:29.000000 func_parallelizer-0.2.0/func_parallelizer.egg-info/not-zip-safe
+-rw-r--r--   0 vikashg    (501) staff       (20)       18 2024-05-13 16:26:58.000000 func_parallelizer-0.2.0/func_parallelizer.egg-info/top_level.txt
+-rw-r--r--   0 vikashg    (501) staff       (20)       38 2024-05-13 16:26:58.778374 func_parallelizer-0.2.0/setup.cfg
+-rw-r--r--   0 vikashg    (501) staff       (20)      558 2024-05-13 16:26:46.000000 func_parallelizer-0.2.0/setup.py
```

### Comparing `func_parallelizer-0.1.0/README.md` & `func_parallelizer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `func_parallelizer-0.1.0/func_parallelizer/func_parallelizer.py` & `func_parallelizer-0.2.0/func_parallelizer/func_parallelizer.py`

 * *Files identical despite different names*

### Comparing `func_parallelizer-0.1.0/setup.py` & `func_parallelizer-0.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r") as f:
+    description = f.read()
+
 setup(
     name='func_parallelizer',
-    version='0.1.0',
+    version='0.2.0',
     author='Vikash G',
     author_email='vikashgraja@gmail.com',
-    description="Func_Parallelizer is a simple Python module for parallel execution of functions "
-                "using multiprocessing. Ideal for parallel execution of heavy cpu operations",
+    description=description,
+    long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
```

