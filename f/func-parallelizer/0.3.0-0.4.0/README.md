# Comparing `tmp/func_parallelizer-0.3.0.tar.gz` & `tmp/func_parallelizer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_parallelizer-0.3.0.tar", last modified: Mon May 13 16:41:11 2024, max compression
+gzip compressed data, was "func_parallelizer-0.4.0.tar", last modified: Mon May 13 17:15:56 2024, max compression
```

## Comparing `func_parallelizer-0.3.0.tar` & `func_parallelizer-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 16:41:11.308828 func_parallelizer-0.3.0/
--rw-r--r--   0 vikashg    (501) staff       (20)     2550 2024-05-13 16:41:11.308909 func_parallelizer-0.3.0/PKG-INFO
--rw-r--r--   0 vikashg    (501) staff       (20)     2225 2024-05-12 17:47:47.000000 func_parallelizer-0.3.0/README.md
-drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 16:41:11.307678 func_parallelizer-0.3.0/func_parallelizer/
--rw-r--r--   0 vikashg    (501) staff       (20)       58 2024-05-12 17:29:31.000000 func_parallelizer-0.3.0/func_parallelizer/__init__.py
--rw-r--r--   0 vikashg    (501) staff       (20)      942 2024-05-13 16:05:35.000000 func_parallelizer-0.3.0/func_parallelizer/func_parallelizer.py
-drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 16:41:11.308688 func_parallelizer-0.3.0/func_parallelizer.egg-info/
--rw-r--r--   0 vikashg    (501) staff       (20)     2550 2024-05-13 16:41:11.000000 func_parallelizer-0.3.0/func_parallelizer.egg-info/PKG-INFO
--rw-r--r--   0 vikashg    (501) staff       (20)      301 2024-05-13 16:41:11.000000 func_parallelizer-0.3.0/func_parallelizer.egg-info/SOURCES.txt
--rw-r--r--   0 vikashg    (501) staff       (20)        1 2024-05-13 16:41:11.000000 func_parallelizer-0.3.0/func_parallelizer.egg-info/dependency_links.txt
--rw-r--r--   0 vikashg    (501) staff       (20)        1 2024-05-13 16:11:29.000000 func_parallelizer-0.3.0/func_parallelizer.egg-info/not-zip-safe
--rw-r--r--   0 vikashg    (501) staff       (20)       18 2024-05-13 16:41:11.000000 func_parallelizer-0.3.0/func_parallelizer.egg-info/top_level.txt
--rw-r--r--   0 vikashg    (501) staff       (20)       38 2024-05-13 16:41:11.309092 func_parallelizer-0.3.0/setup.cfg
--rw-r--r--   0 vikashg    (501) staff       (20)      563 2024-05-13 16:41:07.000000 func_parallelizer-0.3.0/setup.py
+drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 17:15:56.840391 func_parallelizer-0.4.0/
+-rw-r--r--   0 vikashg    (501) staff       (20)     2776 2024-05-13 17:15:56.840476 func_parallelizer-0.4.0/PKG-INFO
+-rw-r--r--   0 vikashg    (501) staff       (20)     2286 2024-05-13 17:10:23.000000 func_parallelizer-0.4.0/README.md
+drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 17:15:56.839261 func_parallelizer-0.4.0/func_parallelizer/
+-rw-r--r--   0 vikashg    (501) staff       (20)       58 2024-05-12 17:29:31.000000 func_parallelizer-0.4.0/func_parallelizer/__init__.py
+-rw-r--r--   0 vikashg    (501) staff       (20)      942 2024-05-13 16:05:35.000000 func_parallelizer-0.4.0/func_parallelizer/func_parallelizer.py
+drwxr-xr-x   0 vikashg    (501) staff       (20)        0 2024-05-13 17:15:56.840246 func_parallelizer-0.4.0/func_parallelizer.egg-info/
+-rw-r--r--   0 vikashg    (501) staff       (20)     2776 2024-05-13 17:15:56.000000 func_parallelizer-0.4.0/func_parallelizer.egg-info/PKG-INFO
+-rw-r--r--   0 vikashg    (501) staff       (20)      301 2024-05-13 17:15:56.000000 func_parallelizer-0.4.0/func_parallelizer.egg-info/SOURCES.txt
+-rw-r--r--   0 vikashg    (501) staff       (20)        1 2024-05-13 17:15:56.000000 func_parallelizer-0.4.0/func_parallelizer.egg-info/dependency_links.txt
+-rw-r--r--   0 vikashg    (501) staff       (20)        1 2024-05-13 16:11:29.000000 func_parallelizer-0.4.0/func_parallelizer.egg-info/not-zip-safe
+-rw-r--r--   0 vikashg    (501) staff       (20)       18 2024-05-13 17:15:56.000000 func_parallelizer-0.4.0/func_parallelizer.egg-info/top_level.txt
+-rw-r--r--   0 vikashg    (501) staff       (20)       38 2024-05-13 17:15:56.840706 func_parallelizer-0.4.0/setup.cfg
+-rw-r--r--   0 vikashg    (501) staff       (20)      757 2024-05-13 17:15:37.000000 func_parallelizer-0.4.0/setup.py
```

### Comparing `func_parallelizer-0.3.0/PKG-INFO` & `func_parallelizer-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,18 @@
-Metadata-Version: 2.1
-Name: func_parallelizer
-Version: 0.3.0
-Author: Vikash G
-Author-email: vikashgraja@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # func_parallelizer
 
 Func_Parallelizer is a simple Python module for parallel execution of functions using multiprocessing. 
 
 Ideal for parallel execution of heavy cpu operations like processing huge no of files in a directory or reading files for pandas.
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install func_parallelizer.
 
 ```bash
-pip install func_parallelizer
+pip install func-parallelizer
 ```
 
 ## Usage
 Import the required packages.
 
 ```python
 from func_parallelizer import parallel_runner
@@ -74,21 +63,21 @@
 
 By default all cores are used but if you have life and want to do some other things, I would recommend to use 50% to 80% of your CPU cores.
 ```python
 total_mayhem = parallel_runner(tasks, cpu_cores=2)
 ```
 ## Contributing
 
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate.
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate. [GIT Repo](https://github.com/vikashgraja/Func_Parallelizer)
 
 Feel free to ask any help(If it's about this package, dealing a lot IRL can't help yours too.)
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Code of Conduct
 
 Everyone interacting in the readme_renderer project's codebases, issue trackers,
 chat rooms, and mailing lists is expected to follow the [PSF Code of Conduct](https://github.com/pypa/.github/blob/main/CODE_OF_CONDUCT.md).
 
-Copyright © 2014, [The Python Packaging Authority].
+Copyright © 2014, [The Python Packaging Authority].
```

### Comparing `func_parallelizer-0.3.0/README.md` & `func_parallelizer-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,30 @@
+Metadata-Version: 2.1
+Name: func_parallelizer
+Version: 0.4.0
+Summary: Func_Parallelizer is a simple Python module for parallel execution of functions using multiprocessing. Ideal for parallel execution of heavy cpu operations
+Author: Vikash G
+Author-email: vikashgraja@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # func_parallelizer
 
 Func_Parallelizer is a simple Python module for parallel execution of functions using multiprocessing. 
 
 Ideal for parallel execution of heavy cpu operations like processing huge no of files in a directory or reading files for pandas.
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install func_parallelizer.
 
 ```bash
-pip install func_parallelizer
+pip install func-parallelizer
 ```
 
 ## Usage
 Import the required packages.
 
 ```python
 from func_parallelizer import parallel_runner
@@ -63,21 +75,21 @@
 
 By default all cores are used but if you have life and want to do some other things, I would recommend to use 50% to 80% of your CPU cores.
 ```python
 total_mayhem = parallel_runner(tasks, cpu_cores=2)
 ```
 ## Contributing
 
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate.
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate. [GIT Repo](https://github.com/vikashgraja/Func_Parallelizer)
 
 Feel free to ask any help(If it's about this package, dealing a lot IRL can't help yours too.)
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Code of Conduct
 
 Everyone interacting in the readme_renderer project's codebases, issue trackers,
 chat rooms, and mailing lists is expected to follow the [PSF Code of Conduct](https://github.com/pypa/.github/blob/main/CODE_OF_CONDUCT.md).
 
-Copyright © 2014, [The Python Packaging Authority].
+Copyright © 2014, [The Python Packaging Authority].
```

### Comparing `func_parallelizer-0.3.0/func_parallelizer/func_parallelizer.py` & `func_parallelizer-0.4.0/func_parallelizer/func_parallelizer.py`

 * *Files identical despite different names*

### Comparing `func_parallelizer-0.3.0/func_parallelizer.egg-info/PKG-INFO` & `func_parallelizer-0.4.0/func_parallelizer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: func-parallelizer
-Version: 0.3.0
+Version: 0.4.0
+Summary: Func_Parallelizer is a simple Python module for parallel execution of functions using multiprocessing. Ideal for parallel execution of heavy cpu operations
 Author: Vikash G
 Author-email: vikashgraja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -15,15 +16,15 @@
 
 Ideal for parallel execution of heavy cpu operations like processing huge no of files in a directory or reading files for pandas.
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install func_parallelizer.
 
 ```bash
-pip install func_parallelizer
+pip install func-parallelizer
 ```
 
 ## Usage
 Import the required packages.
 
 ```python
 from func_parallelizer import parallel_runner
@@ -74,15 +75,15 @@
 
 By default all cores are used but if you have life and want to do some other things, I would recommend to use 50% to 80% of your CPU cores.
 ```python
 total_mayhem = parallel_runner(tasks, cpu_cores=2)
 ```
 ## Contributing
 
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate.
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate. [GIT Repo](https://github.com/vikashgraja/Func_Parallelizer)
 
 Feel free to ask any help(If it's about this package, dealing a lot IRL can't help yours too.)
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `func_parallelizer-0.3.0/setup.py` & `func_parallelizer-0.4.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='func_parallelizer',
-    version='0.3.0',
+    version='0.4.0',
     author='Vikash G',
     author_email='vikashgraja@gmail.com',
+    description="Func_Parallelizer is a simple Python module for parallel execution of functions "
+                "using multiprocessing. Ideal for parallel execution of heavy cpu operations",
     long_description=description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

